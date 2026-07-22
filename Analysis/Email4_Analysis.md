# Email Analysis #4 – LinkedIn Security Alert Phishing Email

## Email Summary

This email is a phishing attempt that impersonates LinkedIn's Trust & Safety Team by claiming that a new sign-in was detected on the recipient's account from an unrecognized device. The email attempts to create concern by providing a login location and time while urging the recipient to verify their identity through an embedded link. The attacker aims to steal the victim's LinkedIn credentials using a spoofed website.

## Email Details

**Sender:** security@linkedin-accountsupport.com

**Recipient:** user@email.com

**Subject:** New Sign-in Detected on Your LinkedIn Account

**Suspicious URL:** https://linkedin-accountsupport.com/verify

## Email Objective

The primary objective of this phishing email is to trick the recipient into visiting a fake LinkedIn login page and entering their account credentials. This is a **credential harvesting** attack that uses **brand impersonation** and a **look-alike/typosquatted domain** to deceive users. Once the credentials are stolen, the attacker can gain unauthorized access to the victim's LinkedIn account, allowing them to misuse professional connections, personal information, recruiter conversations, and other sensitive account data.

# Technical Analysis

## 1. Domain Verification

The sender's email address does not belong to LinkedIn's official domain. LinkedIn uses the official domain **linkedin.com** for its services and email communications. Instead, the sender uses a spoofed or look-alike domain, **security@linkedin-accountsupport.com**, to imitate LinkedIn and deceive recipients.

The additional words **"accountsupport"** make the email appear legitimate at first glance, but the registered domain is not owned by LinkedIn. This technique is known as **brand impersonation** using a **look-alike (typosquatted) domain**.

## 2. Email Authenticity

Legitimate security notifications from LinkedIn generally direct users to review account activity through the official LinkedIn website or mobile application instead of asking them to verify their identity through an external website.

The email also begins with the generic greeting **"Hello"** instead of addressing the recipient by name. While generic greetings alone do not confirm phishing, they are commonly used in mass phishing campaigns where attackers do not know the recipient's identity.

## 3. Subject Analysis

The subject line **"New Sign-in Detected on Your LinkedIn Account"** is designed to immediately capture the recipient's attention by creating concern about account security. It encourages the recipient to open the email quickly and react without carefully verifying its authenticity.

## 4. URL Investigation

The URL **https://linkedin-accountsupport.com/verify** does not belong to LinkedIn's official domain and instead uses a spoofed domain designed to imitate LinkedIn.

The email asks the recipient to verify their identity using the embedded link. Legitimate companies typically encourage users to access their accounts through their official website or mobile application rather than clicking links contained in unsolicited emails.

## 5. Why the Email Appears Legitimate

Several elements make this phishing email appear convincing:

- It provides a login location (Singapore), similar to genuine security notifications.
- It includes the exact login time, making the alert appear authentic.
- It uses the name **"LinkedIn Trust & Safety Team,"** which resembles an official LinkedIn department.
- The overall format closely resembles security alerts sent by legitimate platforms such as Google, Microsoft, and Meta.
- It states, **"If this was you, no further action is required,"** which makes the email appear balanced and trustworthy before asking the recipient to take action.

## 6. Social Engineering Analysis
The attacker uses multiple social engineering techniques to manipulate the recipient.

- **Authority:** Pretends to represent LinkedIn's Trust & Safety Team.
- **Fear:** Warns about an unauthorized sign-in and possible account restrictions.
- **Urgency:** Requests account verification within 24 hours.
- **Concern:** Creates anxiety by suggesting that someone may have accessed the account.
- **Trust Building:** Uses realistic security notification language to lower the recipient's suspicion.

## 7. Risk Assessment

**Risk Rating:** Critical

This email is classified as **Critical** because it attempts to steal LinkedIn account credentials through a phishing website. If successful, the attacker may gain unauthorized access to the victim's professional profile, recruiter conversations, personal messages, uploaded resumes, work history, and professional network.

A successful **Account Takeover (ATO)** may allow the attacker to impersonate the victim, distribute phishing messages to trusted connections, conduct identity theft, misuse professional relationships, and damage the victim's professional reputation.

## 8. Possible Impact
A successful phishing attack could allow the attacker to:

- Gain unauthorized access to the LinkedIn account.
- Reset the account password.
- Access personal profile information.
- Read private messages and recruiter conversations.
- View professional contacts and network connections.
- Download uploaded resumes and employment information.
- Send fraudulent messages while impersonating the victim.
- Modify or delete profile information.
- Damage the victim's professional reputation.
- Launch further phishing attacks using the victim's trusted profile.

## 9. Incident Response
If this email is received, the user should:

- Do not click on the embedded link.
- Do not enter account credentials.
- Verify account activity through the official LinkedIn website or mobile application.
- Check the sender's email address carefully.
- Report the email as phishing or spam.
- Delete the email after reporting it.

If credentials have already been entered:

- Change the LinkedIn password immediately.
- Sign out of all active sessions.
- Enable Multi-Factor Authentication (MFA).
- Review recent account activity for unauthorized changes.

# Indicators of Compromise (IOCs)

- Unofficial sender email: `security@linkedin-accountsupport.com`
- Spoofed (look-alike) domain: `linkedin-accountsupport.com`
- Suspicious verification URL: `https://linkedin-accountsupport.com/verify`
- Generic greeting -"Hello"
- Unexpected login notification from an unrecognized location
- Urgent request to verify identity within 24 hours
- Threat of temporary account restrictions
- Embedded verification link instead of directing users to the official LinkedIn website
- Use of a trusted department name - "LinkedIn Trust & Safety Team"
- Credential harvesting attempt through a spoofed login page

# Lessons Learned

This investigation improved my understanding of how attackers imitate legitimate security alerts to steal user credentials. I learned that phishing emails often combine realistic details, such as login locations, timestamps, and trusted department names, with spoofed domains and social engineering techniques to appear convincing.
This analysis reinforced the importance of verifying sender domains, avoiding embedded links in unsolicited emails, and accessing accounts only through official websites or mobile applications. I also learned how attackers use **brand impersonation**, **look-alike (typosquatted) domains**, and **credential harvesting** techniques to perform **Account Takeover (ATO)** attacks.

# Conclusion

This email was identified as a phishing attempt that impersonates LinkedIn's Trust & Safety Team to steal user credentials. Although the email contains realistic elements such as a login location, timestamp, and official-looking department name, multiple phishing indicators—including a spoofed sender domain, fake verification URL, generic greeting, and urgency—confirm that the email is malicious.
The attacker uses brand impersonation, social engineering, and credential harvesting techniques to gain unauthorized access to the victim's LinkedIn account. Users should always verify security alerts directly through LinkedIn's official website or mobile application rather than interacting with links provided in unsolicited emails.

# Key Takeaway

Always verify account security notifications through the official LinkedIn website or mobile application instead of clicking links in unsolicited emails. Carefully inspecting the sender's domain, embedded URLs, and communication method can help prevent credential theft and **Account Takeover (ATO)** attacks. Even realistic-looking security alerts should be treated with caution until their authenticity has been verified. 