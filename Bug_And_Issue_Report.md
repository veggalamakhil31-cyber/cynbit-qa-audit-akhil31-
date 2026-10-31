# Bug and Issue Report - REAL EVIDENCE 31 Oct 2026

Reported By: Akhil Kumar | Date: 31-Oct-2026 | Environment: Chrome 124 Win11 HP Laptop | Real Manual Testing

## HIGH PRIORITY BUGS - VALIDATED WITH SCREENSHOTS

### CB-102: Full Name Accepts Numbers 12345 [HIGH] - CONFIRMED BUG

- **File:** Before_BUG02_before_fullname_12345.png (Input) + BUG02_after_inquiry_received_31oct.png (Proof)
- **Steps:**
    1. Go to cynbit.in/contact on HP Laptop
    2. Full Name = 12345
    3. Email = akhil@gmail.com  
    4. Company = 123456789
    5. Message = test
    6. Click SEND INQUIRY
    7. Result: INQUIRY RECEIVED - BUG CONFIRMED!
- **Expected:** Should reject numbers, show "Please enter valid name"
- **Actual:** Accepts 12345 as valid name - HIGH BUG - REAL LAPTOP EVIDENCE 31 Oct

### CB-101: Contact Form Validation Missing - Email

- **File:** BUG01_email_validation_missing_real_31oct_1536.png
- **Status:** CONFIRMED - Email validation missing

### Other Issues:
- CB-1024 - Services overflow on 360px mobile - Medium
- QA-2847 - Performance score 62 Low - Medium
- CYNBIT-112 - Footer LinkedIn Instagram dead links
- CYB-1024 - favicon.ico 404 Not Found - Low
- CB-103 - No loading state on submit - Low
- CB-104 - Missing alt text on hero images - Medium
- CB-105 - Inconsistent button hover states - Low
