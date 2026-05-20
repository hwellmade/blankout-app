# BlankOut — Redact Personal Info From Documents Before Sharing With AI

**On-device PII redaction for Android. Free for everyday use. No cloud. No account. Works offline.**

Every time you share a bill, medical report, or bank statement with an AI assistant like **ChatGPT, Gemini, Claude, Copilot, or Perplexity**, your sensitive data — name, account numbers, address, ID numbers — gets uploaded to a cloud server you don't control.

BlankOut fixes that. It's a free Android app that automatically detects and redacts personal information (PII) from your documents using **on-device AI** — no internet required, no data leaves your phone. GPS and EXIF metadata stripped too. You share a clean, redacted version of your document with one tap. **AI gets only what it needs.**

---

## Why I Built BlankOut

Hi, I'm **Ji-Ling**. I built BlankOut because I kept hitting the same wall.

Every time I wanted AI to help me with a document — a medical report, an insurance form, a contract — I'd freeze. The document had my name, my account number, my address on it. I didn't want to hand that to ChatGPT or any cloud server.

So I'd either give up, or spend ten minutes manually covering things with a photo editor.

That workaround is embarrassing. I'm literally hiding my data with my hand.

BlankOut is the one-tap, fully offline tool I wished existed. It redacts PII from any document using edge AI, so you can ask AI anything — without sending your private life to a cloud server.

---

## What BlankOut Does

Pick a document photo. BlankOut scans it on your phone, detects the personal info inside — **names, addresses, ID numbers, phone numbers, emails, credit cards, bank account numbers** — and covers it with black redaction boxes. You review the result, tap share, done.

Everything runs locally on your Android device. Your photo never leaves the phone. No upload. No account. No login. No tracking.

---

## What You Can Use BlankOut For

- **Ask ChatGPT to explain a medical bill** without showing it your name, insurance ID, or address.
- **Send a bank statement to a financial-advice AI** with your account number and balance hidden.
- **Get an AI to summarize a contract** without leaking client names or signatures.
- **Share an insurance form** with a chatbot without exposing your policy number.
- **Translate a foreign-language receipt** without revealing where you live.
- **Post a screenshot to Reddit, X, or a forum** without doxxing yourself.
- **Send an ID card photo to a hotel, landlord, or rental** with the document number blacked out.
- **Share a payslip or tax form** with a tax-advice AI while hiding personal identifiers.

---

## Why On-Device Redaction Matters

Most "document redaction" or "PII removal" tools online work by uploading your file to their server, processing it in the cloud, and sending the redacted version back. **That defeats the purpose.** To protect your data from one cloud, you've handed it to another.

BlankOut runs every step — OCR, name detection, entity extraction, redaction, metadata stripping — directly on your Android phone. There's no upload step, because there's no server. Your photo and its contents never touch the internet.

---

## BlankOut vs. The Alternatives

|  | **BlankOut** | Manually blur in Photos app | Cloud redaction tools | Send raw to ChatGPT / Gemini / Claude |
|---|---|---|---|---|
| Detects PII automatically | Yes (on-device AI) | No — you eyeball it | Yes | No |
| Data stays on your phone | Yes | Yes | No (uploaded) | No (uploaded) |
| Works offline | Yes | Yes | No | No |
| Strips GPS / EXIF metadata | Yes | No | Sometimes | No |
| Time per document | Seconds | 5–10 minutes | Seconds | Instant — but data is exposed |
| Account required | No | No | Usually yes | Usually yes |
| Cost | Free, optional €3.99 unlock | Free | Subscription | Free / paid (data leaked) |

---

## How It Works

1. **Open a photo.** From your camera or gallery.
2. **Let BlankOut scan it.** On-device OCR reads the document. On-device AI flags names, IDs, phone numbers, addresses, account numbers, emails, credit cards, and any custom words you've added to your blacklist.
3. **Review and share.** Tap to add or remove redactions if you need to. Then share the clean version with any AI app, messenger, or email — or save it to your gallery.

The entire process happens on your phone in seconds.

---

## What BlankOut Detects

- Names of people — multilingual (English, Chinese, Japanese, Korean)
- Phone numbers
- Email addresses
- Postal and street addresses
- National ID, passport, and driving licence numbers
- Credit card and bank account numbers
- Dates (including dates of birth)
- GPS coordinates and camera EXIF metadata
- **Custom words and phrases** you add to your private blacklist (employer names, project codenames, family members, anything)

---

## Frequently Asked Questions

### Is it safe to upload my bank statement or medical report to ChatGPT?

Not really. When you send a document to ChatGPT, Gemini, Claude, or any cloud AI, the file is processed on their servers. Even with strong privacy policies, the data leaves your device. For sensitive documents — anything with your name, account number, ID, or address — you should redact before sharing. That's what BlankOut is for.

### How do I remove personal info from a photo before sharing it with AI?

On Android, the easiest way is BlankOut. Open the photo, let BlankOut scan it, and it automatically blacks out names, IDs, addresses, phone numbers, and account numbers. You can also manually add or remove redactions. Then share or save the clean version.

### Does BlankOut work offline?

Yes. All scanning and redaction runs on your phone, with no internet connection needed. The only exception is a one-time download of the on-device AI model the first time you use the app.

### Does BlankOut send my photos anywhere?

No. There is no server, no analytics, no crash reporting, no account. Your photos are read locally, redacted locally, and stay on your device until you choose to share or save them.

### What's the difference between BlankOut and just blurring with the Photos app?

Manual blurring relies on your eyes catching every sensitive field — which on a bank statement or medical report can be twenty-plus items spread across the page. BlankOut uses on-device AI to find them all automatically in seconds. It also strips invisible metadata (GPS coordinates, camera info, timestamps) that manual blurring leaves behind.

### Can I use BlankOut for HIPAA or GDPR-sensitive documents?

BlankOut never transmits your data, so the document itself doesn't leave your device — which is a strong starting point for any privacy-sensitive workflow. Whether a specific use case is fully HIPAA- or GDPR-compliant depends on the rest of your handling, but using BlankOut significantly reduces exposure compared to uploading raw documents to a cloud AI service.

### What languages does BlankOut support?

OCR works on Latin scripts (English, Spanish, French, German, Portuguese, Italian, and others), Chinese, Japanese, and Korean. Name detection is multilingual.

### Is there an iPhone or iOS version of BlankOut?

Not yet. BlankOut is Android only for now.

### Is BlankOut really free?

Yes. **Five redactions per day are free, forever**, with no account and no signup — enough for most everyday use. If you need unlimited redactions, there's a **one-time €3.99 unlock** — no subscription, no recurring charges, no account.

### How does BlankOut detect names and IDs without sending data to the cloud?

BlankOut runs small, optimised AI models directly on your phone — Google ML Kit for OCR and entity extraction, plus a DistilBERT name-detection model via ONNX Runtime. Modern Android phones are powerful enough to run these locally in under a second.

### Can I redact custom words like my employer's name or a project codename?

Yes. BlankOut has a private custom blacklist where you can add any word, name, or phrase that should always be redacted from your documents.

### What if BlankOut misses something or redacts the wrong thing?

After the AI scan, you get a review screen. Tap any block to remove a redaction, or draw a new black box over anything the AI missed. Nothing is shared until you tap share.

---

## Pricing

- **Free for everyday use** — 5 documents per day, resets at midnight. No account, no signup, no tracking. Enough for most people.
- **Unlimited unlock** — €3.99 one-time purchase. No subscription. No account. Pay once, use forever.

---

## Privacy Commitments

- No data collection of any kind
- No analytics, no crash reporting, no telemetry
- No accounts, logins, or sign-ups
- No network requests during redaction (one-time AI model download on first launch only)
- Camera and photo access used locally only
- Full privacy policy: [blankout-offline.com/privacy](https://blankout-offline.com/privacy)

---

## Under the Hood (For the Curious)

- **Language:** Kotlin
- **UI Framework:** Jetpack Compose
- **OCR:** Google ML Kit Text Recognition (Latin, Chinese, Japanese, Korean)
- **Entity Detection:** Google ML Kit Entity Extraction
- **Name Detection (NER):** DistilBERT via ONNX Runtime for Android
- **Local Storage:** DataStore Preferences (for the custom blacklist)
- **Metadata Stripping:** AndroidX ExifInterface
- **Billing:** Google Play Billing (one-time in-app purchase)
- **Website:** Next.js on Vercel
- **Minimum Android version:** 8.0 (API 26)

### PII Detection Pipeline

| Layer | Technology | What it detects |
|---|---|---|
| 1. Regex | Custom patterns | Phone numbers, emails, ID numbers, credit cards, dates |
| 2. Entity Extraction | Google ML Kit | Addresses, payment cards, semantic phone numbers |
| 3. Name Detection (NER) | DistilBERT (ONNX Runtime) | Person names — multilingual |
| 4. User Blacklist | Local DataStore | User-defined words and phrases |

Results from all four layers are combined with OR logic — if any layer flags a text block, it gets redacted.

---

## Links

- **Website:** [blankout-offline.com](https://blankout-offline.com)
- **Google Play:** [BlankOut on Google Play](https://play.google.com/store/apps/details?id=com.blankout)
- **Support:** support@blankout-offline.com
- **Feedback & bug reports:** open an Issue in this repository

---

## About This Repository

This is the public product repository for BlankOut. The Android source code is proprietary and not included here. Use the Issues tab for feature requests, bug reports, or product feedback.

---

*BlankOut is a free, on-device document redaction app for Android. It automatically removes names, ID numbers, addresses, phone numbers, account numbers, and GPS metadata from your photos so you can safely share bank statements, medical reports, ID cards, contracts, invoices, payslips, and screenshots with AI assistants like ChatGPT, Gemini, Claude, Copilot, or Perplexity — without uploading your personal data to the cloud.*
