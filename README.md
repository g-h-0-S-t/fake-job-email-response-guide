# fake-job-email-response-guide

> A step-by-step guide on what to do when you receive a fake job offer email. From DFIR analysis to reporting across 17 agencies globally.

---

## What is DFIR?

**DFIR** stands for **Digital Forensics and Incident Response.**

In simple terms: examining digital evidence to figure out exactly what happened, who did it, and how.

---

## The Playbook

### STEP 1: DUMP IT INTO AN AI

Copy paste the entire email into any AI assistant, attach any documents that came with it, and say:

```
Do a DFIR analysis on this email and attachments and conclude whether it is a scam.
```

The AI will instantly identify fake domains, forged documents, legal violations, and the full attack chain.

---

### STEP 2: TRACE THE DOMAIN

Go to [whois.com/whois/[sender-domain]](https://www.whois.com) and look up the registrant.

You will get the real name, email, phone and registrar behind the fake domain in seconds.

Then ask the AI:

```
Analyse this WHOIS data and tell me what it reveals.
```

---

### STEP 3: FORWARD THE EMAIL

Ask the AI to generate a formal investigation report email.  
Also ask it:

```
Find the official legal/abuse contact email for [company being impersonated].
```

Then send it with the original email and all attachments.

| Field | Value |
|---|---|
| TO | Registrar abuse desk (found via WHOIS) |
| CC | The scammer (puts them on notice they have been identified) |
| BCC | Everyone below |

**BCC list:**

| Organization | Email |
|---|---|
| Real company legal team | Ask AI to find the official contact |
| APWG | reportphishing@apwg.org |
| CERT-In | incident@cert-in.org.in |
| US-CERT | phishing-report@us-cert.gov |
| Action Fraud UK | report@phishing.gov.uk |
| Cloudflare | abuse@cloudflare.com |
| Microsoft | phish@office365.microsoft.com |
| GoDaddy | abuse@godaddy.com |
| Namecheap | abuse@namecheap.com |

---

### STEP 4: HIT EVERY WEB FORM

Ask the AI to guide you through each one. It will fill every field for you.

| Organization | Link |
|---|---|
| FBI IC3 | [ic3.gov](https://www.ic3.gov) |
| FTC | [reportfraud.ftc.gov](https://reportfraud.ftc.gov) |
| ICANN | [icann.org/compliance/complaint](https://www.icann.org/compliance/complaint) |
| Google Safe Browsing | [safebrowsing.google.com/safebrowsing/report_phish](https://safebrowsing.google.com/safebrowsing/report_phish/) |
| Microsoft SmartScreen | [microsoft.com/en-us/wdsi/support/report-unsafe-site](https://www.microsoft.com/en-us/wdsi/support/report-unsafe-site) |
| Netcraft | [report.netcraft.com](https://report.netcraft.com/report) |
| Spamhaus | [submit.spamhaus.org](https://submit.spamhaus.org/submit/) |
| Interpol | [interpol.int/en/Contacts/Contact-INTERPOL](https://www.interpol.int/en/Contacts/Contact-INTERPOL) |
| Cloudflare Abuse | [cloudflare.com/abuse](https://www.cloudflare.com/abuse/) |
| Google Abuse | [support.google.com/mail/contact/abuse](https://support.google.com/mail/contact/abuse) |
| India Cybercrime | [cybercrime.gov.in](https://cybercrime.gov.in) |

---

## Result

**Total time:** One evening.  
**Result:** Domain blacklisted globally across Google, Microsoft, FBI, FTC, ICANN, Interpol and Spamhaus simultaneously.

---

## Red Flags to Look For

- Sender domain is slightly different from the real company
- Unsolicited email with no prior application
- Offers salary, housing, car and benefits before any interview
- Asks for passport scan or educational certificates upfront
- Asks you to pay a visa or processing fee (advance-fee fraud)
- Contract cites laws from a different country
- Employment form asks irrelevant personal questions (smoking, drinking, hobbies)
- WHOIS registrant address is fake or blank
- Domain registered days or weeks before the email arrived

---

## Contributing

Found a new reporting channel that works? Open a PR with the verified email or web form link.

## License

MIT

---

> Don't stay silent. Stay dangerous.
