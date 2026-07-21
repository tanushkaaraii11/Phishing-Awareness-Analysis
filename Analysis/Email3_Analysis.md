# Email Analysis #3 – Amazon's Package Delivery Phishing Email

## Email Summary

This email is a phishing attempt that impersonates Amazon's Delivery Team by claiming that the recipient's package could not be delivered due to an incorrect delivery address. The email instructs the recipient to confirm their delivery details within 12 hours using a verification link. By creating a sense of urgency and concern, the attacker attempts to trick the recipient into revealing their Amazon account credentials through a spoofed website.

## Email Details

**Sender:** delivery@amazon-packagecenter.com

**Recipient:** customer@email.com

**Subject:** Your Amazon Package Could Not Be Delivered

**Suspicious URL:** https://amazon-packagecenter.com/confirm-delivery

## Email Objective

The primary objective of this phishing email is to trick the recipient into visiting a spoofed Amazon website and entering their account credentials. By exploiting concerns about an undelivered package, the attacker attempts to gain unauthorized access to the victim's Amazon account, which may contain personal information, saved payment methods, delivery addresses, and order history.

## Technical Analysis

### 1. Domain Verification

The sender's email address does not belong to Amazon's official domain. Amazon uses the official domain **amazon.com** for its services and email communications. Instead, the sender uses a spoofed (look-alike) domain, **delivery@amazon-packagecenter.com**, to appear legitimate and deceive recipients.
The domain is designed to imitate Amazon's branding and trick users into believing the email is genuine.

### 2. Email Authenticity

Legitimate courier or e-commerce companies generally contact customers through official channels such as the Amazon app, SMS, or registered customer support rather than asking users to verify delivery information through an external website.
The email also begins with the generic greeting **"Dear Customer"** instead of addressing the recipient by name. While generic greetings alone do not confirm phishing, they are commonly found in mass phishing campaigns where attackers do not know the recipient's identity.

### 3. Subject Analysis

The subject line **"Your Amazon Package Could Not Be Delivered"** is designed to immediately attract the recipient's attention. Since many users regularly receive Amazon deliveries, the attacker exploits curiosity and concern to encourage the recipient to open the email without questioning its legitimacy.

### 4. URL Investigation
The URL **https://amazon-packagecenter.com/confirm-delivery** does not belong to Amazon's official domain and instead uses a spoofed domain designed to impersonate Amazon.
The email also describes the URL as a **"secure link."** Legitimate companies rarely emphasize that a link is "secure" within the email itself. Attackers often use reassuring phrases such as **"secure link," "official portal,"** or **"verified website"** to increase the recipient's trust and encourage them to click the malicious link.

### 5. Social Engineering Analysis

The attacker uses multiple social engineering techniques to manipulate the recipient.

- **Authority:** Pretends to represent Amazon Delivery Team.
- **Curiosity:** Claims the package could not be delivered, encouraging the user to check what happened.
- **Urgency:** Gives only 12 hours to confirm delivery details.
- **Fear:** Warns that the package will be returned.
- **Financial Pressure:** States that additional delivery charges may apply if no action is taken.

### 6. Risk Assessment
**Risk Rating:** Critical

This email is classified as **Critical** because it attempts to steal Amazon account credentials through a phishing link. If the victim enters their login credentials, the attacker could gain unauthorized access to the Amazon account.
A successful compromise may allow the attacker to place unauthorized orders, access saved payment methods, view personal addresses and phone numbers, reset account credentials, commit financial fraud, and misuse the victim's personal information for future phishing or identity theft attacks.

### 7. Possible Impact

A successful phishing attack could allow the attacker to gain unauthorized access to the victim's Amazon account. The attacker may:

- Reset the account password.
- View personal information.
- Access saved payment methods.
- View delivery addresses and phone numbers.
- Review shopping history and purchasing habits.
- Place unauthorized orders.
- Use the stolen information for identity theft or future phishing attacks.

### 8. Incident Response
If this email is received, the user should:

- Do not click on the embedded link.
- Do not enter account credentials.
- Verify delivery status directly through the Amazon app or official website.
- Contact Amazon Customer Support through official channels if necessary.
- Report the email as phishing or spam.
- Delete the email after reporting it.

## Indicators of Compromise (IOCs)

- Unofficial sender email: `delivery@amazon-packagecenter.com`
- Spoofed domain: `amazon-packagecenter.com`
- Suspicious verification URL: `https://amazon-packagecenter.com/confirm-delivery`
- Generic greeting ("Dear Customer") instead of the recipient's name
- Subject line designed to attract immediate attention ("Your Amazon Package Could Not Be Delivered")
- Request to verify delivery details through an external website
- Urgent deadline of **12 hours** to create pressure
- Threat of package return and additional delivery charges
- Use of reassuring language such as **"secure link"** to increase trust

## Lessons Learned

This investigation improved my understanding of how attackers exploit everyday situations such as online shopping and package deliveries, to conduct phishing attacks. I learned that legitimate companies should be verified through their official domains and communication channels rather than links provided in unsolicited emails. This analysis also reinforced the importance of checking sender domains, URLs, greetings, and social engineering techniques before taking any action on suspicious emails.

## Conclusion

This email was identified as a phishing attempt designed to impersonate Amazon's Delivery Team and steal the recipient's account credentials. Multiple phishing indicators, including a spoofed sender domain, suspicious URL, generic greeting, misleading subject line, and the use of urgency and fear, confirmed that the email was malicious. Users should always verify delivery-related issues through Amazon's official website or mobile application and avoid interacting with links provided in unsolicited emails.

## Key Takeaway

Always verify delivery-related notifications through the official Amazon website or mobile application instead of clicking links in unsolicited emails. Carefully inspecting the sender's domain and embedded URLs can prevent credential theft and account compromise. 