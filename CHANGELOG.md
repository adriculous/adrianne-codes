# Changelog

All notable changes to this project will be documented here.

---

## 2026-04-28: New Learn Notes About CSS Specificity

### Added
- Added new **Learn** notes: *Why Your CSS Isn't Working: A Friendly Guide to Specificity*

### Fixed
- Fixed the headless path for `/learn/index.astro`, so that posts will be linked to its own page, not at the Hashnode page.

---

## 2026-04-22: Hashnode Integration & Content System Update

### Added
- Hashnode headless CMS integration using GraphQL
- `client.ts` and `schema.ts` for structured data fetching
- Dynamic routing for posts via `/post/[slug].astro`
- Tuts page now pulls live posts from Hashnode
- Category-based filtering system using tags (SSGs, CSS, WordPress, Python, Daily Tools, Archive)
- Styled category sections with color-coded top borders

### Changed
- Refactored `/tuts/index.astro` to support:
  - Latest Tutorials section (recent posts)
  - Category-based sections driven by tags
- Updated tutorial links to use internal Astro routes instead of external Hashnode URLs
- Improved UI consistency between category cards and content sections
- Updated Adrianne Codes case study to reflect hybrid content system

### Fixed
- Resolved TypeScript issues in Astro files (`any` type errors and missing imports)
- Fixed Hashnode posts not appearing due to incorrect filtering logic
- Corrected GraphQL data handling (`edges → node` structure)

### Notes
- Adopted a hybrid content workflow:
  - Local Markdown for structured case studies and project pages
  - Hashnode CMS for content-heavy sections (Tuts and Learn)
- Followed official Astro and Hashnode documentation for stable integration

---

## 2026-04-16: Initial Build

### Added
- Initial Astro project setup
- Base layout (`Layout.astro`) and global styling
- Navigation and footer components
- Core pages: Home, Projects, Tuts, Learn, About, Contact
- Markdown support for Learn and case studies
- First Learn post: fixing GitHub push permission error
- CHANGELOG.md

### Changed
- Replaced default Astro README with custom project README
- Refined layout structure (site shell, sidebar, content areas)
- Updated Learn page to support categorized links

### Fixed
- GitHub permission denied error when pushing (switched from HTTPS to SSH)

### Notes
- Project is a rebuild of Adrianne Codes as a frontend + technical writing portfolio using Astro

---

## 2026-04-16: Initial Build

### Added
- Initial Astro project setup
- Base layout (Layout.astro) and global styling
- Navigation and footer components
- Core pages: Home, Projects, Tuts, Learn, About, Contact
- Markdown support for Learn and case studies
- First Learn post: fixing GitHub push permission error
- CHANGELOG.md

### Changed
- Replaced default Astro README with custom project README
- Refined layout structure (site shell, sidebar, content areas)
- Updated Learn page to support categorized links

### Fixed
- GitHub permission denied error when pushing (switched from HTTPS to SSH)

### Notes
- Project is a rebuild of Adrianne Codes as a frontend + technical writing portfolio using Astro
