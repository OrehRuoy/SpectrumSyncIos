# Privacy Policy for Spectrum Sync (iOS)

Your privacy comes first. Here's how Spectrum Sync protects it.

**Effective date:** July 24, 2026  
**Last updated:** October 26, 2026

---

## 1. Introduction

This Privacy Policy describes how **Spectrum Sync** ("**App**," "**we**," "**us**," or "**our**") collects, uses, stores, shares, and protects information when you install or use our **iOS** application and its custom keyboard extension.

Spectrum Sync is a social language coaching tool designed to help neurodivergent users communicate more confidently in text-based conversations. The App includes a settings and onboarding experience and an optional **Spectrum Sync Keyboard** that analyzes text you type with that keyboard to provide real-time coaching feedback.

**Developer / Data Controller:** Brock Hall  
**Contact email:** [hallanhype@gmail.com](mailto:hallanhype@gmail.com)  
**iOS bundle ID:** `com.spectrumsync.keyboard`  
**Keyboard extension:** `com.spectrumsync.keyboard.keyboard`  
**Privacy policy URL:** https://orehruoy.github.io/SpectrumSyncIos/privacy-policy.html

This policy applies to the **iOS** app and keyboard only.

By downloading, installing, or using Spectrum Sync on iOS, you agree to this Privacy Policy. If you do not agree, do not use the App.

---

## 2. Summary (Plain Language)

- Spectrum Sync **does not require you to create an account**.
- Coaching works only if you **voluntarily enable** the Spectrum Sync Keyboard and grant **Allow Full Access** so the keyboard can use the network for cloud AI when needed.
- When coaching is active, the App may analyze **text you type using the Spectrum Sync Keyboard** (not text typed with other keyboards, and not by reading other apps’ fields in the background).
- AI analysis prefers **Apple Intelligence** on-device when available (iOS 26). Otherwise it uses **Google’s Gemini** through **Firebase AI Logic** (model `gemini-3.5-flash-lite`), sending the current sentence plus up to five earlier sentences held only in short-term keyboard memory. **Some coaching text leaves your device for that cloud step**; we do not operate our own coaching transcript database.
- We **do not sell** your personal information.
- We **do not use** third-party advertising networks.
- **Firebase Analytics** (in the keyboard extension) receives only limited, anonymous engagement signals we choose to log—not your message text. **Usage counters** (keyboard opens, coach pills shown, and similar integers) stay on your device unless you include them in optional feedback.
- Most settings and preferences stay **on your device**. Subscription status is handled by **Apple App Store / StoreKit**.

---

## 3. Information We Collect

### 3.1 Information You Provide Directly

#### A. Text you type (User Content)

When the Spectrum Sync Keyboard is enabled, Full Access is allowed, disclosure is accepted, and coaching is not paused, the keyboard may access text from the field you are typing in **through the keyboard’s document proxy**, including:

- Message drafts in messaging, email, and social apps (when Spectrum Sync Keyboard is the active keyboard)
- The current sentence or line being composed
- Up to **5** completed prior sentences in that same field, each trimmed to **180** characters (up to **720** characters of prior context total), held only in short-term keyboard memory so a follow-up can be coached with conversation context (for example pronouns like “that” or “he”). This buffer is **not written to disk** and is cleared when you change fields, hide the keyboard, focus a private field, or coaching resets.

This text is used **only** to provide coaching feedback (tone warnings, explanations, and suggested rewrites).

**When it is sent for analysis:** about **2 seconds** after you stop typing (or about **3.5 seconds** after a delete), and when a sentence ends with `.`, `!`, `?`, or return—subject to minimum length/word checks and usage limits.

**What goes to the cloud:** If on-device Apple Intelligence is unavailable or does not produce a usable result, the keyboard sends the trimmed current sentence (up to **280** characters), optional prior-sentence context as above, coaching instructions (including your sensitivity and coaching toggles), and technical request metadata to **Google** via **Firebase AI Logic** (Gemini). **We do not store your coaching sentences on our servers** or keep a long-term transcript on the device. Google processes requests under [Google’s terms and privacy policies](https://policies.google.com/privacy) for the Firebase / Gemini services.

**On-device path:** When Apple Intelligence is available and returns a usable result, that analysis stays on the device for that check.

We apply safeguards to **avoid analyzing** text when:

- The field is secure (`isSecureTextEntry`)
- The field’s content type is a one-time code, password, new password, credit card, telephone number, email address, username, URL, or an address (street, city, state, postal code, country, or location)
- The keyboard type is a number pad, ASCII number pad, phone pad, email, URL, web search, or decimal pad
- Coaching is paused
- You have not accepted the in-app disclosure
- Local or cloud usage limits block analysis

#### B. App settings and preferences

Stored locally on your device (shared between the host app and keyboard via an App Group), including:

- AI sensitivity / aggression filter level
- Coaching toggles (for example bluntness filter, explain-why)
- Theme preferences
- Whether coaching is paused
- Trial start timestamp
- Premium subscription active flag (synced from App Store purchase state)

#### C. In-app feedback form (optional)

From **Settings → Feedback**, you may send a message to the developer through **Web3Forms** ([web3forms.com](https://web3forms.com)). The form sends:

- The **message** you type (required)
- An **email address**, only if you choose to enter one (optional—we use it only to reply)
- **Platform** (iOS), **app version**, and **device model/OS** string
- **Usage counts** from on-device diagnostics (integers and timestamps such as keyboard opens and coach pills shown—**not** message text)

We use feedback **only** to respond and improve the App. You do not have to use the form.

#### D. Support communications

If you email us at [hallanhype@gmail.com](mailto:hallanhype@gmail.com), we receive the information you choose to send.

### 3.2 Information Collected Automatically

#### A. Keyboard and field context

The keyboard may use:

- Whether the active field is secure or treated as private (see list above)
- Limited document-proxy text needed for sentence detection
- A short-term in-memory list of recent completed sentences (not saved to disk)
- Local counters for cloud AI limits

#### B. Subscription and billing information

Purchases, free trials, and subscription status are processed by **Apple App Store / StoreKit**. Apple may provide us with:

- Whether you have an active subscription or trial entitlement
- Product identifiers (for example `premium_access_monthly`, `premium_access_yearly`, `free_forever`)
- Transaction metadata needed to verify premium access

We do **not** receive your full payment card number. Payment details are handled by Apple.

#### C. Firebase Analytics (keyboard extension)

When the keyboard extension runs with network access, **Google Analytics for Firebase** may receive:

- **Automatic metrics** the Firebase SDK may collect (for example app instance identifiers and standard technical/device fields per Google’s SDK behavior)
- **Custom events we log intentionally** (no message or coaching text):
  - `service_enabled` — once per install, the first time cloud coaching is used
  - `daily_limit_reached` — at most once per calendar day when a trial user hits the daily cloud cap, with `trial_day` (1–7)

These events are **not linked to your name, email, or typed messages** in our systems.

#### D. On-device usage counters (not analytics uploads)

The keyboard maintains **funnel statistics** locally in the App Group: counts and first/last timestamps (for example keyboard opens, coach pills shown, rewrites accepted, errors, daily-limit hits). **They do not include message text** and are **not** sent to Firebase Analytics. They appear in a hidden diagnostics panel in the host app and are included **only if you submit the feedback form**.

### 3.3 Information We Do Not Collect

We do **not** intentionally collect:

- Passwords from secure text fields (coaching is skipped)
- Full browsing history
- Contacts, photos, microphone audio, or camera data
- A persistent account profile on our servers
- Advertising identifiers for ad targeting

---

## 4. How We Use Information

| Purpose | Examples |
|--------|----------|
| **Provide coaching** | Analyze typed text and show tone feedback, warnings, and rewrite suggestions on the keyboard |
| **Safety** | Skip secure and private fields; honor pause and disclosure settings |
| **Operate the App** | Save settings and pause state locally (App Group) |
| **Manage subscriptions** | Verify premium access and free-trial eligibility via the App Store |
| **Limit cloud AI usage** | Enforce daily/hourly caps and cooldowns |
| **Respond to you** | Answer feedback and support emails |
| **Legal compliance** | Meet legal obligations |

We do **not** use your typed message content for advertising or sell it to data brokers.

---

## 5. Custom Keyboard and Full Access Disclosure

Spectrum Sync uses a custom **iOS Keyboard Extension**.

### What the keyboard can access

When enabled and Full Access is allowed, it may:

- See text in the active input field via the system document proxy (only while Spectrum Sync Keyboard is selected)
- Use the network to send coaching text and instructions to Google (Gemini via Firebase AI Logic) when on-device Apple Intelligence is not used
- Show a coaching pill / panel above the keyboard
- Insert suggested replacement text when you choose a suggestion

### Why Full Access is required

iOS sandboxes keyboard extensions by default. **Allow Full Access** is required for network access so the keyboard can call Firebase AI Logic (Gemini) and related Firebase services when **Apple Intelligence** is unavailable or does not produce a usable result. Without Full Access, cloud coaching cannot run (on-device Apple Intelligence may still work on supported devices when enabled).

### What we do not do

We do **not**:

- Read text typed with other keyboards
- Use Accessibility APIs to monitor other apps in the background
- Sell keystroke data
- Use coaching text for advertising

### Your control

You can stop processing at any time by:

1. Switching back to another keyboard
2. Turning off **Allow Full Access** for Spectrum Sync Keyboard in iOS Settings
3. Using **Pause coaching** inside Spectrum Sync
4. Uninstalling the App

---

## 6. AI Processing

Spectrum Sync uses artificial intelligence to analyze text and generate coaching feedback.

On iOS, analysis prefers **Apple Intelligence** (Apple’s on-device foundation model via the Foundation Models framework) when the device supports it and Apple Intelligence is enabled (iOS 26). Otherwise — or if on-device analysis is unavailable — the App uses **Google’s generative AI** through **Firebase AI Logic**, model id **`gemini-3.5-flash-lite`**.

Cloud requests send the **current sentence** (up to **280** characters) and may include **up to 5** recently completed prior sentences as context (limits above). That context lives only in keyboard RAM, is not stored long-term on the device, and is not sent as a chat history or account transcript. The model is instructed to coach only the current sentence.

Cloud requests are subject to app-side limits, including approximately:

- **25** cloud coaching requests per day during the free trial
- **150** cloud coaching requests per day for active premium subscribers
- **40** cloud requests per hour and additional spacing/cooldown limits after errors or rate limits

AI responses are structured coaching results (status, short warning, reasoning, and suggestions). Choosing a suggestion may replace text in the active field via the keyboard.

We do not routinely have humans read your typed content. Feedback and support messages you send us are handled separately.

If you tap the quoted word in a suggestion, that **word** may be saved locally as a learned word for autocorrect (`learned_words` in the App Group). It is not uploaded as coaching text.

---

## 7. How We Share Information

| Provider | Purpose | Data involved |
|---------|---------|---------------|
| **Google Firebase / Firebase AI Logic (Gemini)** | Cloud AI inference | Trimmed coaching text, prior-sentence context, prompts/instructions, technical request metadata |
| **Google Analytics for Firebase** | Anonymous engagement analytics (keyboard extension) | SDK automatic metrics; custom events `service_enabled` and `daily_limit_reached` only—no message content |
| **Web3Forms** | Deliver optional in-app feedback to the developer | Your message; optional email; platform, version, device; usage counts |
| **Apple App Store / StoreKit** | Subscriptions, trials, purchase verification | Product IDs, subscription/transaction status |

We may disclose information if required by law or to protect rights and safety. We do **not** sell personal information for cross-context behavioral advertising.

---

## 8. Data Retention

| Data type | Retention |
|----------|-----------|
| Local settings (App Group JSON) | Until you change settings, clear app data, or uninstall |
| Coaching text in memory | Only while processing the current request |
| Recent-sentence coaching context | In keyboard RAM only (up to 5 completed sentences). Cleared when the keyboard hides, the text field changes, a private field is focused, or coaching resets. Not written to disk. |
| Words you choose to keep | Saved on device under `learned_words` for autocorrect; not uploaded |
| Cloud usage counters | Stored locally; reset per daily/hourly logic |
| Funnel usage counters | Stored locally until uninstall; optional copy sent with feedback |
| App Store purchase records | Retained by Apple under Apple’s policies; we retain local entitlement flags as needed |
| Feedback via Web3Forms | Retained as long as needed to respond and operate support |
| Support emails | As long as needed to respond |

---

## 9. Data Security

We use reasonable measures designed to protect information, including:

- Skipping secure and private text fields
- Limiting cloud transmission to the current sentence plus a small, short-lived context window
- Using encrypted transport (HTTPS/TLS) for cloud AI and feedback requests
- Storing settings in the App’s App Group container

No method of transmission or storage is 100% secure.

---

## 10. Your Choices and Rights

### Controls in the App

- Enable or disable the Spectrum Sync Keyboard and Full Access
- Pause coaching
- Adjust sensitivity and coaching options
- Manage or cancel subscriptions in iOS Settings → Apple ID → Subscriptions

### Access, deletion, correction

Because most data is stored locally:

- Change settings in the App
- Delete the App to remove local App data
- Email [hallanhype@gmail.com](mailto:hallanhype@gmail.com?subject=Spectrum%20Sync%20iOS%20Data%20Deletion%20Request) for help with information you sent by email or feedback

### Children

Spectrum Sync is not directed to children under 13. We do not knowingly collect personal information from children under 13.

---

## 11. International Users

If you use the App outside the United States, your information may be processed in the United States and other countries where Google and Apple operate.

---

## 12. Changes to This Policy

We may update this Privacy Policy from time to time. The “Last updated” date at the top will change when we do. Continued use of the App after an update means you accept the revised policy.

---

## 13. Contact

**Brock Hall**  
Email: [hallanhype@gmail.com](mailto:hallanhype@gmail.com)

Privacy policy URL: https://orehruoy.github.io/SpectrumSyncIos/privacy-policy.html
