# Requirements Traceability Matrix (RTM)
## Flight Reservation System

This matrix maps every UI screen and component to its requirement, test case description, and pass/fail status.

| Page | Requirement | Description | Test Case | Status | Complete |
|---|---|---|---|---|---|
| Welcome | Sign up button | Clicking Sign Up navigates to registration screen | — | Pass | ✅ |
| Welcome | Already have an account button | Clicking navigates to Login screen | — | Pass | ✅ |
| Sign Up | Already have an account button | Pressing navigates back to Login | — | Pass | ✅ |
| Sign Up | Signup button — valid all | All fields valid | E:T, P:T, FN:T | Pass | ✅ |
| Sign Up | Signup button — email invalid | Email invalid | E:T, P:T, FN:F | Pass | ✅ |
| Sign Up | Signup button — password invalid | Password invalid | E:T, P:F, FN:T | Pass | ✅ |
| Sign Up | Signup button — email+pass invalid | | E:T, P:F, FN:F | Pass | ✅ |
| Sign Up | Signup button — name invalid | | E:F, P:T, FN:T | Pass | ✅ |
| Sign Up | Signup button — two fields invalid | | E:F, P:T, FN:F | Pass | ✅ |
| Sign Up | Signup button — all invalid | | E:F, P:F, FN:T | Pass | ✅ |
| Sign Up | Signup button — all empty | | E:F, P:F, FN:F | Pass | ✅ |
| Login | Login information — valid | Valid credentials login | E:T, P:T | Pass | ✅ |
| Login | Login information — wrong password | | E:T, P:F | Pass | ✅ |
| Login | Login information — wrong email | | E:F, P:T | Pass | ✅ |
| Login | Login information — both wrong | | E:F, P:F | Pass | ✅ |
| Login | Login button | Navigates to Home | — | Pass | ✅ |
| Login | Forget Password button | Navigates to Forgot Password page | — | Pass | ✅ |
| Forgot Password | Forget password — valid email + save | | E:T, S:T | Failure | ❌ |
| Forgot Password | Forget password — valid email, no save | | E:T, S:F | Failure | ❌ |
| Forgot Password | Forget password — invalid email + save | | E:F, S:T | Failure | ❌ |
| Forgot Password | Forget password — all invalid | | E:F, S:F | Failure | ❌ |
| Forgot Password | Submit button | Navigates to confirmation | — | Failure | ❌ |
| Forgot Password | Back arrow | Returns to previous page | — | Pass | ✅ |
| Home | Rate Us button | Navigates to feedback screen | — | Pass | ✅ |
| Home | Search bar | Navigates to search screen | — | Failure | ❌ |
| Home | Riyadh card | Navigates to Riyadh booking screen | — | Pass | ✅ |
| Home | Doha card | Navigates to Doha booking screen | — | Pass | ✅ |
| Home | Istanbul card | Navigates to Istanbul booking screen | — | Pass | ✅ |
| Home | Dubai card | Navigates to Dubai booking screen | — | Pass | ✅ |
| Home | Go to page 2 button | Navigates to second page of destinations | — | — | — |
| Home | Account button | Navigates to Profile screen | — | Pass | ✅ |
| Home | Back arrow | Returns to previous page | — | Pass | ✅ |
| Home Page 2 | Rate Us button | Navigates to feedback screen | — | Pass | ✅ |
| Home Page 2 | Search bar | Navigates to search screen | — | Failure | ❌ |
| Home Page 2 | Cairo card | Navigates to Cairo booking | — | Pass | ✅ |
| Home Page 2 | Japan card | Navigates to Japan booking | — | Pass | ✅ |
| Home Page 2 | Kuwait card | Navigates to Kuwait booking | — | Pass | ✅ |
| Home Page 2 | Paris card | Navigates to Paris booking | — | Pass | ✅ |
| Home Page 2 | Back to page 1 button | Returns to first page of destinations | — | — | — |
| Booking (Riyadh) | Back arrow | Returns to previous page | — | Pass | ✅ |
| Booking (Riyadh) | Adults number | Counter increments adults count | — | Pass | ✅ |
| Booking (Riyadh) | Children number | Counter increments children count | — | — | — |
| Booking (Riyadh) | Price slider | Adjusts max price filter | — | — | — |
| Booking (Riyadh) | Dropdown list | Selects flight class | — | — | — |
| Booking (Riyadh) | Continue button | Navigates to payment screen | — | — | — |
| Booking (Doha) | Adults number | | — | Failure | ❌ |
| Booking (Doha) | Children number | | — | Failure | ❌ |
| Booking (Doha) | Price slider | | — | Pass | ✅ |
| Booking (Doha) | Dropdown list | | — | Pass | ✅ |
| Booking (Doha) | Continue button | | — | Pass | ✅ |
| Booking (Istanbul) | Adults number | | — | Failure | ❌ |
| Booking (Istanbul) | Children number | | — | Failure | ❌ |
| Booking (Istanbul) | Price slider | | — | Pass | ✅ |
| Booking (Istanbul) | Dropdown list | | — | Pass | ✅ |
| Booking (Istanbul) | Continue button | | — | Pass | ✅ |
| Booking (Dubai) | Adults number | | — | Failure | ❌ |
| Booking (Dubai) | Children number | | — | Failure | ❌ |
| Booking (Dubai) | Dropdown list | | — | Pass | ✅ |
| Booking (Dubai) | Continue button | | — | Pass | ✅ |
| Booking (Cairo) | Adults number | | — | Failure | ❌ |
| Booking (Cairo) | Children number | | — | Failure | ❌ |
| Booking (Cairo) | Price slider | | — | Pass | ✅ |
| Booking (Cairo) | Dropdown list | | — | Pass | ✅ |
| Booking (Cairo) | Continue button | | — | Pass | ✅ |
| Booking (Japan) | Adults number | | — | Failure | ❌ |
| Booking (Japan) | Children number | | — | Failure | ❌ |
| Booking (Japan) | Price slider | | — | Pass | ✅ |
| Booking (Japan) | Dropdown list | | — | Pass | ✅ |
| Booking (Japan) | Continue button | | — | Pass | ✅ |
| Booking (Kuwait) | Adults number | | — | Failure | ❌ |
| Booking (Kuwait) | Children number | | — | Failure | ❌ |
| Booking (Kuwait) | Price slider | | — | Pass | ✅ |
| Booking (Kuwait) | Dropdown list | | — | Pass | ✅ |
| Booking (Kuwait) | Continue button | | — | Pass | ✅ |
| Booking (Paris) | Adults number | | — | Failure | ❌ |
| Booking (Paris) | Children number | | — | Failure | ❌ |
| Booking (Paris) | Price slider | | — | Pass | ✅ |
| Booking (Paris) | Dropdown list | | — | Pass | ✅ |
| Booking (Paris) | Continue button | | — | Pass | ✅ |
| Payment | Back arrow | Returns to previous page | — | Pass | ✅ |
| Payment | Visa radio button | Selects Visa payment method | — | Pass | ✅ |
| Payment | Mastercard radio button | Selects Mastercard payment | — | Pass | ✅ |
| Payment | Bank transfer radio button | Selects bank transfer | — | Pass | ✅ |
| Payment | Confirm button | Proceeds to confirmation screen | — | Pass | ✅ |
| Payment | Account button | Navigates to Profile | — | Pass | ✅ |
| Payment | Cancel/Reschedule | Opens cancel or reschedule flow | — | Pass | ✅ |
| Confirmation | Back arrow | Returns to previous page | — | Pass | ✅ |
| Confirmation | Rate Us button | Navigates to feedback | — | Pass | ✅ |
| Confirmation | Confirm flight | Finalizes booking | — | Pass | ✅ |
| Confirmation | Cancel/Reschedule | Opens cancel or reschedule flow | — | Pass | ✅ |
| Track Flight | Back arrow | Returns to previous page | — | Pass | ✅ |
| Track Flight | SMS message button | Sends confirmation via SMS | — | Pass | ✅ |
| Track Flight | Email button | Sends confirmation via email | — | Pass | ✅ |
| Track Flight | Back to home button | Returns to Home | — | Pass | ✅ |
| Track Flight | Account button | Navigates to Profile | — | Pass | ✅ |
| Confirmation Sent | Back arrow | Returns to previous page | — | Pass | ✅ |
| Confirmation Sent | Account button | Navigates to Profile | — | Pass | ✅ |
| Confirmation Sent | Back to home button | Returns to Home | — | Pass | ✅ |
| Rate Us | Back arrow | Returns to previous page | — | Pass | ✅ |
| Rate Us | Description box | Allows user to enter feedback text | — | Pass | ✅ |
| Rate Us | Submit button | Submits feedback, navigates to Thank You | — | Pass | ✅ |
| Rate Us | Cancel button | Cancels and returns to Home | — | Pass | ✅ |
| Thank You | Account button | Navigates to Profile | — | Pass | ✅ |
| Thank You | Back to home button | Returns to Home | — | Pass | ✅ |
| Profile | Back arrow | Returns to previous page | — | Pass | ✅ |
| Profile | Rate Us button | Navigates to feedback | — | Pass | ✅ |
| Profile | Update password | Opens password update / logout flow | — | Pass | ✅ |
| Profile | Flight history button | Navigates to History screen | — | Pass | ✅ |
| Profile | Delete account button | Initiates account deletion | — | Pass | ✅ |
| Profile | Log out button | Logs out user and returns to Login | — | Pass | ✅ |
| Profile | Back to home button | Returns to Home | — | Pass | ✅ |
| History | Back arrow | Returns to previous page | — | Pass | ✅ |
| History | Rate Us button | Navigates to feedback | — | Pass | ✅ |

---

## Summary

| Status | Count |
|---|---|
| ✅ Pass | ~90 |
| ❌ Failure | ~20 (mainly: forgot password, search bar, adults/children counter on booking screens) |
| — Not Yet Tested | ~10 |

> **Main known failures:** Forgot Password flow is incomplete; the global search bar is not yet functional; the adults/children number counters on most booking pages fail.
