# Privacy Policy for Spectrum Sync (iOS)

**Effective date:** July 24, 2026  
**Last updated:** July 24, 2026

---

## 1. Introduction

This Privacy Policy describes how **Spectrum Sync** ("**App**," "**we**," "**us**," or "**our**") collects, uses, stores, shares, and protects information when you install or use our **iOS** application and its custom keyboard extension.

Spectrum Sync is a social language coaching tool designed to help neurodivergent users communicate more confidently in text-based conversations. The App includes a settings and onboarding experience and an optional **Spectrum Sync Keyboard** that analyzes text you type with that keyboard to provide real-time coaching feedback.

**Developer / Data Controller:** Brock Hall  
**Contact email:** [hallanhype@gmail.com](mailto:hallanhype@gmail.com)  
**iOS bundle ID:** `com.spectrumsync.keyboard`  
**Keyboard extension:** `com.spectrumsync.keyboard.keyboard`  
**Privacy policy URL:** https://orehruoy.github.io/SpectrumSyncIos/privacy-policy.html

This policy applies to the **iOS** product only. The Android version of Spectrum Sync has a separate privacy policy.

By downloading, installing, or using Spectrum Sync on iOS, you agree to this Privacy Policy. If you do not agree, do not use the App.

---

## 2. Summary (Plain Language)

- Spectrum Sync **does not require you to create an account**.
- Coaching works only if you **voluntarily enable** the Spectrum Sync Keyboard and grant **Allow Full Access** so the keyboard can use the network for AI analysis.
- When coaching is active, the App may analyze **text you type using the Spectrum Sync Keyboard** (not text typed with other keyboards, and not by reading other apps’ fields in the background).
- AI analysis is performed via **Google’s cloud AI** through Firebase AI Logic (**Gemini 3.5 Flash-Lite**), using trimmed sentence-level text.
- We **do not sell** your personal information.
- We **do not use** third-party advertising networks.
- We use **Google Analytics for Firebase** for anonymous usage statistics. We do **not** send message content or coaching text to analytics.
- Most App data stays **on your device**. Subscription status is handled by **Apple App Store / StoreKit**.

---

## 3. Information We Collect

### 3.1 Information You Provide Directly

#### A. Text you type (User Content)

When the Spectrum Sync Keyboard is enabled, Full Access is allowed, disclosure is accepted, and coaching is not paused, the keyboard may access text from the field you are typing in **through the keyboard’s document proxy**, including:

- Message drafts in messaging, email, and social apps (when Spectrum Sync Keyboard is the active keyboard)
- The current sentence or line being composed

This text is used **only** to provide coaching feedback (tone warnings, explanations, and suggested rewrites).

We apply safeguards to **avoid analyzing** text when:

- The field is a secure/password field (`isSecureTextEntry`)
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

#### C. Support communications

If you email us at [hallanhype@gmail.com](mailto:hallanhype@gmail.com), we receive the information you choose to send.

### 3.2 Information Collected Automatically

#### A. Keyboard and field context

The keyboard may use:

- Whether the active field is secure
- Limited document-proxy text needed for sentence detection
- Local counters for cloud AI limits

#### B. Subscription and billing information

Purchases, free trials, and subscription status are processed by **Apple App Store / StoreKit**. Apple may provide us with:

- Whether you have an active subscription or trial entitlement
- Product identifiers (for example `premium_access_monthly`, `premium_access_yearly`)
- Transaction metadata needed to verify premium access

We do **not** receive your full payment card number.

#### C. App usage analytics (Firebase Analytics)

We collect limited, anonymous usage information such as:

- App opens and session counts
- Screen or tab views within the app
- Device model, OS version, and app version
- Whether coaching cloud features were used at least once (`service_enabled`)
- When a trial user reaches the daily coaching limit (`daily_limit_reached`, with trial day 1–7)

**Analytics does not include** the text you type, coaching suggestions, or message content.

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
| **Safety** | Skip secure fields; honor pause and disclosure settings |
| **Operate the App** | Save settings and pause state locally (App Group) |
| **Manage subscriptions** | Verify premium access and free-trial eligibility via the App Store |
| **Limit cloud AI usage** | Enforce daily/hourly caps and cooldowns |
| **Respond to you** | Answer support emails |
| **Legal compliance** | Meet legal obligations |

We do **not** use your typed message content for advertising or sell it to data brokers.

---

## 5. Custom Keyboard and Full Access Disclosure

Spectrum Sync uses a custom **iOS Keyboard Extension**.

### What the keyboard can access

When enabled and Full Access is allowed, it may:

- See text in the active input field via the system document proxy (only while Spectrum Sync Keyboard is selected)
- Use the network to send trimmed sentence text to Google for AI coaching
- Show a coaching pill / panel above the keyboard
- Insert suggested replacement text when you choose a suggestion

### Why Full Access is required

iOS sandboxes keyboard extensions by default. **Allow Full Access** is required for network access so the keyboard can call Firebase AI Logic (Gemini) and related Firebase services. Without Full Access, cloud coaching cannot run.

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

On iOS, analysis uses **Google’s generative AI services** through **Firebase AI Logic**, using **Gemini 3.5 Flash-Lite**. The App may send **only the current sentence or line being analyzed** (trimmed to an internal length limit).

Cloud requests are subject to app-side limits, including approximately:

- **25 cloud coaching requests per day** during the free trial
- **150 cloud coaching requests per day** for active premium subscribers
- Additional hourly, interval, and cooldown limits

AI responses are structured coaching results (status, short warning, reasoning, and suggestions). Choosing a suggestion may replace text in the active field via the keyboard.

We do not routinely have humans read your typed content. Support emails you send us are handled separately.

---

## 7. How We Share Information

| Provider | Purpose | Data involved |
|---------|---------|---------------|
| **Google Firebase / Firebase AI Logic** | Cloud AI inference | Trimmed coaching text, prompts/instructions, technical request metadata |
| **Apple App Store / StoreKit** | Subscriptions, trials, purchase verification | Product IDs, subscription/transaction status |
| **Google Analytics for Firebase** | Anonymous usage analytics | App/session metrics; no message content |

We may disclose information if required by law or to protect rights and safety. We do **not** sell personal information for cross-context behavioral advertising.

---

## 8. Data Retention

| Data type | Retention |
|----------|-----------|
| Local settings (App Group JSON) | Until you change settings, clear app data, or uninstall |
| Coaching text in memory | Only while processing the current request |
| Cloud usage counters | Stored locally; reset per daily/hourly logic |
| App Store purchase records | Retained by Apple under Apple’s policies; we retain local entitlement flags as needed |
| Support emails | As long as needed to respond |

---

## 9. Data Security

We use reasonable measures designed to protect information, including:

- Skipping secure text fields
- Limiting cloud transmission to trimmed sentence-level text
- Using encrypted transport (HTTPS/TLS) for cloud AI requests
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
- Email [hallanhype@gmail.com](mailto:hallanhype@gmail.com?subject=Spectrum%20Sync%20iOS%20Data%20Deletion%20Request) for help with information you sent by email

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
