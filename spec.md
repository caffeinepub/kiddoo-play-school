# Kiddoo Play School

## Current State
Full-stack play school website with sections: Hero, About, Programs, Why Us, Gallery, Testimonials, Contact, Footer. All content is static/frontend. School details (address, phone, email, founded year) are up to date.

## Requested Changes (Diff)

### Add
- Announcements section with two columns: one for Teachers and one for Parents
- Each column shows a list of sample announcements (date, title, short description)
- Add "Announcements" link to the navbar and footer

### Modify
- NAV_LINKS: add Announcements entry pointing to `#announcements`
- App component: include AnnouncementsSection between WhyUsSection and GallerySection

### Remove
- Nothing removed

## Implementation Plan
1. Add ANNOUNCEMENTS data constant with teacher-specific and parent-specific arrays (date, title, description)
2. Create AnnouncementsSection component with two-column layout; each column has a colored header and a list of announcement cards
3. Add `{ label: "Announcements", href: "#announcements" }` to NAV_LINKS
4. Insert <AnnouncementsSection /> in App between WhyUsSection and GallerySection
5. Apply data-ocid markers to announcement items and section
