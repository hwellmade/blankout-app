# BlankOut — Android PII Redaction App

**BlankOut** is an Android app that automatically detects and redacts personal information (PII) from document photos before the user shares them — fully on-device, no internet connection required, no cloud processing, no account needed.

---

## Problem

When people share document photos with AI assistants (ChatGPT, Gemini, Claude) or via messaging apps, those documents often contain sensitive personal data: names, ID numbers, phone numbers, addresses, credit card details. Most users do not notice or have no easy way to remove that data before sharing.

BlankOut solves this with a one-tap redaction flow that runs entirely on the Android device.

---

## Key Features

- **On-device AI** — all OCR, entity detection, and redaction runs locally on the phone. No photo or text ever leaves the device.
- **4-layer PII detection pipeline** — regex patterns, Google ML Kit entity extraction, DistilBERT NER (via ONNX Runtime), and a user-defined custom blacklist.
- **Multi-language OCR** — detects text in Latin, Chinese, Japanese, and Korean scripts.
- **EXIF/GPS metadata stripping** — removes location and camera metadata from output images automatically.
- **Manual edit mode** — users can draw or remove redaction boxes after AI detection.
- **Custom blacklist** — users can add their own words or phrases to always redact.
- **No account, no subscription** — freemium model with a one-time unlock purchase.

---

## How It Works

1. User selects a document photo (camera or gallery).
2. App runs multi-language OCR across the image.
3. Each detected text block passes through the 4-layer PII detection pipeline.
4. Black redaction boxes are drawn over all flagged regions.
5. User reviews the result, edits if needed, then shares or saves.

The entire process runs on the Android device in seconds. No data is transmitted.

---

## PII Detection Pipeline

| Layer | Technology | What it detects |
|---|---|---|
| 1. Regex | Custom patterns | Phone numbers, emails, ID numbers, credit cards, dates |
| 2. Entity Extraction | Google ML Kit | Addresses, payment cards, phone numbers (semantic) |
| 3. NER | DistilBERT (ONNX Runtime) | Person names — multilingual |
| 4. User Blacklist | Local DataStore | User-defined words and phrases |

Results from all layers are combined (OR logic) — if any layer flags a text block, it is redacted.

---

## Tech Stack

- **Language:** Kotlin
- **UI Framework:** Jetpack Compose
- **OCR:** Google ML Kit Text Recognition (Latin, Chinese, Japanese, Korean)
- **Entity Detection:** Google ML Kit Entity Extraction
- **NER Model:** DistilBERT running via ONNX Runtime for Android
- **Billing:** Google Play Billing (one-time in-app purchase)
- **Local Storage:** DataStore Preferences
- **Metadata Stripping:** AndroidX ExifInterface
- **Minimum Android version:** Android 8.0 (API 26)
- **Website:** Next.js, hosted on Vercel

---

## Pricing

- **Free:** 5 redactions per day, resets at midnight (tracked locally, no account)
- **Unlimited:** €3.99 one-time purchase, no subscription, no account required

---

## Privacy

- No data collection
- No analytics or crash reporting
- No network requests (except one-time ML Kit model download on first use)
- Camera and photo access used locally only
- Privacy policy: [blankout-offline.com/privacy](https://blankout-offline.com/privacy)

---

## Links

- **Website:** [blankout-offline.com](https://blankout-offline.com)
- **Google Play:** [BlankOut on Google Play](https://play.google.com/store/apps/details?id=com.blankout)
- **Support:** support@blankout-offline.com

---

## Repository

This is the public product repository for BlankOut. Source code is proprietary.  
For questions, feature requests, or bug reports, please open an Issue.

---

## Use Cases

- Sharing medical documents with AI assistants without exposing patient data
- Redacting ID cards, passports, or driving licences before sending photos
- Removing personal details from invoices, contracts, or bank statements
- Privacy-first document handling for professionals in finance, healthcare, and legal industries

---

*BlankOut — Android document redaction, on-device AI, PII detection, privacy-first, no cloud.*
