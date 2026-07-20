# Email Analysis #2 – Microsoft 365 Password Expiry Phishing Email

## Email Summary
This email is a phishing attempt that impersonates the Microsoft Security Team. It claims that the recipient's Microsoft 365 account password will expire today and instructs the user to verify their account within two hours to avoid permanent suspension of email and Office services. The attacker includes a malicious verification link designed to trick the recipient into entering their Microsoft 365 credentials, potentially leading to unauthorized access to the account.

## Email Details

**Sender:** security@micr0soft365-support.com

**Recipient:** employee@company.com

**Subject:** Action Required: Your Microsoft 365 Password Expires Today

**Suspicious URL:** https://micr0soft365-support.com/verify

## Technical Analysis

### 1. Sender Analysis

The sender's email address does not belong to Microsoft's official domain. Microsoft uses the official domain **microsoft.com** for its emails. Instead, the sender uses a spoofed or look-alike domain, **security@micr0soft365-support.com**, to appear legitimate and deceive recipients.

The sender has used **typosquatting**, a technique in which attackers replace letters with similar-looking numbers or characters to create a domain that closely resembles a legitimate one. In this case, the letter **"o"** has been replaced with the number **"0"**, making the domain appear genuine at first glance while actually directing users to a malicious website.

### 2. Subject Analysis

The subject line, **"Action Required: Your Microsoft 365 Password Expires Today,"** is designed to create a sense of urgency and pressure the recipient into taking immediate action. By claiming that the password will expire **today**, the attacker attempts to make the recipient act impulsively without verifying the authenticity of the email. This tactic reduces the likelihood that the user will carefully examine the sender or the link before responding.

### 3. Greeting Analysis

The email starts with **"Dear Employee"** instead of addressing the recipient by their registered name. Legitimate organizations generally personalize important security-related communications by using the recipient's name. The use of a generic greeting indicates that the email may have been sent in bulk to multiple recipients, which is a common characteristic of phishing campaigns.

### 4. URL Analysis

The URL **https://micr0soft365-support.com/verify** does not belong to Microsoft's official domain. The legitimate Microsoft domain is **microsoft.com**, whereas this URL uses **micr0soft365-support.com**, which is a spoofed (look-alike) domain.

The attacker has used **typosquatting** by replacing the letter **"o"** with the number **"0"** to make the domain appear genuine. The additional words **"365-support"** are included to make the URL look more convincing. Users who do not carefully inspect the domain may mistake it for an official Microsoft website and disclose their login credentials.

### 5. Social Engineering Techniques

The attacker uses several social engineering techniques to manipulate the recipient into taking immediate action.

- **Urgency:** Claims that the password will expire today and requires action within two hours.
- **Fear:** Warns that the mailbox will be permanently suspended if no action is taken.
- **Authority:** Impersonates the Microsoft Security Team to appear trustworthy and legitimate.

These techniques are intended to pressure the recipient into clicking the malicious link without verifying the authenticity of the email.

## Possible Impact

If the employee enters their Microsoft 365 credentials through the malicious link, the attacker can steal the username, password, and potentially the MFA code. The attacker can then gain unauthorized access to the employee's Microsoft 365 account.

Once inside the account, the attacker may:
- Access company emails and confidential documents.
- Read, download, or modify sensitive files stored in OneDrive or SharePoint.
- Access Microsoft Teams conversations and shared data.
- Send phishing emails from the employee's account to other employees or clients.
- Reset account settings or passwords (depending on the permissions available).
- Use the compromised account to move laterally within the organization's network, potentially leading to a larger security breach.

## Risk Assessment

**Risk Rating:** Critical

This email is classified as **Critical** because it attempts to steal Microsoft 365 credentials through a phishing link. If an employee clicks the link and enters their login credentials, the attacker could gain unauthorized access to the organization's Microsoft 365 environment.

A successful attack could result in the compromise of company emails, confidential documents, Microsoft Teams data, and other business resources. The attacker may also misuse the compromised account to launch further phishing attacks, steal sensitive information, or disrupt business operations, making the overall risk critical.

## Recommended Actions

- Do not click on any links or open any attachments contained in the email.
- Do not enter your Microsoft 365 credentials on the linked website.
- Report the email to the organization's Security Team or IT department for investigation.
- Mark the email as **Phishing** or **Spam** in the email client.
- Delete the email after it has been reported.
- If credentials have already been entered, immediately change the password, revoke active sessions if possible, and notify the Security Team.

## Indicators of Compromise (IOCs)

- Unofficial sender email: `security@micr0soft365-support.com`
- Suspicious verification URL: `https://micr0soft365-support.com/verify`
- Spoofed (look-alike) domain: `micr0soft365-support.com`
- Typosquatting (the letter "o" replaced with the number "0")
- Generic greeting ("Dear Employee") instead of the recipient's name
- Urgent subject line requesting immediate action
- Threat of permanent mailbox suspension
- Request to verify Microsoft 365 credentials through an external link

## Lessons Learned

This analysis reinforced the importance of carefully examining the sender's email address, domain name, and embedded URLs before responding to any security-related email. I learned that attackers often use social engineering techniques such as urgency, fear, and authority to manipulate users into revealing sensitive information. I also learned how to identify typosquatting, spoofed domains, and other common phishing indicators that can help prevent credential theft and unauthorized access.

## Conclusion

This email was identified as a phishing attempt designed to steal Microsoft 365 credentials by impersonating the Microsoft Security Team. Multiple phishing indicators, including a spoofed domain, typosquatting, urgent language, a generic greeting, and a malicious verification link, confirmed that the email was not legitimate. Users should always verify the sender, inspect URLs carefully, and report suspicious emails to the Security Team before taking any action.