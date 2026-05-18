# Section A — Validation Criteria and Checklist Development

# Q1. Validation Criteria Engineering

## Scenario
A university management system provides:
- Student login
- Online assignment submission
- Attendance tracking
- Faculty dashboard
- Activity logging

---

# 1. Measurable Validation Criteria

| System Feature | Stakeholder Expectation | Validation Criteria | Measurement Method |
|---|---|---|---|
| Student Login | Secure and successful login | Login success rate ≥ 95% | Functional testing |
| Student Login | Unauthorized users blocked | Invalid credentials rejected 100% | Security testing |
| Assignment Submission | Assignments upload correctly | File upload success within 5 seconds | Performance testing |
| Assignment Submission | No duplicate submissions | Duplicate prevention works correctly | Validation testing |
| Attendance Tracking | Accurate attendance records | Attendance accuracy = 100% | Database verification |
| Faculty Dashboard | Dashboard loads quickly | Dashboard response time ≤ 3 seconds | UI testing |
| Activity Logging | User actions are logged | Every critical action stored in logs | Log verification |

---

# 2. Structured Validation Checklist

| ID | Module | Validation Item | Expected Result | Status | Evidence |
|---|---|---|---|---|---|
| VC-01 | Login | Valid student login | User redirected to dashboard | Pass/Fail | Screenshot |
| VC-02 | Login | Invalid login attempt | Access denied | Pass/Fail | Log file |
| VC-03 | Assignment | Upload assignment | File uploaded successfully | Pass/Fail | Upload evidence |
| VC-04 | Assignment | Duplicate upload prevention | Duplicate blocked | Pass/Fail | Screenshot |
| VC-05 | Attendance | Mark attendance | Attendance stored correctly | Pass/Fail | Database record |
| VC-06 | Faculty Dashboard | View reports | Reports displayed correctly | Pass/Fail | Screenshot |
| VC-07 | Logging | User activity logging | Logs generated successfully | Pass/Fail | Log evidence |
| VC-08 | Security | Session timeout | User auto logout after inactivity | Pass/Fail | Screenshot |

---

# Purpose of Validation Checklist

The validation checklist helps:
- verify functional requirements,
- maintain validation evidence,
- improve traceability,
- support audit and compliance review.

---

# Conclusion

The validation criteria ensure that all system features are measurable and testable. The checklist provides structured documentation for validation and quality assurance activities.
