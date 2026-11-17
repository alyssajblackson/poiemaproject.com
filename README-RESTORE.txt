POIEMA PROJECT: ORIGINAL WEBSITE + BIGGER NAVIGATION

This restores the original Poiema design, fonts, palette, copy and layout.
The editorial theme is removed completely. Navigation labels alone have
been enlarged, including the mobile menu. The newer Menstrual Classes links,
Home and Learn invitations, and contact inquiry option are retained.

TO UPDATE GITHUB
1. Unzip this package.
2. Open https://github.com/alyssajblackson/poiemaproject.com
3. Upload the HTML files from this ZIP to the top level of the repository.
4. Commit, replacing the matching HTML files. Do not delete any other files.
5. Remove poiema-editorial.css from the repository if desired: this package
   no longer references it, so it will not affect the website either way.
6. Keep all existing images, PDFs, CNAME, and other site files.

IMPORTANT: The earlier redesign uploaded a September-era Work With Me page.
This package restores its original styling, but for an exact byte-for-byte
restore of that page's most recent footer layout, first use GitHub's history
to recover work-with-me.html from the November 10 commit (60f7ab869d17).
The other files restore the original page presentation. The Menstrual Classes
page was not included in the redesign and remains unchanged; its navigation
text size can be updated separately using the same CSS snippet below.

GITHUB HISTORY (exact original snapshot before WEB REDO):
https://github.com/alyssajblackson/poiemaproject.com/tree/60f7ab869d17

NAVIGATION STYLING (if applying to the Menstrual Classes page):

/* Only requested change: larger navigation text. Retains original colors and fonts. */
@media (min-width: 1121px) {
  nav .nav-links { gap: clamp(.78rem, 1.25vw, 1.35rem); }
  nav .nav-links a, nav .nav-cta {
    font-size: 1.04rem;
    letter-spacing: .055em;
  }
  nav .nav-logo-text { font-size: 1.27rem; }
}
.mobile-menu a { font-size: 1.15rem; }
