# Email Analysis #7 – Invoice Fraud (Vendor Impersonation)

## Email Summary
This email is a **Vendor Impersonation** attack, a type of **Business Email Compromise (BEC)**, in which the attacker pretends to be a trusted supplier and requests the finance department to update the vendor's bank account details. The attacker claims that the company has undergone a banking migration and asks that all future payments be sent to a new bank account provided in an attached document. The objective of this attack is to redirect legitimate business payments into a fraudulent bank account, resulting in significant financial loss.

## Email Details

**Sender:** billing@globaltech-supplies.com

**Recipient:** finance@company.com

**Subject:** Updated Bank Details for Invoice #GT-45821

**Attachment:** Updated_Bank_Details.pdf

**Attack Type:** Vendor Impersonation / Business Email Compromise (BEC) / Payment Redirection Fraud

## Email Objective
The objective of this attack is to convince the finance department to replace the vendor's legitimate bank account details with a fraudulent account controlled by the attacker. Once the payment information is updated, future invoice payments intended for the vendor will be redirected to the attacker's account.

# Technical Analysis

## 1. Sender Verification

The sender's email address should be carefully verified before trusting the request. Although the email appears to come from a legitimate supplier, the sender's domain should always be compared with the vendor's officially registered domain. Any unexpected or slightly different domain name should be treated as suspicious until independently verified.
Attackers frequently impersonate trusted vendors because employees are less likely to question communications from organizations they already do business with.

## 2. Email Authenticity

The email appears professional and polite, which increases its credibility. It explains that the company has completed a **banking migration**, making the request seem like a routine business update.
The email does not ask for passwords or sensitive information, making it less suspicious than traditional phishing emails. Instead, it manipulates normal business operations by requesting changes to vendor payment records.

## 3. Subject Analysis

The subject line **"Updated Bank Details for Invoice #GT-45821"** appears legitimate because it references a specific invoice number and relates to a routine financial process.
Employees in finance departments regularly receive invoice-related emails, making this request appear normal and reducing suspicion.

## 4. Attachment Analysis

The email contains an attachment named **"Updated_Bank_Details.pdf"**, which is intended to provide the new payment information.
The attachment makes the email appear more professional and convincing. It may contain fraudulent bank account details or, in some attacks, even malicious content. Employees should never trust payment information contained in an attachment without first verifying it through official communication channels.

## 5. Why the Email Appears Legitimate
Several characteristics make this email appear convincing.

- It impersonates a trusted vendor.
- It provides a believable explanation by mentioning a banking migration.
- It references a specific invoice number.
- It uses a professional tone.
- It includes an attachment that resembles official financial documentation.
- It requests an update to financial records rather than an immediate payment, making the request appear routine.

## 6. Social Engineering Analysis
The attacker uses several social engineering techniques to manipulate the recipient.

- **Authority:** Pretends to represent the vendor's Accounts Manager.
- **Trust:** Exploits the existing business relationship with the supplier.
- **Familiarity:** Uses a vendor the company is expected to recognize.
- **Urgency:** Requests immediate record updates to avoid payment delays.
- **Responsibility:** Encourages the finance department to act quickly to maintain normal business operations.

## 7. Attack Flow

Email Delivered
        ↓
Finance employee trusts the email
        ↓
Attachment is opened
        ↓
Bank account details are updated
        ↓
Future invoice payments are sent to the fraudulent account
        ↓
Attacker receives legitimate business payments
        ↓
Financial Loss to the organization

## 8. Risk Assessment

**Risk Rating:** Critical
This attack is classified as **Critical** because it directly targets an organization's financial operations.

If successful, the attacker may:

- Redirect legitimate invoice payments.
- Cause significant financial losses.
- Disrupt business relationships with vendors.
- Delay supplier payments.
- Damage the organization's reputation.
- Create legal and financial disputes between the organization and the genuine vendor.

Unlike credential theft attacks, this attack manipulates business processes rather than technical systems.

## 9. Possible Impact
A successful attack could result in:

- Payment Redirection Fraud.
- Business Email Compromise (BEC).
- Financial loss.
- Delayed vendor payments.
- Business disruption.
- Loss of trust between the company and its suppliers.
- Increased investigation and recovery costs.
- Reputational damage.

## 10. Incident Response
If this email is received, employees should:

- Do not update vendor bank details immediately.
- Verify the sender's email address carefully.
- Contact the vendor using previously verified phone numbers or official contact information.
- Perform **Out-of-Band (OOB) Verification** before making any banking changes.
- Confirm the request with the Finance Manager or appropriate authority.
- Report the email to the Information Security or SOC Team if it appears suspicious.
- Delete the email after it has been reported.

If payment information has already been updated:

- Immediately suspend pending payments.
- Contact the legitimate vendor.
- Notify the organization's finance department.
- Inform the bank if fraudulent payments have been initiated.
- Begin an internal fraud investigation.

## 11. Financial Controls That Could Prevent This Attack
Organizations should implement strong financial controls, including:

- Mandatory Out-of-Band (OOB) Verification for all vendor bank account changes.
- Dual approval before updating payment information.
- Formal vendor change management procedures.
- Verification using official vendor contact details.
- Documentation and approval of all banking changes.
- Regular employee awareness training on Vendor Impersonation attacks.

# Indicators of Compromise (IOCs)
- Unexpected request to change vendor bank details.
- Banking migration used as justification.
- Request to update payment records immediately.
- Attachment containing new banking information.
- Vendor impersonation.
- Payment Redirection Fraud attempt.
- Business Email Compromise (BEC).

# Lessons Learned
This investigation improved my understanding of **Vendor Impersonation** attacks and how attackers exploit trust between organizations and their suppliers to commit financial fraud. I learned that not all phishing attacks aim to steal credentials—some focus on manipulating business processes to redirect legitimate payments.
I also learned the importance of verifying changes to vendor banking information through **Out-of-Band (OOB) Verification**, implementing strong financial controls, and following formal approval procedures before updating payment records.

# Conclusion
This email was identified as a **Vendor Impersonation** attack and a form of **Business Email Compromise (BEC)**. Instead of requesting login credentials, the attacker attempts to manipulate the organization's payment process by convincing the finance department to replace legitimate bank account details with fraudulent ones.
Successful exploitation could result in **Payment Redirection Fraud**, causing continuous financial losses until the fraudulent bank details are identified and corrected. Independent verification and strong financial controls are essential to prevent this type of attack.

# Key Takeaway
Requests to change vendor bank account information should never be trusted based solely on an email. Organizations should always verify such requests through **Out-of-Band (OOB) Verification**, follow established financial approval procedures, and confirm changes using official vendor contact information before processing future payments.