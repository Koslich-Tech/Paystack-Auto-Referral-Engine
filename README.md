# Paystack Auto-Referral Engine

Automates the Paystack payment verification process, updates Google Sheets, dispatches confirmation emails, and routes referrals to partners or students.

## Overview

This Make.com automation scenario handles end-to-end payment verification and referral routing:

1. **Payment Trigger**: Listens for incoming payment webhooks via Paystack.
2. **Sheet Update & Email**: Validates transactions in Google Sheets, updates row statuses, and dispatches customer confirmation emails via Gmail.
3. **Conditional Referral Routing**:
   - **Partner Flow**: Matches the partner referral code and increments partner commission/status in Google Sheets.
   - **Student Flow**: Matches the student ID and updates referral credits.

---

## Setup Instructions

1. Export your Make.com scenario blueprint as a `.json` file and upload it to this repository.
2. Configure webhook connections for Paystack, Gmail, and Google Sheets in Make.com.
3. Map your target spreadsheet column headers to match the scenario variables.
