#Paystack Auto-Referral Engine
Automates paystack payment process, updates Google sheets, send confirmation emails and routes referrals to partners or students.

##overview
This make.com automaton handles end-end payment verification and referral routing:

1. **Payment Trigger** : Listen for incoming payment webhooks via paystack.

2. **Sheet Update & Email** : Validates transactions in Google sheet, updates row statues and dispatches customers emails via Gmail.
   
3. **Conditional Referral Routing** 

**Partner Flow** : MatchesThe referral code and increments partner statusin the Goggle Sheets.

**Student Flow** : Matches the student and ID and updates referral credits.


## Setup Instructions

1. Export your Make.com Scenario blueprint as a `.json` file and upload it to this repository.

2. Configure webhook connection for paystack, Gmail and Goggle Sheets in make.com.

3. Map your target spreadsheet column header to match the scenario Variables.  
