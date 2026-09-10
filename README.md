# Awesome-Email-Verification-API

# ✉️ Top Email Verification APIs



> A curated list of **Email Verification APIs** and open-source alternatives for validating email addresses, detecting invalid and disposable addresses, checking MX/DNS records, performing SMTP verification, identifying catch-all domains, detecting role-based addresses, correcting typos, and improving email deliverability.



Email Verification APIs help businesses determine whether an email address is likely to be **deliverable, invalid, risky, disposable, temporary, role-based, catch-all, spam-trap or otherwise problematic** without sending an actual email.



This repository focuses primarily on **open-source alternatives** that can be self-hosted and used to build an alternative to commercial email verification services.



---



## 📑 Table of Contents



* [☁️ SaaS/Hosted Platforms](#️-saashosted-platforms)

* [🌍 Open-Source](#-open-source)

* [📧 Open-Source Email Verification Engines](#-open-source-email-verification-engines)

* [🌐 Open-Source DNS & MX Verification](#-open-source-dns--mx-verification)

* [📡 Open-Source SMTP Verification](#-open-source-smtp-verification)

* [🗑️ Open-Source Disposable Email Detection](#️-open-source-disposable-email-detection)

* [👤 Open-Source Role-Based Email Detection](#-open-source-role-based-email-detection)

* [🔤 Open-Source Email Syntax Validation](#-open-source-email-syntax-validation)

* [🧠 Open-Source Email Intelligence & Enrichment](#-open-source-email-intelligence--enrichment)

* [⚡ Open-Source Email Verification APIs](#-open-source-email-verification-apis)

* [📊 Open-Source Bulk Email Verification](#-open-source-bulk-email-verification)

* [🏗️ Email Verification Architecture](#️-email-verification-architecture)

* [🔄 Open-Source Email Verification Architecture](#-open-source-email-verification-architecture)

* [🧩 Commercial Platform → Open-Source Equivalent](#-commercial-platform--open-source-equivalent)

* [⚖️ Commercial vs Open-Source](#️-commercial-vs-open-source)

* [🚀 Recommended Open-Source Stacks](#-recommended-open-source-stacks)

* [🔬 Email Verification Pipeline](#-email-verification-pipeline)

* [🎯 Verification Result Classification](#-verification-result-classification)

* [🔐 Enterprise Email Verification Architecture](#-enterprise-email-verification-architecture)

* [🌐 Open-Source Email Verification Landscape](#-open-source-email-verification-landscape)

* [🤝 Contributing](#-contributing)

* [⚠️ Disclaimer](#️-disclaimer)



---



# ☁️ SaaS/Hosted Platforms



Commercial Email Verification APIs provide managed validation infrastructure, DNS/MX checks, SMTP verification, disposable-email detection, catch-all detection, spam-trap detection, bulk validation and integrations.



> 📊 **Market Overview:** The global email verification and deliverability software market is estimated at **$710M – $790M** (expanding to **~$2.8B** when including broader email security & deliverability infrastructure), growing at a **CAGR of ~9.8%** toward **$1.1B – $6.4B by 2030–2034**. The sector is **moderately to highly fragmented** rather than a winner-take-all market, featuring enterprise consolidation (e.g., ZoomInfo, Validity, SparkPost/Bird) alongside dozens of profitable independent niche verifiers and specialized API vendors.

| Platform | Company | Company Size (Rev / Valuation) | Primary Focus | Pricing | Free Tier Limit | Key Capabilities |
| -------------------------------------------------------------------------------------------- | ---------------------- | ------------------------------------- | --------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------- |
| [NeverBounce](https://neverbounce.com/) | ZoomInfo | ~$1.2B Rev / ~$1.2B Market Cap (NASDAQ: ZI) | Email Verification | Starts at $8 for 1,000 credits ($0.008/email Pay-as-you-go) or $49/mo (sync) | 10 free credits upon signup (One-time trial) + free list analysis | Real-time API, bulk verification, list cleaning, disposable detection, validation |
| [MailboxValidator](https://www.mailboxvalidator.com/) | SparkPost / Bird | ~$600M Acq. Valuation / Bird ~$500M Rev | Email Verification | Starts at $19.95 for 1,000 credits (Bulk) or $9.95/mo for 1,000 queries/mo (API) | 300 queries/month (Free forever API plan) or 100 credits free trial | Syntax, MX, SMTP, disposable, free-provider and domain validation |
| [BriteVerify](https://www.validity.com/products/briteverify/) | Validity | ~$62M – $70M ARR / ~$300M+ Valuation | Email Verification & Data Quality | Starts at $40 for 5,000 verifications ($0.008/verification Pay-as-you-go) | 1,000 free credits for 30-day trial (via DemandTools trial) or sales demo | Real-time and bulk verification, data quality and deliverability |
| [Mailboxlayer](https://mailboxlayer.com/) | apilayer / Idera | ~$15M ARR (Parent Idera ~$3B+ Valuation) | Email Validation API | Starts at $14.99/mo for Basic (5,000 requests/month) | 100 requests/month (Free forever plan) | Syntax, MX, SMTP, disposable, role and free-provider detection |
| [ZeroBounce](https://www.zerobounce.net/) | ZeroBounce | ~$10M – $25M ARR (Inc. 5000) | Email Validation & Deliverability | Starts at $39 for 2,000 credits (Pay-as-you-go) or $99/mo (10,000 credits/mo) | 100 credits/month (Free forever, refreshes monthly) | Real-time/bulk validation, SMTP checks, spam-trap detection, disposable detection, catch-all, scoring |
| [Hunter Email Verifier](https://hunter.io/email-verifier) | Hunter | ~$8M – $10M ARR (Bootstrapped) | Email Verification | Starts at $49/mo (or $34/mo billed annually) for 2,000 credits/mo | 50 credits/month (Free forever, up to 100 email verifications/mo) | Email verification API, syntax, domain, SMTP and deliverability checks |
| [Bouncer](https://usebouncer.com/) | Bouncer | ~$7.5M ARR | Email Verification | Starts at $8 for 1,000 credits ($0.008/email Pay-as-you-go) or $24/mo | 100 free credits upon signup (One-time trial, no credit card required) | Real-time/bulk verification, deliverability, toxicity detection, disposable detection |
| [Clearout](https://clearout.io/) | Clearout | ~$5M ARR | Email Verification | Starts at $21 for 3,000 credits (Pay-as-you-go) or $19.50/mo (3,000 credits/mo) | 100 free credits upon signup (One-time trial, credits never expire) | Real-time/bulk validation, catch-all, disposable, spam-trap and role detection |
| [Kickbox](https://kickbox.com/) | Kickbox | ~$2.3M – $5M ARR | Email Verification | Starts at $5 for 500 credits ($0.01/email) or $10 for 1,000 credits | 100 free credits upon signup (One-time trial) | API, bulk verification, deliverability, risk analysis, integrations |
| [Emailable](https://emailable.com/) | Emailable | ~$1.9M ARR (Cache Ventures) | Email Verification | Starts at $38 for 5,000 credits (Pay-as-you-go) or $32.30/mo | 250 free credits upon signup (One-time trial, credits never expire) | Real-time API, bulk verification, syntax/DNS/SMTP checks, risk analysis |
| [Abstract Email Verification](https://www.abstractapi.com/email-verification-validation-api) | Abstract API | ~$1.5M – $3M ARR | Email Validation API | Starts at $19/mo (or $9/mo billed annually) for 10,000 requests/mo | 100 requests/month (Free forever, 3 req/sec rate limit) | Syntax, MX, SMTP, disposable, free-provider and quality checks |
| [QuickEmailVerification](https://quickemailverification.com/) | QuickEmailVerification | ~$1M – $2.5M ARR | Email Verification | Starts at $4.00 for 500 credits ($0.008/email Pay-as-you-go) | 100 credits/day (~3,000 credits/month, Free forever, resets daily) | API, bulk validation, SMTP verification, disposable detection |
| [Verifalia](https://verifalia.com/) | Verifalia | ~$1M – $2M ARR | Email Validation | Starts at $9/mo for Starter (250 credits/day) or $7.90 for 1,000 credits | 25 credits/day (~750 credits/month, Free forever, resets daily) | Real-time and bulk verification, syntax/DNS/SMTP, disposable and catch-all detection |
| [EmailListVerify](https://emaillistverify.com/) | EmailListVerify | ~$1M – $2M ARR | Email Verification | Starts at $5 for 1,000 credits ($0.005/email Pay-as-you-go) or $139/mo | 100 free credits upon signup (One-time trial) | Bulk list cleaning, API, SMTP, disposable and catch-all detection |
| [Xverify](https://www.xverify.com/) | Xverify | ~$1M – $2M ARR | Contact Validation | Starts at $5 for 500 verifications ($0.01/verification Pay-as-you-go) | 100 free credits upon signup (One-time trial) + 5 checks/day on website | Email, phone and postal validation |
| [DeBounce](https://debounce.io/) | DeBounce | ~$800K – $1.5M ARR | Email Validation | Starts at $10 for 5,000 credits ($0.002/email Pay-as-you-go) | 100 free credits upon signup (One-time trial, no credit card required) | Bulk validation, API, SMTP checks, disposable detection, catch-all detection |
| [EmailOversight](https://www.emailoversight.com/) | EmailOversight | ~$500K – $1M ARR | Email Hygiene | Starts at $70/mo for up to 10,000 verifications/month | 200 free credits upon signup (Trial plan, active until credits exhausted) | Verification, suppression and list cleaning |
| [MillionVerifier](https://www.millionverifier.com/) | MillionVerifier | ~$440K – $1M ARR | Bulk Email Verification | Starts at $39 for 10,000 credits (Pay-as-you-go; promo $4.90 for 2,000) | 100 free credits upon signup (up to 500 for business email, one-time trial) | Bulk validation, API, SMTP and deliverability checks |
| [Captain Verify](https://captainverify.com/) | Captain Verify | ~$400K – $800K ARR | Email Verification | Starts at €7 (~$7.60) for 1,000 credits (Pay-as-you-go) | 100 free credits upon signup (One-time trial) + 3 checks/day on website | Bulk and real-time verification |
| [Proofy](https://proofy.io/) | Proofy | ~$300K – $600K ARR | Email Verification | Starts at $5 for 5,000 credits (Starter package Pay-as-you-go) | 100 free credits upon registration (One-time trial) + free web checker | Bulk verification, API, SMTP, disposable and catch-all detection |



> **Note:** Commercial providers use different verification methodologies. A service returning `valid`, `deliverable`, or `safe` does not guarantee that a message will ultimately be delivered.



---



# 🌍 Open-Source



Unlike commercial providers, open-source email verification generally works by combining several independent checks:



```text

Email Address

     │

     ├── Syntax

     │

     ├── Domain

     │

     ├── DNS / MX

     │

     ├── Disposable Domain

     │

     ├── Role Account

     │

     ├── Free Provider

     │

     ├── SMTP

     │

     ├── Catch-All

     │

     └── Risk Signals

              │

              ▼

       Verification Result

```



The strongest open-source implementations therefore tend to be **composable systems rather than a single ZeroBounce-like project**.



---



# 📧 Open-Source Email Verification Engines



| Project                                                                                                 | License     | Description                                                                                                               |

| ------------------------------------------------------------------------------------------------------- | ----------- | ------------------------------------------------------------------------------------------------------------------------- |

| [AfterShip Email Verifier](https://github.com/AfterShip/email-verifier)                                 | MIT         | Go email verification library with syntax, DNS, MX, SMTP, catch-all, disposable and role checks                           |

| [Visulima Email Verifier](https://github.com/visulima/visulima/tree/main/packages/email/email-verifier) | MIT         | Comprehensive TypeScript email verification and enrichment library with DNS/SMTP, disposable, role and provider detection |

| [Email Verifier](https://github.com/yolodex-ai/email-verifier)                                          | MIT         | Node.js verifier using syntax, DNS, MX, SMTP probing, catch-all and provider detection                                    |

| [Python Email Validator](https://github.com/JoshData/python-email-validator)                            | Unlicense   | Robust Python email syntax and deliverability validation library                                                          |

| [Email Validator](https://github.com/sagnik11/email-checker)                                            | Open Source | TypeScript validator with syntax, DNS, SMTP, disposable and B2C detection                                                 |

| [UnlimitedVerifier](https://github.com/unlimitedverifier/free-email-verifier)                           | MIT         | Lightweight Python email verifier using syntax, MX and SMTP validation                                                    |

| [Email Verification Tool](https://github.com/SyedSamrozeAli/Email-Verification-Tool)                    | Open Source | Local CSV email verification application using MX, SMTP and syntax checks                                                 |

| [email-verifier](https://github.com/AfterShip/email-verifier)                                           | MIT         | Go-based email verification library and self-hosted API reference                                                         |



---



# 🌐 Open-Source DNS & MX Verification



DNS/MX verification determines whether a domain is configured to receive email.



| Project                                                                 | Language | Description                                                    |

| ----------------------------------------------------------------------- | -------- | -------------------------------------------------------------- |

| [dnspython](https://github.com/rthalley/dnspython)                      | Python   | DNS toolkit supporting MX, A, AAAA, TXT and other record types |

| [miekg/dns](https://github.com/miekg/dns)                               | Go       | Full-featured DNS library                                      |

| [Trust-DNS / Hickory DNS](https://github.com/hickory-dns/hickory-dns)   | Rust     | DNS client and server implementation                           |

| [c-ares](https://github.com/c-ares/c-ares)                              | C        | Asynchronous DNS resolution library                            |

| [getdns](https://getdnsapi.net/)                                        | C        | Modern DNS API and resolver library                            |

| [Email Validator](https://github.com/JoshData/python-email-validator)   | Python   | Performs optional DNS MX validation                            |

| [AfterShip Email Verifier](https://github.com/AfterShip/email-verifier) | Go       | Includes MX and DNS validation                                 |



### MX Verification



```text

user@example.com

       │

       ▼

   Extract Domain

       │

       ▼

   example.com

       │

       ▼

    DNS Query

       │

       ▼

    MX Records?

      /      \

    YES       NO

     │         │

     ▼         ▼

Continue    A/AAAA fallback

```



A domain without a usable mail-exchange configuration is generally a strong signal that an address cannot receive normal email.



---



# 📡 Open-Source SMTP Verification



SMTP verification attempts to determine whether a receiving mail server will accept a recipient address without actually sending a message.



| Project                                                                                                 | Language   | Description                                              |

| ------------------------------------------------------------------------------------------------------- | ---------- | -------------------------------------------------------- |

| [AfterShip Email Verifier](https://github.com/AfterShip/email-verifier)                                 | Go         | SMTP verification with catch-all detection               |

| [Visulima Email Verifier](https://github.com/visulima/visulima/tree/main/packages/email/email-verifier) | TypeScript | SMTP probing with greylisting and mailbox-state handling |

| [Email Verifier](https://github.com/yolodex-ai/email-verifier)                                          | Node.js    | SMTP RCPT probing and catch-all detection                |

| [Email Validator](https://github.com/sagnik11/email-checker)                                            | TypeScript | Live SMTP handshakes                                     |

| [UnlimitedVerifier](https://github.com/unlimitedverifier/free-email-verifier)                           | Python     | SMTP verification without sending an email               |

| [Email Verification Tool](https://github.com/SyedSamrozeAli/Email-Verification-Tool)                    | Python     | Bulk SMTP verification                                   |



### SMTP Verification



```text

Client

  │

  │ EHLO

  ▼

Mail Server

  │

  │ MAIL FROM

  ▼

Mail Server

  │

  │ RCPT TO:<user@example.com>

  ▼

 ┌─────────────────────┐

 │ SMTP Response       │

 ├─────────────────────┤

 │ 2xx → accepted      │

 │ 4xx → temporary     │

 │ 5xx → rejected      │

 └─────────────────────┘

```



> **Important:** SMTP verification is inherently imperfect. Greylisting, anti-enumeration systems, catch-all servers, firewalls, tarpits and temporary failures can make an address appear `unknown` even when it is valid.



---



# 🗑️ Open-Source Disposable Email Detection



Disposable/temporary email addresses are frequently used for short-lived registrations, trials, abuse and spam.



| Project                                                                                             | License      | Description                                                           |

| --------------------------------------------------------------------------------------------------- | ------------ | --------------------------------------------------------------------- |

| [disposable-email-domains](https://github.com/disposable-email-domains/disposable-email-domains)    | CC0-1.0      | Large community-maintained disposable email domain blocklist          |

| [disposable](https://github.com/disposable/disposable)                                              | MIT          | Disposable/temporary email domain database with automated updates     |

| [disposable-email-domains](https://github.com/disposable/disposable-email-domains)                  | MIT          | Daily-updated disposable-domain dataset                               |

| [email-disposable](https://github.com/gtkppr/email-disposable)                                      | MIT          | Regularly updated disposable email domain list and JavaScript library |

| [burner-email-providers](https://github.com/wesbos/burner-email-providers)                          | MIT          | List of burner/disposable email providers                             |

| [fakefilter](https://github.com/7c/fakefilter)                                                      | BSD-3-Clause | Disposable email domain filtering                                     |

| [Propaganistas Laravel Disposable Email](https://github.com/Propaganistas/Laravel-Disposable-Email) | MIT          | Disposable email validation for Laravel                               |

| [Temporary Email Domain List](https://github.com/TempMailDetector/Temporary-Email-Domain-Blocklist) | Open Source  | Temporary/disposable email domain blocklist                           |



A disposable-domain check is generally much cheaper than an SMTP verification and should therefore be performed early in a verification pipeline.



---



# 👤 Open-Source Role-Based Email Detection



Role addresses represent functional accounts rather than individual recipients.



Common examples:



```text

admin@

support@

sales@

info@

contact@

billing@

hello@

marketing@

security@

webmaster@

postmaster@

```



| Project                                                                                                 | Description                                                 |

| ------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |

| [Visulima Email Verifier](https://github.com/visulima/visulima/tree/main/packages/email/email-verifier) | Detects role-based and no-reply addresses                   |

| [AfterShip Email Verifier](https://github.com/AfterShip/email-verifier)                                 | Role-account detection                                      |

| [disposable-email-domains](https://github.com/disposable-email-domains/disposable-email-domains)        | Community email-domain data useful for validation pipelines |

| [Verifly disposable-email-domains](https://github.com/james-sib/disposable-email-domains)               | Includes curated role-account local parts                   |



Role detection does **not** mean an address is invalid. A `support@example.com` mailbox can be completely deliverable.



---



# 🔤 Open-Source Email Syntax Validation



| Project                                                                                                 | Language   | Description                                                   |

| ------------------------------------------------------------------------------------------------------- | ---------- | ------------------------------------------------------------- |

| [email-validator](https://github.com/JoshData/python-email-validator)                                   | Python     | Robust syntax and domain validation                           |

| [AfterShip Email Verifier](https://github.com/AfterShip/email-verifier)                                 | Go         | Syntax validation                                             |

| [Visulima Email Verifier](https://github.com/visulima/visulima/tree/main/packages/email/email-verifier) | TypeScript | Syntax, Unicode and email structure validation                |

| [email-addresses](https://github.com/andris9/mailparser)                                                | JavaScript | Email parsing ecosystem                                       |

| [validator.js](https://github.com/validatorjs/validator.js)                                             | JavaScript | General-purpose validation library including email validation |



### Basic Validation



```text

Input

 │

 ▼

RFC / Syntax Validation

 │

 ├── Invalid → Reject

 │

 └── Valid

       │

       ▼

     Domain

       │

       ▼

    DNS / MX

```



---



# 🧠 Open-Source Email Intelligence & Enrichment



Commercial services often combine verification with additional intelligence.



| Project                                                                                                 | Description                                                                                   |

| ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |

| [Visulima Email Verifier](https://github.com/visulima/visulima/tree/main/packages/email/email-verifier) | Provider classification, name parsing, typo suggestions, quality scoring and email attributes |

| [AfterShip Email Verifier](https://github.com/AfterShip/email-verifier)                                 | Free-provider, disposable, role and reachability information                                  |

| [disposable](https://github.com/disposable/disposable)                                                  | Disposable-provider intelligence                                                              |

| [Mailchecker](https://github.com/FGRibreau/mailchecker)                                                 | Disposable email detection                                                                    |

| [burner-email-providers](https://github.com/wesbos/burner-email-providers)                              | Burner email provider database                                                                |



Potential enrichment signals include:



```text

Email

 │

 ├── Provider

 ├── Free / Business

 ├── Disposable

 ├── Role

 ├── No-Reply

 ├── Domain Age

 ├── Domain Reputation

 ├── MX Provider

 ├── Typo Suggestion

 ├── Catch-All

 └── SMTP Reachability

```



---



# ⚡ Open-Source Email Verification APIs



An open-source verification library can be wrapped in a REST API to create a self-hosted alternative to commercial verification APIs.



| Project                                                                                                 | API Capability | Description                                        |

| ------------------------------------------------------------------------------------------------------- | -------------- | -------------------------------------------------- |

| [AfterShip Email Verifier](https://github.com/AfterShip/email-verifier)                                 | ✅              | Includes a simple self-hosted API server reference |

| [UnlimitedVerifier](https://github.com/unlimitedverifier/free-email-verifier)                           | CLI / Library  | Lightweight self-hosted verification               |

| [Email Verification Tool](https://github.com/SyedSamrozeAli/Email-Verification-Tool)                    | Local App      | CSV-based verification interface                   |

| [Visulima Email Verifier](https://github.com/visulima/visulima/tree/main/packages/email/email-verifier) | Library        | Can be embedded into a Node.js API                 |

| [Email Verifier](https://github.com/yolodex-ai/email-verifier)                                          | Library / CLI  | Node.js verification engine                        |



### Example Self-Hosted API



```text

POST /v1/verify



{

  "email": "user@example.com"

}

```



Possible response:



```json

{

  "email": "user@example.com",

  "status": "deliverable",

  "syntax": true,

  "domain": true,

  "mx": true,

  "smtp": true,

  "catch_all": false,

  "disposable": false,

  "role": false,

  "free_provider": false

}

```



---



# 📊 Open-Source Bulk Email Verification



Bulk verification is particularly useful for replacing ZeroBounce/NeverBounce-style list-cleaning workflows.



| Project                                                                                                 | Capability                                      |

| ------------------------------------------------------------------------------------------------------- | ----------------------------------------------- |

| [Email Verification Tool](https://github.com/SyedSamrozeAli/Email-Verification-Tool)                    | CSV upload, live validation and result export   |

| [UnlimitedVerifier](https://github.com/unlimitedverifier/free-email-verifier)                           | CLI-based verification                          |

| [AfterShip Email Verifier](https://github.com/AfterShip/email-verifier)                                 | Library/API suitable for custom bulk processing |

| [Email Verifier](https://github.com/yolodex-ai/email-verifier)                                          | Multiple-email verification                     |

| [Visulima Email Verifier](https://github.com/visulima/visulima/tree/main/packages/email/email-verifier) | Programmatic verification                       |



### Bulk Processing Architecture



```text

CSV / Database

      │

      ▼

Email Parser

      │

      ▼

Deduplication

      │

      ▼

Syntax Validation

      │

      ▼

Disposable Check

      │

      ▼

DNS / MX

      │

      ▼

SMTP Verification

      │

      ▼

Catch-All Detection

      │

      ▼

Risk Classification

      │

      ▼

Clean Dataset

```



---



# 🏗️ Email Verification Architecture



```mermaid

flowchart TD



    A[Email Address] --> B[Syntax Validation]



    B --> C[Domain Extraction]



    C --> D[DNS / MX Check]



    D --> E[Disposable Check]



    E --> F[Role / Free Provider Check]



    F --> G[SMTP Verification]



    G --> H[Catch-All Detection]



    H --> I[Risk Analysis]



    I --> J[Final Classification]



    J --> K[Valid]



    J --> L[Invalid]



    J --> M[Risky]



    J --> N[Unknown]

```



---



# 🔄 Open-Source Email Verification Architecture



```mermaid

flowchart LR



    A[Client Application]



    A --> B[API Gateway]



    B --> C[Verification Service]



    C --> D[Syntax Engine]



    C --> E[DNS Resolver]



    C --> F[Disposable Database]



    C --> G[SMTP Engine]



    C --> H[Provider Detection]



    C --> I[Risk Engine]



    D --> J[Result Aggregator]

    E --> J

    F --> J

    G --> J

    H --> J

    I --> J



    J --> K[Verification Result]



    K --> L[(Cache)]



    K --> M[(Database)]



    K --> N[Webhook / API Response]

```



---



# 🔬 Email Verification Pipeline



```mermaid

flowchart TD



    A[Input Email]



    A --> B{Syntax Valid?}



    B -->|No| X[Invalid]



    B -->|Yes| C{Domain Exists?}



    C -->|No| X



    C -->|Yes| D{MX Available?}



    D -->|No| X



    D -->|Yes| E{Disposable?}



    E -->|Yes| Y[Risky / Disposable]



    E -->|No| F{Role Account?}



    F -->|Yes| G[Role Address]



    F -->|No| H[SMTP Probe]



    G --> H



    H --> I{SMTP Result}



    I -->|5xx| X



    I -->|4xx / Timeout| J[Unknown]



    I -->|2xx| K{Catch-All?}



    K -->|Yes| L[Risky / Catch-All]



    K -->|No| M[Deliverable]



    M --> N[Final Score]

    L --> N

    J --> N

    Y --> N

```



---



# 🎯 Verification Result Classification



A robust verification service should avoid treating every result as simply `true` or `false`.



| Result          | Meaning                                                  |

| --------------- | -------------------------------------------------------- |

| `valid`         | Strong evidence that the mailbox is deliverable          |

| `invalid`       | Strong evidence that the mailbox cannot receive mail     |

| `risky`         | Address may accept mail but has elevated risk            |

| `catch-all`     | Domain accepts arbitrary recipients                      |

| `disposable`    | Address belongs to a temporary/disposable provider       |

| `role-based`    | Address represents a functional role                     |

| `free-provider` | Address belongs to a consumer email provider             |

| `unknown`       | Verification could not reliably determine mailbox status |

| `greylisted`    | Receiving server temporarily deferred the request        |

| `timeout`       | Verification server did not respond in time              |

| `mailbox-full`  | Mailbox may exist but cannot currently receive messages  |

| `spam-trap`     | Address is associated with anti-abuse infrastructure     |



---



# 🧩 Commercial Platform → Open-Source Equivalent



| Commercial Platform             | Open-Source Building Blocks                                                                                     |

| ------------------------------- | --------------------------------------------------------------------------------------------------------------- |

| **ZeroBounce**                  | AfterShip Email Verifier + Visulima Email Verifier + disposable-email-domains + DNS + SMTP + custom risk engine |

| **NeverBounce**                 | AfterShip Email Verifier + bulk processing + disposable-domain database + SMTP                                  |

| **Bouncer**                     | Visulima Email Verifier + SMTP + disposable lists + custom scoring                                              |

| **DeBounce**                    | AfterShip Email Verifier + DNS + SMTP + disposable detection                                                    |

| **Emailable**                   | Visulima Email Verifier + DNS + SMTP + catch-all detection                                                      |

| **MailboxValidator**            | Python Email Validator + dnspython + SMTP verifier + disposable list                                            |

| **Verifalia**                   | Custom verification service built from SMTP + DNS + disposable + role detection                                 |

| **Abstract Email Verification** | Python Email Validator + DNS + SMTP + disposable detection                                                      |

| **QuickEmailVerification**      | AfterShip Email Verifier + bulk processing + REST API                                                           |

| **Kickbox**                     | SMTP verifier + DNS + disposable database + risk engine                                                         |

| **Clearout**                    | Visulima Email Verifier + disposable lists + SMTP + role detection                                              |

| **Hunter Email Verifier**       | AfterShip Email Verifier + DNS + SMTP + typo detection                                                          |

| **Proofy**                      | AfterShip Email Verifier + bulk processing + SMTP                                                               |

| **Mailboxlayer**                | Python Email Validator + dnspython + disposable detection + SMTP                                                |

| **Hunter**                      | Email verification stack + domain intelligence + enrichment                                                     |

| **Abstract API**                | Python Email Validator + DNS + SMTP + disposable intelligence                                                   |



---



# 🧱 Email Verification Layers



| Layer              | Commercial Examples            | Open-Source Options                        |

| ------------------ | ------------------------------ | ------------------------------------------ |

| API                | ZeroBounce, Emailable, Kickbox | FastAPI, Express, Go                       |

| Syntax             | All major providers            | Python Email Validator, validator.js       |

| DNS                | All major providers            | dnspython, miekg/dns, c-ares               |

| MX                 | All major providers            | dnspython, AfterShip Email Verifier        |

| Disposable         | ZeroBounce, Bouncer, Clearout  | disposable-email-domains, disposable       |

| Role Detection     | Bouncer, Clearout              | Visulima, AfterShip                        |

| SMTP               | ZeroBounce, NeverBounce        | AfterShip, Visulima                        |

| Catch-All          | Most major providers           | AfterShip, Visulima                        |

| Typo Detection     | ZeroBounce, Hunter             | Custom edit-distance / domain dictionaries |

| Provider Detection | Multiple                       | Visulima, AfterShip                        |

| Bulk Processing    | NeverBounce, ZeroBounce        | Celery, BullMQ, Kafka                      |

| Queue              | Managed                        | Redis, RabbitMQ, Kafka                     |

| Cache              | Managed                        | Redis                                      |

| Database           | Managed                        | PostgreSQL                                 |

| Monitoring         | Managed                        | Prometheus, Grafana, OpenTelemetry         |

| API Gateway        | Managed                        | Kong, Traefik, NGINX                       |

| Deployment         | Cloud                          | Docker, Kubernetes                         |



---



# ⚖️ Commercial vs Open-Source



| Capability             | SaaS Email Verification | Open-Source Stack                       |

| ---------------------- | ----------------------- | --------------------------------------- |

| API                    | Included                | Build yourself                          |

| Real-Time Verification | ✅                       | ✅                                       |

| Bulk Verification      | ✅                       | ✅                                       |

| Syntax Validation      | ✅                       | ✅                                       |

| DNS / MX               | ✅                       | ✅                                       |

| SMTP                   | ✅                       | ✅                                       |

| Catch-All              | ✅                       | ✅                                       |

| Disposable Detection   | ✅                       | ✅                                       |

| Role Detection         | ✅                       | ✅                                       |

| Spam-Trap Intelligence | Usually sophisticated   | Requires custom data                    |

| IP Reputation          | Provider-managed        | Must manage yourself                    |

| Proxy Infrastructure   | Included                | Build / operate yourself                |

| Greylisting Handling   | Sophisticated           | Must implement                          |

| Global Infrastructure  | Included                | Build yourself                          |

| Data Ownership         | Vendor-dependent        | Full control                            |

| Self-Hosting           | Usually limited         | ✅                                       |

| Air-Gapped             | Usually unavailable     | ✅                                       |

| Customization          | Medium                  | Very High                               |

| Vendor Lock-in         | Higher                  | Lower                                   |

| Engineering Effort     | Low                     | High                                    |

| Infrastructure Cost    | Usage-based             | Infrastructure-based                    |

| Source Code            | Usually unavailable     | Available                               |

| Custom Scoring         | Limited                 | Unlimited                               |

| Offline Verification   | Limited                 | Excellent for syntax/domain/list checks |



---



# 🚀 Recommended Open-Source Stacks



## 1. 🏆 General-Purpose Email Verification



```text

AfterShip Email Verifier

        +

Python Email Validator

        +

dnspython

        +

disposable-email-domains

        +

Redis

        +

PostgreSQL

        +

FastAPI

```



A practical foundation for building a self-hosted verification API.



---



## 2. ⚡ High-Accuracy SMTP Verification



```text

Visulima Email Verifier

        +

DNS Resolver

        +

Disposable Domain Database

        +

SMTP Verification

        +

Catch-All Detection

        +

Greylist Retry Engine

        +

Risk Scoring

```



Best when mailbox reachability is the primary objective.



---



## 3. 📊 Bulk Email Verification



```text

CSV / Database

      ↓

FastAPI

      ↓

Redis Queue

      ↓

Worker Pool

      ↓

Email Verification Engine

      ↓

PostgreSQL

      ↓

CSV / API / Webhook

```



Suitable for building a self-hosted NeverBounce/ZeroBounce-style list-cleaning system.



---



## 4. 🏢 Enterprise Email Verification



```text

API Gateway

      +

Authentication

      +

Verification Service

      +

DNS Resolver Cluster

      +

SMTP Worker Cluster

      +

Disposable Domain Database

      +

Risk Engine

      +

Redis

      +

PostgreSQL

      +

Prometheus

      +

Grafana

```



---



## 5. 🧪 Lightweight Developer API



```text

FastAPI

   +

Python Email Validator

   +

dnspython

   +

Disposable Domain List

   +

Redis

```



Best for signup forms and small SaaS applications where full SMTP probing is not always necessary.



---



# 🔐 Enterprise Email Verification Architecture



```mermaid

flowchart TB



    A[Applications]



    A --> B[API Gateway]



    B --> C[Authentication]



    C --> D[Verification API]



    D --> E[Rate Limiter]



    E --> F[Verification Queue]



    F --> G[Worker Cluster]



    G --> H[Syntax]



    G --> I[DNS / MX]



    G --> J[Disposable Database]



    G --> K[SMTP]



    G --> L[Role Detection]



    G --> M[Risk Engine]



    H --> N[Result Aggregator]

    I --> N

    J --> N

    K --> N

    L --> N

    M --> N



    N --> O[(PostgreSQL)]



    N --> P[(Redis)]



    N --> Q[Webhook]



    N --> R[API Response]



    S[Prometheus] --> G

    T[Grafana] --> S

```



---



# 🛡️ Anti-Abuse & Rate Limiting



SMTP verification infrastructure must be designed carefully.



```text

                    Verification Request

                            │

                            ▼

                      Rate Limiter

                            │

                            ▼

                     Domain Throttle

                            │

                            ▼

                     SMTP Worker

                            │

                            ▼

                    Receiving Server

```



Recommended controls:



* Global request limits

* Per-domain concurrency limits

* Per-domain delays

* Connection timeouts

* Exponential backoff

* Greylist retries

* Circuit breakers

* DNS caching

* SMTP connection pooling

* IP reputation monitoring

* Abuse prevention

* Audit logs



Never treat an SMTP timeout as proof that an address is invalid.



---



# 🧠 Why Email Verification Is Hard



A simplistic verifier might assume:



```text

MX exists

     ↓

Email is valid

```



But real-world email infrastructure is more complicated:



```text

                    Email Address

                         │

                         ▼

                    Syntax Check

                         │

                         ▼

                     DNS / MX

                         │

             ┌───────────┴───────────┐

             │                       │

          Valid MX                No MX

             │                       │

             ▼                       ▼

          SMTP                  Probably Invalid

             │

       ┌─────┼─────┐

       │     │     │

      2xx   4xx   5xx

       │     │     │

       ▼     ▼     ▼

    Accept Unknown Reject

       │

       ▼

  Catch-All Test

       │

   ┌───┴────┐

   │        │

  Yes       No

   │        │

 Risky   Higher Confidence

```



Factors that can make verification uncertain include:



* Greylisting

* Catch-all domains

* SMTP tarpits

* Anti-enumeration systems

* Firewalls

* Temporary DNS failures

* Mailbox quotas

* SMTP connection failures

* Provider-specific behavior

* Disposable addresses

* Spam traps

* Accept-all mail servers



---



# 🌐 Open-Source Email Verification Landscape



```mermaid

mindmap

  root((Email Verification))

    Core Verification

      Syntax

      DNS

      MX

      SMTP

      Catch-All

    Risk Detection

      Disposable

      Role

      Free Provider

      Spam Trap

      Greylisting

    Open Source Engines

      AfterShip

      Visulima

      Python Email Validator

      Email Verifier

      UnlimitedVerifier

    Data

      Disposable Domains

      Provider Lists

      Role Lists

      Domain Data

    Infrastructure

      Redis

      PostgreSQL

      RabbitMQ

      Kafka

      Kubernetes

    API

      FastAPI

      Express

      Go

    Monitoring

      Prometheus

      Grafana

      OpenTelemetry

```



---



# 🔬 Verification Technology Comparison



| Technology               | Syntax | DNS |  MX | SMTP | Catch-All | Disposable |   Role   |

| ------------------------ | :----: | :-: | :-: | :--: | :-------: | :--------: | :------: |

| AfterShip Email Verifier |    ✅   |  ✅  |  ✅  |   ✅  |     ✅     |      ✅     |     ✅    |

| Visulima Email Verifier  |    ✅   |  ✅  |  ✅  |   ✅  |     ✅     |      ✅     |     ✅    |

| Python Email Validator   |    ✅   |  ✅  |  ✅  |   ❌  |     ❌     |      ❌     |     ❌    |

| Email Verifier           |    ✅   |  ✅  |  ✅  |   ✅  |     ✅     |      ❌     | Provider |

| UnlimitedVerifier        |    ✅   |  ✅  |  ✅  |   ✅  |     ❌     |      ❌     |     ❌    |

| Email Verification Tool  |    ✅   |  ✅  |  ✅  |   ✅  |     ✅     |   Partial  |  Partial |

| Disposable Email Domains |    ❌   |  ❌  |  ❌  |   ❌  |     ❌     |      ✅     |     ❌    |

| Mailchecker              |    ❌   |  ❌  |  ❌  |   ❌  |     ❌     |      ✅     |     ❌    |



---



# 🏆 Recommended Projects by Use Case



| Use Case                          | Recommended Project          |

| --------------------------------- | ---------------------------- |

| Best general-purpose Go verifier  | **AfterShip Email Verifier** |

| Comprehensive TypeScript verifier | **Visulima Email Verifier**  |

| Python syntax + DNS validation    | **Python Email Validator**   |

| Node.js SMTP verification         | **Email Verifier**           |

| Disposable detection              | **disposable-email-domains** |

| Disposable domain database        | **disposable**               |

| Lightweight Python verification   | **UnlimitedVerifier**        |

| CSV verification                  | **Email Verification Tool**  |

| DNS infrastructure                | **dnspython**                |

| Production queue                  | **Redis / RabbitMQ / Kafka** |

| API                               | **FastAPI / Go / Express**   |

| Database                          | **PostgreSQL**               |

| Monitoring                        | **Prometheus + Grafana**     |



---



# 🏗️ Building a ZeroBounce Alternative



A realistic open-source ZeroBounce-style platform can be constructed from:



```text

                         ┌─────────────────────┐

                         │      REST API       │

                         └──────────┬──────────┘

                                    │

                         ┌──────────▼──────────┐

                         │ Verification Engine │

                         └──────────┬──────────┘

                                    │

          ┌─────────────────────────┼─────────────────────────┐

          │                         │                         │

    ┌─────▼─────┐             ┌─────▼─────┐             ┌────▼─────┐

    │  Syntax   │             │   DNS     │             │  SMTP    │

    │ Validator │             │   / MX    │             │  Probe   │

    └─────┬─────┘             └─────┬─────┘             └────┬─────┘

          │                         │                         │

          └─────────────────────────┼─────────────────────────┘

                                    │

                           ┌────────▼────────┐

                           │  Risk Engine    │

                           └────────┬────────┘

                                    │

             ┌──────────────────────┼──────────────────────┐

             │                      │                      │

        Disposable               Role                 Catch-All

        Detection              Detection              Detection

             │                      │                      │

             └──────────────────────┼──────────────────────┘

                                    │

                           ┌────────▼────────┐

                           │ Result Scoring  │

                           └────────┬────────┘

                                    │

                           ┌────────▼────────┐

                           │ API / Webhook   │

                           └─────────────────┘

```



---



# 🧩 Minimal Self-Hosted Implementation



```text

API

 │

 ├── FastAPI

 │

 ▼

Verification Engine

 │

 ├── Python Email Validator

 ├── dnspython

 ├── SMTP Client

 └── Disposable Domain List

 │

 ▼

Redis

 │

 ▼

PostgreSQL

 │

 ▼

Prometheus + Grafana

```



This architecture is enough to build a basic self-hosted email-verification service for:



* SaaS signup forms

* Lead-generation systems

* CRM imports

* Newsletter lists

* Customer databases

* Account registration

* Contact forms

* Marketing databases



---



# 🚀 Advanced Open-Source Stack



For a production-scale platform:



```text

                    API Gateway

                         │

                         ▼

                  Authentication

                         │

                         ▼

                   Rate Limiter

                         │

                         ▼

                  Message Queue

                         │

              ┌──────────┼──────────┐

              │          │          │

           Worker     Worker     Worker

              │          │          │

              └──────────┼──────────┘

                         │

          ┌──────────────┼──────────────┐

          │              │              │

        DNS            SMTP          Intelligence

          │              │              │

          └──────────────┼──────────────┘

                         │

                  Result Engine

                         │

              ┌──────────┼──────────┐

              │          │          │

           Redis     PostgreSQL   Analytics

```



Potential infrastructure:



```text

FastAPI / Go

Redis

RabbitMQ / Kafka

PostgreSQL

Kubernetes

Prometheus

Grafana

OpenTelemetry

```



---



# 🌟 Why Open-Source Email Verification Matters



Commercial services package the following capabilities into a single API:



```text

Syntax

   +

DNS

   +

MX

   +

SMTP

   +

Disposable Detection

   +

Role Detection

   +

Catch-All

   +

Provider Intelligence

   +

Risk Scoring

   +

Bulk Processing

   +

Analytics

```



Open source allows organizations to assemble these capabilities themselves:



```text

Open-Source Components

          │

          ▼

┌──────────────────────────────┐

│ Email Verification Engine   │

│ DNS / MX                    │

│ SMTP                        │

│ Disposable Lists            │

│ Role Detection              │

│ Risk Engine                 │

│ Queue                       │

│ Database                    │

│ API                         │

└──────────────────────────────┘

          │

          ▼

Self-Hosted Email Verification

```



Advantages include:



* Full data ownership

* Self-hosting

* Private-cloud deployment

* Air-gapped deployment

* Custom verification rules

* Custom risk scoring

* Custom disposable-domain lists

* Custom SMTP behavior

* No mandatory API vendor

* No per-verification SaaS charge

* Complete control over verification data

* Ability to integrate verification directly into internal systems



---



# 🤝 Contributing



Contributions are welcome!



Please consider contributing:



* New Email Verification APIs

* Open-source verification engines

* SMTP verification libraries

* DNS/MX tools

* Disposable email datasets

* Role-account datasets

* Email parsing libraries

* Provider detection databases

* Bulk verification tools

* Self-hosted APIs

* Verification benchmarks

* Deliverability research

* Anti-abuse techniques

* Verification architectures

* Documentation

* Tutorials



When adding an open-source project, please verify its **current license** and distinguish genuine open-source projects from source-available or proprietary products.



---



# ⚠️ Disclaimer



This repository is an independent technical curation and is **not affiliated with or endorsed by any company or project listed here**.



Email verification is probabilistic. An SMTP server accepting a `RCPT TO` command does not guarantee that an email will ultimately be delivered.



SMTP behavior can be affected by:



* Greylisting

* Catch-all configuration

* Anti-enumeration systems

* Rate limiting

* Firewalls

* Temporary server failures

* Spam filtering

* Mailbox quotas

* Provider-specific policies



Always verify the current license, API terms, acceptable-use policies and technical behavior of individual projects before deploying them in production.



Projects and services can change their licensing, pricing, features and availability over time.



---



## ⭐ Star This Repository



If you are interested in:



* Email Verification

* Email Validation

* Email Deliverability

* SMTP Verification

* DNS / MX Validation

* Disposable Email Detection

* Email Hygiene

* Lead Validation

* Email APIs

* Open-Source Email Infrastructure

* Self-Hosted SaaS Alternatives



consider giving this repository a ⭐ **Star** and contributing new projects.



---



**Last updated: September 2026**
