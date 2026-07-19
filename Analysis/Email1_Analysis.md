# Email Analysis #1 – SBI Banking Phishing Email

# Email Summary

A phishing email impersonating the State Bank of India (SBI) attempts to trick users into believing that their online banking account has been suspended due to suspicious activity. The attacker urges the victim to verify their account through a malicious link.

# Email Details

**Sender**
support@sbi-securityverify.com
**Subject**
URGENT: Your SBI Account Has Been Suspended
**Suspicious URL**
https://sbi-securityverify.com/login

# Technical Analysis

# 1. Sender Analysis
The sender's email address does not belong to SBI's official domain. Instead, it uses a look-alike domain (`sbi-securityverify.com`) to appear legitimate and deceive recipients.

**Finding:** Suspicious

# 2. Subject Analysis
The subject line creates urgency by claiming the account has been suspended. This encourages victims to act without verifying the legitimacy of the email.

**Finding:** High Risk

# 3. Greeting Analysis
The email starts with **"Dear Customer"** instead of addressing the recipient by their registered name. Legitimate banks generally personalize their communications.

**Finding:** Suspicious

# 4. URL Analysis
The provided URL does not belong to SBI's official website. It is designed to imitate the bank and trick users into entering their login credentials.

**Finding:** Malicious URL

# 5. Social Engineering Techniques
The attacker uses:
- Fear
- Urgency
- Authority
- Trust in a well-known organization

# 6. Possible Impact
If the victim enters their credentials, the attacker could:
- Steal login credentials
- Perform unauthorized banking transactions
- Commit identity theft
- Access personal information
- Cause financial loss

# 7. Risk Assessment
**Risk Level:**  Critical
**Reason:**
The phishing email targets banking credentials, which could result in severe financial loss and compromise sensitive personal information.

# 8. Recommended Actions
- Do not click the link.
- Do not enter any credentials.
- Report the email to the security team.
- Mark it as phishing/spam.
- Delete the email.
- Verify account status using the official SBI website or mobile application.

# Indicators of Compromise (IOCs)
During the analysis, the following Indicators of Compromise (IOCs) were identified:
- Unofficial sender domain: `sbi-securityverify.com`
- Suspicious login URL directing users to a fake banking website
- Generic greeting used instead of the customer's registered name
- Urgent language designed to pressure immediate action
- Request to verify banking credentials through an embedded link

# Lessons Learned
- Always verify the sender's domain.
- Never trust urgent banking emails without verification.
- Check URLs carefully before clicking.
- Banks rarely ask customers to verify accounts through email links.

# Conclusion
This email is a phishing attempt that uses impersonation, urgency, and fear to trick victims into revealing sensitive banking credentials. Users should always verify suspicious emails through official communication channels before taking any action.