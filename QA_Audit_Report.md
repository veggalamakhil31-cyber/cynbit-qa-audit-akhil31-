# QA Audit Report - Detailed Test Execution
Tester: Akhil | Date: 31-Oct-2026 | Environment: Chrome 124, Win11

Test Scope: cynbit.in Website
Modules: Homepage, Services, Contact Form, Footer, Performance

TC-001: Contact Form Validation UX - PARTIAL PASS (Real Test by Akhil)
Steps: Open cynbit.in/contact > Leave Full Name empty > Click SEND INQUIRY
Expected: Custom styled inline error "Full Name is required" with red border
Actual: Only browser native tooltip "Please fill in this field" shows, no custom UI, no inline message, UX needs improvement. Functional validation present but needs custom styling. Real evidence captured on HP laptop 31-10-2026 by Akhil
Bug ID: CB-101 | Severity: Low (UX Improvement) | Status: Functional OK, UX Needs Improvement
Evidence: 06_manual_contact_test_akhil_real.png (Real laptop photo) & 01_contact_form_validation_browser_default.png

TC-002: Mobile Responsive - Services Section - FAIL
Steps: DevTools 360x800 > Check Services
Expected: Cards stack vertically
Actual: Horizontal scroll overflow, layout broken
Bug ID: CB-1024 | Severity: Medium
Evidence: 02_mobile_360px_overflow.png

TC-003: Performance Lighthouse - FAIL
Steps: Lighthouse > Performance > Analyze
Expected: Performance >=90
Actual: Score 62, LCP 4.8s, Images 1.9MB unoptimized
Bug ID: QA-2847 | Severity: Medium
Evidence: 03_lighthouse_performance_62.png

TC-004: Footer Social Links - FAIL
Steps: Footer > Inspect LinkedIn Instagram links
Expected: Valid URLs
Actual: href="#" dead links
Bug ID: CYNBIT-112 | Severity: Low
Evidence: 04_footer_social_links_dead.png

TC-005: Console Favicon 404 - FAIL
Steps: F12 Console
Expected: Favicon loads no error
Actual: GET favicon.ico 404 Not Found
Bug ID: CYB-1024 | Severity: Low
Evidence: 05_favicon_404_console_error.png

Conclusion: 5 critical issues found, needs fixing before release.
