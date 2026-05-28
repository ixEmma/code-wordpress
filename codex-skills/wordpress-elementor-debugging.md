# WordPress & Elementor Debugging Skill

## Purpose

Use this skill when diagnosing WordPress, Elementor, hosting, server, caching, REST API, or editor-preview failures.

The goal is to identify the failing layer first, then recommend targeted, reversible fixes. Do not guess. Do not immediately blame Elementor or plugins. Diagnose the system layer before changing settings.

## Core Rules

1. Identify the failing layer before recommending fixes.
2. Read logs, browser console errors, and network requests before changing settings.
3. Prefer reversible actions first.
4. Do not delete plugins, themes, files, or database tables for testing.
5. Do not disable all plugins as the first step.
6. Use Elementor Safe Mode before full plugin isolation.
7. Document every change so it can be rolled back.
8. Treat caching, OPcache, object cache, CDN, and firewall issues as serious suspects.
9. Always separate symptoms from root causes.
10. Explain what failed, why it failed, and how the fix resolves the issue.

## Layer Identification Matrix

When a WordPress or Elementor problem is reported, classify it into one likely layer first.

| Layer | Common Symptoms |
|---|---|
| Browser | JavaScript errors, CORS errors, asset 404s, broken editor UI |
| CDN or Firewall | Cached errors, blocked admin requests, firewall blocks, timeout errors |
| DNS or SSL | Site unreachable, redirect mismatch, certificate problems |
| Server | 503, 502, 504, connection refused, timeout errors |
| PHP or PHP-FPM | 500 errors, white screen, fatal errors, memory exhaustion |
| WordPress Core | Redirect loops, wp-login issues, REST API 401 or 403 |
| Plugin | Conflicts after update, AJAX failures, specific feature breakage |
| Theme | Visual breakage, template hierarchy problems, layout override issues |
| Database | Slow queries, locked tables, connection limits, table corruption |
| Elementor | Preview not loading, editor blank, missing widgets, CSS not generated |

## Diagnostic Order

Use this order before recommending fixes:

1. Confirm the exact symptom.
2. Identify the likely failing layer.
3. Check browser DevTools if the issue is visual, editor-related, or frontend-related.
4. Check server and PHP logs if the issue is 500, 503, white screen, or timeout-related.
5. Check REST API and admin AJAX if the issue affects Elementor editor or preview.
6. Check cache/CDN/firewall if the issue appears inconsistent or works in one environment but not another.
7. Use Elementor Safe Mode for Elementor-specific editor failures.
8. Only then isolate plugins or theme conflicts.

## Elementor Preview Could Not Be Loaded

Likely layer: REST API, AJAX, firewall, cache, or Elementor preview iframe.

Check:

1. Visit `/wp-json/wp/v2/posts` and confirm it returns JSON.
2. Confirm `/wp-json/` is not blocked by security plugins, firewall rules, or `.htaccess`.
3. Confirm `/wp-admin/admin-ajax.php` is not blocked.
4. Check browser DevTools Console for JavaScript errors.
5. Check browser DevTools Network tab for 401, 403, 404, or 500 requests.
6. Enable Elementor Safe Mode.
7. Regenerate Elementor CSS and data.
8. Clear all cache layers: plugin cache, server cache, CDN cache, OPcache, and object cache.
9. Temporarily disable JavaScript optimization, defer, delay, combine, or minify settings.
10. Check Elementor system info and logs.

Do not assume Elementor itself is broken until REST API, AJAX, cache, and firewall layers are checked.

## Elementor Editor Blank or Not Loading

Likely layer: browser, assets, JavaScript optimization, cache, or Elementor-generated files.

Check:

1. Open DevTools Console.
2. Record all JavaScript errors.
3. Open DevTools Network tab.
4. Filter by JavaScript and CSS files.
5. Look for 404, 403, 500, blocked, or MIME type errors.
6. Regenerate Elementor files and data.
7. Clear cache layers.
8. Disable JavaScript optimization temporarily.
9. Check if Rocket Loader, LiteSpeed delay JS, WP Rocket delay JS, or similar optimization is breaking the editor.
10. Flush OPcache and object cache after plugin or PHP changes.

## 503 Service Unavailable

Likely layer: server, PHP-FPM, hosting resource limits, or database overload.

Check:

1. Server error logs.
2. PHP-FPM status if available.
3. PHP memory limit.
4. PHP worker limits.
5. Database status and connection count.
6. Hosting resource usage.
7. Recent plugin, theme, or PHP version changes.

Recommended fix order:

1. Restart PHP-FPM or hosting PHP service if allowed.
2. Clear server cache.
3. Increase PHP memory only if logs prove memory exhaustion.
4. Investigate the plugin, process, request, or query causing resource exhaustion.
5. Review hosting limits if repeated 503s occur.

Do not treat a 503 as an Elementor design issue. It is usually infrastructure or resource-related.

## White Screen of Death

Likely layer: PHP fatal error.

Check:

1. Enable debug logging with public display off.
2. Read `/wp-content/debug.log`.
3. Identify the exact file, function, plugin, theme, and line number causing the fatal error.
4. Check PHP version compatibility.
5. If the issue appeared after an update, deactivate the suspected plugin or theme safely.
6. If the theme is suspected, switch to a default WordPress theme only after backup or safe access is confirmed.

Use this pattern in `wp-config.php` only when needed:

```php
define('WP_DEBUG', true);
define('WP_DEBUG_LOG', true);
define('WP_DEBUG_DISPLAY', false);