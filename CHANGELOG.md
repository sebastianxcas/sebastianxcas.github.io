# Changelog

All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 1.0.0 (2026-08-14)


### Features

* add 404 page and robots.txt ([167991e](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/167991e746da6029edf2c5570438591c605af6a9))
* add a glass search modal with a header trigger and ⌘K shortcut ([f9d1cde](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/f9d1cdeb6727925d5d56fe7abf9d2f70cd30bb4d))
* add About page; drop unused team collection ([7033063](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/703306359480e69e76cfe546ef7e9e53d4d3da17))
* add blog components and sample content ([d6f7378](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/d6f73784c01163a4a19168ae82e8708d724d02cd))
* add Pagefind search indexing behind a feature flag ([379f5cd](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/379f5cd6bf83635ff139c65662daed361a56ca4c))
* add Pagefind-powered site search behind a feature flag ([33b0a74](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/33b0a742fad08f395cae31ce0ddce801cfbbb643))
* add shared UI primitives and consolidate SEO ([c49aaec](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/c49aaec0575cc2e02b6ebcc8f49d8d208b167b71))
* **blog:** pagination, tag archives, TOC, RSS and prev/next ([3a57cf4](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/3a57cf4d13925c184a3f4f49b8e2db21f21c0c32))
* **images:** run blog/project images through astro:assets ([a98a8be](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/a98a8be41835cc1d13da1ba43f64cd3c927bb6c7))
* implement blog list and article pages ([f91eb4a](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/f91eb4a64198de3e1410522a15b1229e6dfeca79))
* initial project setup with Astro ([44e0d11](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/44e0d1141a047a59227c966d8e63bc8c28e30d6b))
* **landing:** static EC landing template and showcase home ([2abe7ee](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/2abe7eed27f5a3e68081df81bedc1538575bfbe6))
* **portfolio:** work archive, project detail, gallery and samples ([46700fc](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/46700fc6917ca4835bc433c55730bcda4792295c))
* refine favicon and add full app icon set ([a1325d0](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/a1325d0e2342327cb07214e7961925fd6077e34a))
* upgrade to Astro 7 and migrate to Content Layer API ([712e704](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/712e704df57289426df544f9a0b8564789a15fb8))
* wire previously-inert site.config options ([744a5b7](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/744a5b701322043dcfd8c12f70c642563448ad83))


### Bug Fixes

* **a11y:** meet AA contrast for accent text and fix skip-link focus ([daa5739](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/daa57391a475afe3f90ccb55bd90cf63921f6d63))
* **a11y:** take closed mobile nav out of the tab order; fix active state ([797cb7b](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/797cb7b3d899fb379b442792f4f7536c0a72da50))
* add sharp as a direct dev dependency ([18b425f](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/18b425fc1b1f74dffd806202754923e53f010ce5))
* **blog:** don't show a bogus reading time for MDX posts ([e3d72f0](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/e3d72f038d0e3997664663f988cc56aaa740165e))
* **blog:** honour blog.showReadingTime on the post card grid ([a71e7cc](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/a71e7cc5941d5229e0966ee111d24ba7637a2c31))
* drive homepage/landing brand and source link from siteConfig ([d0e2a5c](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/d0e2a5c0b736876d211ebac27851600aced3bc87))
* guard optional social link in footer credit ([c771aaa](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/c771aaaf9937bb3a9e512b484f388cb9f2f69a97))
* guard the search modal against stale results and a nullable input ([c7177ee](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/c7177ee790120678cccc833f2a11b94950303d6d))
* load the Pagefind bundle via an opaque dynamic import ([7be6035](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/7be603564fb5bd7297c630e65c3a15611abf49e2))
* **portfolio:** only show tech filter on a single-page archive ([0334c29](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/0334c29b44fa1c72e9086ad2d60d4c3d3edc1fed))
* **seo:** escape &lt; in JSON-LD to prevent &lt;/script&gt; breakout ([cff8065](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/cff80656112688bae6e6f1853031c01431a89c2f))
* **tags:** group tags by slug to avoid collisions and empty routes ([d475ee4](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/d475ee4a24e748f776f6704c21eb6c7395ad3f22))
* **theme:** guard localStorage and separate selected/resolved theme state ([3d80f50](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/3d80f5082c7c2dfc86ec1089211512438e441337))
* v1.1.1 バグ修正まとめ（[#17](https://github.com/sebastianxcas/sebastianxcas.github.io/issues/17)-[#25](https://github.com/sebastianxcas/sebastianxcas.github.io/issues/25)） ([#49](https://github.com/sebastianxcas/sebastianxcas.github.io/issues/49)) ([6b5f0fb](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/6b5f0fbd0e00d279ec45302950f67b08bbbf182c))
* v1.2.0 まとめ（[#26](https://github.com/sebastianxcas/sebastianxcas.github.io/issues/26)-[#42](https://github.com/sebastianxcas/sebastianxcas.github.io/issues/42)） ([#50](https://github.com/sebastianxcas/sebastianxcas.github.io/issues/50)) ([cedac9b](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/cedac9b86a966675145385509311d8c0706c1765))


### Performance Improvements

* drop nested backdrop-filter from Badge and Tag ([7761b47](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/7761b477da2b1d83303cac472e875113ee7bb9e1))
* pause aurora animation while the tab is hidden ([0655b59](https://github.com/sebastianxcas/sebastianxcas.github.io/commit/0655b59a30261cf00f40a806080f514484d1d8a1))

## [1.2.0] - 2026-07-26

### Added

- `site.config` now exposes `lang` / `ogLocale`, so `<html lang>` and `og:locale` can be configured per site instead of being hardcoded ([#34](https://github.com/kpab/astro-haze/issues/34))
- Work detail pages now emit `CreativeWork` JSON-LD structured data and `og:type=article` ([#40](https://github.com/kpab/astro-haze/issues/40))
- The search modal now opens/closes with a fade + scale transition, disabled under `prefers-reduced-motion` ([#30](https://github.com/kpab/astro-haze/issues/30))
- CI now runs `astro check` and `astro build` on every pull request, plus an ESLint/Prettier lint gate ([#41](https://github.com/kpab/astro-haze/issues/41), [#42](https://github.com/kpab/astro-haze/issues/42))

### Fixed

- Hover states (cards, links, buttons) no longer stick after a tap on touch devices ([#26](https://github.com/kpab/astro-haze/issues/26))
- Interactive elements below the 44px touch-target minimum — the menu toggle, buttons, pagination and filters — are now sized to meet it ([#27](https://github.com/kpab/astro-haze/issues/27))
- Full-height sections now fall back correctly on iOS Safari, where `100vh` doesn't account for the collapsing toolbar ([#28](https://github.com/kpab/astro-haze/issues/28))
- The mobile nav now locks background scroll while open (without clobbering the search modal's own scroll lock), has a fallback for browsers without `backdrop-filter`, and derives its offset from a shared header-height variable ([#29](https://github.com/kpab/astro-haze/issues/29))
- Search result counts are now announced to screen readers ([#31](https://github.com/kpab/astro-haze/issues/31))
- `ThemeToggle` now announces the current theme state to screen readers ([#35](https://github.com/kpab/astro-haze/issues/35))
- Gradient brand text now falls back to a solid color where `background-clip: text` isn't supported, and the skip link now meets contrast requirements in both themes ([#36](https://github.com/kpab/astro-haze/issues/36))
- External links now announce "opens in new tab" and are auto-detected from `href` instead of requiring manual tagging, including when a caller also passes a custom `aria-label` ([#37](https://github.com/kpab/astro-haze/issues/37))
- The work/project filter now shows an empty state (instead of a blank grid) when no items match, and animates items in on filter change ([#38](https://github.com/kpab/astro-haze/issues/38))
- Internal links and canonical URLs are now consistently trailing-slashed, matching the site's `trailingSlash: 'always'` config ([#39](https://github.com/kpab/astro-haze/issues/39))

### Changed

- `transition: all` has been replaced with explicit property lists across components, and buttons now have a dedicated `:active` press feedback state ([#32](https://github.com/kpab/astro-haze/issues/32))
- Media query breakpoints have been consolidated from 13 ad-hoc values down to a standard set (640/768/900/1024px) ([#33](https://github.com/kpab/astro-haze/issues/33))

## [1.1.1] - 2026-07-26

### Fixed

- Site name no longer doubles up in page `<title>` / `og:title` when a page passes its own title ([#17](https://github.com/kpab/astro-haze/issues/17))
- Footer no longer links to `/privacy` / `/terms`, which the theme doesn't ship ([#18](https://github.com/kpab/astro-haze/issues/18))
- Footer nav now respects `features.*` flags, so a disabled section (e.g. `blog`) no longer leaves a dead link there ([#19](https://github.com/kpab/astro-haze/issues/19))
- RSS `<channel>` link now includes the configured `base`, instead of pointing at the origin root ([#20](https://github.com/kpab/astro-haze/issues/20))
- Blog post dates now render in UTC, so the displayed date no longer shifts with the build host's timezone ([#21](https://github.com/kpab/astro-haze/issues/21))
- `prose` tables now scroll horizontally on narrow viewports instead of overflowing, and long words wrap instead of being clipped ([#22](https://github.com/kpab/astro-haze/issues/22))
- Root-relative image paths (string form) and `links.case` on project pages now go through `withBase`, fixing potential 404s under a subpath deploy ([#23](https://github.com/kpab/astro-haze/issues/23))
- Featured posts no longer appear a second time in the blog list's "Latest Posts" grid — including when a featured post falls on a later pagination page ([#24](https://github.com/kpab/astro-haze/issues/24))
- Documented that `public/robots.txt` and `public/_headers` are not served/applied on GitHub Pages ([#25](https://github.com/kpab/astro-haze/issues/25))

## [1.1.0] - 2026-07-17

### Added

- Pagefind-powered static site search behind a new `features.search` flag ([#1](https://github.com/kpab/astro-haze/pull/1))
  - Search index generated during `astro build` via the `astro-pagefind` integration — no deploy-workflow changes needed
  - Glass search modal (native `<dialog>`) opened from a header button or <kbd>⌘K</kbd> / <kbd>Ctrl+K</kbd>, with ↑/↓ result navigation
  - Pagefind bundle lazy-loaded on first open; site chrome excluded from the index with `data-pagefind-ignore`

## [1.0.0] - 2026-06-30

### Added

- Initial release: glassmorphism multi-purpose Astro 7 theme
  - Reusable glass UI system with aurora backgrounds, light/dark theme toggle
  - Paginated blog with tags, table of contents, reading time and share links
  - Portfolio with technology filters, case-study pages and responsive galleries
  - Config-driven e-commerce landing page
  - SEO (canonical, Open Graph, Twitter cards, JSON-LD), RSS feed and XML sitemap
  - Optimized images (AVIF/WebP via `astro:assets`), accessibility and reduced-motion support

[1.2.0]: https://github.com/kpab/astro-haze/compare/v1.1.1...v1.2.0
[1.1.1]: https://github.com/kpab/astro-haze/compare/v1.1.0...v1.1.1
[1.1.0]: https://github.com/kpab/astro-haze/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/kpab/astro-haze/releases/tag/v1.0.0
