# Email Analysis #6 – QR Code Phishing (Quishing) Attack

## Email Summary
This email is a **QR Code Phishing (Quishing)** attack that impersonates an organization's IT Security Team by requesting employees to re-register their Multi-Factor Authentication (MFA) as part of a quarterly security compliance review. Instead of using a malicious hyperlink, the attacker embeds a QR code that redirects victims to a fake Microsoft 365 login page. The primary objective of the attacker is to steal user credentials through **Credential Harvesting**, ultimately leading to **Account Takeover (ATO)** and **Initial Access** into the organization's environment.

## Email Details

**Sender:** security@company-microsoft365support.com

**Recipient:** employee@company.com

**Subject:** Action Required: Multi-Factor Authentication Reset

**Attack Type:** QR Code Phishing (Quishing)

## Email Objective
The objective of this attack is to convince employees to scan a malicious QR code and enter their Microsoft 365 credentials on a spoofed login page. By compromising the employee's account, the attacker gains **Initial Access** to corporate resources such as Outlook, Teams, OneDrive, SharePoint, and other Microsoft 365 services.

# Technical Analysis

## 1. Domain Verification

The sender's email address uses a **look-alike (spoofed) domain**, **company-microsoft365support.com**, instead of an official Microsoft or company domain.
Attackers commonly combine trusted keywords such as **Microsoft**, **365**, **Support**, and **Security** within a domain name to make it appear legitimate. Employees may quickly recognize familiar words without carefully verifying the registered domain.

## 2. Email Authenticity

The email begins with the generic greeting **"Hello"** instead of addressing the employee by name.
Legitimate organizations generally communicate security-related updates through official IT portals or internal communication platforms rather than requesting employees to scan QR codes received via email.

The email also states:
"If you have already completed the verification, please ignore this email."

This statement mimics legitimate corporate security notifications and is intended to increase the credibility of the email.

## 3. Subject Analysis
The subject line **"Action Required: Multi-Factor Authentication Reset"** immediately attracts the recipient's attention by suggesting that a mandatory security action must be completed.
The phrase **"Action Required"** creates urgency, while **"Multi-Factor Authentication Reset"** appears legitimate because MFA is a widely used organizational security measure.

## 4. QR Code Investigation
Unlike traditional phishing emails that contain malicious hyperlinks, this email hides the phishing website inside a QR code.
QR codes reduce suspicion because users cannot immediately inspect the destination URL before scanning. Many users instinctively trust QR codes and scan them without verifying where they lead.
After scanning, the victim is redirected to a fake Microsoft 365 login page designed to capture login credentials.

## 5. Why the Email Appears Legitimate
Several characteristics make this phishing email appear convincing.

- It claims to come from the IT Security Team.
- It refers to a quarterly security compliance review.
- It mentions Multi-Factor Authentication (MFA), a legitimate security control.
- It specifies a deadline of **6:00 PM**, making the request appear routine and scheduled.
- It includes the statement **"If you have already completed the verification, please ignore this email,"** which resembles genuine corporate security notifications.

## 6. Social Engineering Analysis
The attacker uses several social engineering techniques to manipulate the recipient.

- **Authority:** Pretends to represent the IT Security Team.
- **Urgency:** Requires completion before 6:00 PM.
- **Fear:** Warns that Microsoft 365 services may be suspended.
- **Compliance:** Uses the phrase "Quarterly Security Compliance Review" to make the request appear mandatory.
- **Trust:** Uses familiar Microsoft 365 services and security terminology.
- **Anxiety:** Encourages employees to act quickly to avoid losing access to business applications.

## 7. Attack Chain

Email Delivered
        ↓
Victim scans QR Code
        ↓
QR Code redirects to fake Microsoft 365 login page
        ↓
Victim enters Microsoft 365 credentials
        ↓
Credential Harvesting
        ↓
Attacker captures MFA verification code
        ↓
Account Takeover (ATO)
        ↓
Initial Access to the organization's environment

## 8. Risk Assessment

**Risk Rating:** Critical

This email is classified as **Critical** because it targets Microsoft 365 credentials, which often provide access to multiple corporate services.
If successful, the attacker may obtain:

- Unauthorized access to Outlook emails.
- Microsoft Teams conversations.
- OneDrive cloud storage.
- SharePoint documents.
- Company contacts.
- Calendar events.
- Internal confidential documents.
- Authentication tokens.
- Sensitive organizational information.

Compromising a single Microsoft 365 account can provide attackers with significant access to the organization's internal environment.

## 9. Possible Impact
A successful attack could result in:

- Credential Harvesting.
- Account Takeover (ATO).
- Initial Access into the corporate network.
- Unauthorized access to confidential emails.
- Exposure of sensitive company documents.
- Theft of intellectual property.
- Access to Teams conversations.
- Cloud data compromise.
- Identity theft.
- Further phishing attacks using the compromised account.

## 10. Incident Response
If this email is received, employees should:

- Do not scan the QR code.
- Verify the sender's email address carefully.
- Contact the IT Helpdesk using official communication channels.
- Confirm whether the MFA reset request is legitimate.
- Ask colleagues whether they received the same email.
- Report the email to the Information Security or SOC Team.
- Mark the email as phishing.
- Delete the email after reporting it.

If the QR code has already been scanned and credentials have been entered:

- Immediately change the Microsoft 365 password.
- Reset Multi-Factor Authentication (MFA).
- Sign out of all active sessions.
- Notify the IT Security Team.
- Review recent login activity for unauthorized access.

# Indicators of Compromise (IOCs)

- Look-alike sender domain (company-microsoft365support.com)
- Generic greeting ("Hello")
- Request to scan a QR code instead of using official portals
- Mandatory MFA reset request
- Urgent deadline (6:00 PM)
- Threat of Microsoft 365 service suspension
- Quarterly Security Compliance Review used as justification
- QR code redirecting to a fake login page
- Credential Harvesting attempt
- Social engineering through authority, urgency, compliance, and fear

# Lessons Learned

This investigation improved my understanding of **QR Code Phishing (Quishing)** attacks and how attackers exploit employee trust in QR codes and organizational security policies. I learned that attackers often replace malicious hyperlinks with QR codes because users are less likely to inspect the destination URL before scanning.
I also learned the importance of verifying MFA-related requests through official IT communication channels instead of scanning QR codes received via email. Organizations should educate employees about Quishing attacks, encourage verification through trusted sources, and reinforce awareness of social engineering techniques.

# Conclusion
This email was identified as a **QR Code Phishing (Quishing)** attack designed to steal Microsoft 365 credentials through **Credential Harvesting**. The attacker impersonates the IT Security Team and uses authority, urgency, compliance, and fear to convince employees to scan a malicious QR code.
Unlike traditional phishing emails that rely on visible hyperlinks, this attack conceals the malicious website within a QR code, making it more difficult for users to recognize the threat. Successful exploitation could result in **Account Takeover (ATO)** and provide the attacker with **Initial Access** to the organization's environment.

# Key Takeaway
QR codes should never be trusted solely because they appear in official-looking emails. Employees should always verify security-related requests through official IT communication channels and avoid scanning QR codes from unsolicited emails. Careful verification can prevent **Credential Harvesting**, **Account Takeover (ATO)**, and unauthorized access to organizational resources.