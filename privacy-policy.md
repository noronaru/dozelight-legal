---
title: Dozelight — Privacy Policy
permalink: /privacy-policy
---

<!--
  DRAFT — have a lawyer review this before the public release, especially the KVKK (Turkish
  Personal Data Protection Law) sections on health-related data, explicit consent and
  transfers abroad. Keep it in sync with the app: the shared fields in section 2 must match
  ecosystemAccount.shareConsent and the SharedNight contract (packages/ecosystem/src/
  sharedNights.ts); crash reporting in section 4 must match src/crashReporting/.
-->

# Privacy Policy

**Effective date:** 2026-10-24

Dozelight ("the app") is provided by **Noronaru** ("we", "us"). Noronaru is the data controller for the personal data described in this policy. You can reach us at **noronaru@proton.me**.

## In short

- Your sleep log — nights, ratings, tags, notes, naps and what the app reads from Health Connect — is stored **on your device**. We do not upload it.
- Signing in with Google is **optional**. You only need it to connect Dozelight with our Hydrorep and InnerWeather apps.
- If you turn on "Share with my other apps", only a **summary of each night** is stored in our cloud database in the European Union. Your notes, your own tags, sleep stages and body measurements stay on your device.
- If the app crashes, an **anonymous crash report** is sent so we can fix it. You can turn this off in Settings. It never contains your sleep data.
- There are **no ads, no analytics and no tracking** in Dozelight, and we do not sell your data.
- Dozelight is **not a medical service**.

## 1. Information that stays on your device

The following is stored only in the app's storage on your device:

- Your nights: bed and wake times, how well you slept, tags, notes, caffeine and naps
- Tags you create, your sleep goal, reminder times and app preferences
- Data the app reads from **Health Connect** with your permission: sleep sessions and sleep stages, and — when a watch or ring has written them — heart rate, blood oxygen and body temperature during sleep. Dozelight only reads this data and never writes to Health Connect.

We have no access to this information. Uninstalling the app, clearing its data, or **Settings → Your data → Delete all data** deletes it from your device.

**Exporting your data.** When you export your nights as JSON or CSV, the app creates a file and opens your device's share menu. Where the file goes is your choice, and that service's own privacy terms apply to it.

**Health Connect.** Dozelight's use of information received from Health Connect adheres to the [Health Connect Permissions policy](https://support.google.com/googleplay/android-developer/answer/12991134), including its Limited Use requirements. Health Connect data is used only to show your sleep in the app. It is never uploaded, shared, sold, or used for advertising.

## 2. Optional: Google sign-in and sharing with your other apps

Hydrorep is our workout tracker, with its own [privacy policy](https://noronaru.github.io/hydrorep-legal/privacy-policy), and InnerWeather is our mood journal, with its own [privacy policy](https://noronaru.github.io/innerweather-legal/privacy-policy). If you use them with the same Google account, Dozelight can show your sleep next to your training and mood.

**Signing in with Google.** Sign-in is handled by Firebase Authentication, a Google service. When you sign in, it receives your Google account's email address, name and a unique account identifier. To protect sign-in from abuse, it also processes your IP address and information about your device. We use this only to identify your account and to connect Dozelight with our other apps. Signing in to them with the same Google account gives you **one account for all three**, so deleting it in any of them deletes it for all (see section 8).

**What is shared, and only after you agree.** Nothing is shared until you turn on "Share with my other apps" in **Settings → Account** and confirm it. From then on, starting with the last 90 days, Dozelight stores for each night you log:

- the date
- how well you slept (a rating from 0 to 4) and how long
- your bed and wake times
- which of the five built-in tags you picked (late caffeine, stressed, alcohol, screen before bed, napped)
- your last caffeine time
- the day's nap minutes

This summary is stored in Google Cloud Firestore, in the European Union, under your account. Security rules allow only your signed-in account to read or change it, and our Hydrorep and InnerWeather apps read it when you are signed in there with the same account. **Not shared:** your notes, tags you created, sleep stages, heart rate, blood oxygen and body temperature.

**What Dozelight reads.** When you are signed in, Dozelight reads what you chose to share from our other apps — InnerWeather's daily mood and Hydrorep's daily training summary — to show them on a night's "The day after" view. It reads them from your account and does not store them on our servers again.

**Stopping.** You can turn sharing off or sign out at any time in Settings → Account. Dozelight then stops sending summaries and deletes the ones it shared from your account (signing out without a connection leaves them there until you delete your account, see section 8).

Because sleep data can be considered health-related data, we share it only with your explicit consent, which you give when you turn sharing on and can withdraw at any time.

<!-- Lawyer review: confirm the in-app sharing consent satisfies KVKK explicit consent
     requirements for health-related data and for transferring it abroad. -->

## 3. Purchases

If Dozelight offers optional in-app purchases, they are processed by Google Play. We never receive your card or payment details. To confirm which purchases belong to you, we use **RevenueCat**, a service provider that receives your purchase history and an app user identifier.

## 4. Crash reports

To find and fix crashes, Dozelight uses **Sentry**. When the app crashes, it sends a report with the error, the app version and basic device information (such as the device model and Android version). Reports are configured not to include personal data, and they **never include your sleep data**, notes or account. Crash reporting is on by default; you can turn it off at any time in **Settings → Privacy → Share crash reports**.

## 5. Reminders and sleep sounds

Reminders are scheduled on your device, and sleep sounds play from files inside the app. We do not operate a notification or streaming server.

## 6. What we do not do

Dozelight shows no ads, contains no analytics or advertising SDKs, does not use your advertising ID, does not track you across other apps or websites, and we do not sell your personal data.

## 7. Children

Dozelight is not directed at children under 13, and we do not knowingly collect personal data from them. If you are under 18, please use the app only with permission from a parent or guardian.

## 8. Your rights

Depending on where you live — including under the Turkish Personal Data Protection Law (KVKK) and the EU General Data Protection Regulation (GDPR) — you may have the right to access, correct, or delete your personal data, to object to or restrict its processing, and to withdraw consent.

- **Data on your device:** you can edit or delete nights in the app, use **Settings → Your data → Delete all data**, or uninstall the app.
- **Your account and shared summaries:** in Dozelight, go to **Settings → Account → Delete account**. This deletes your sign-in account and every shared night right away. Because Dozelight, Hydrorep and InnerWeather share one account, it also deletes what those apps keep in your account, such as InnerWeather's cloud backup of your journal. Your nights stay on your device.
- **Without the app:** email **noronaru@proton.me** from the address of your Google account and ask us to delete your account. We will delete your sign-in account, everything stored under it and any related purchase record held by RevenueCat within 30 days. Purchases themselves stay on record with Google Play under its own terms. Step-by-step instructions: [Delete your account](./delete-account).

For any other request or question, contact **noronaru@proton.me**.

## 9. Transfers outside your country

Shared night summaries are stored in the European Union. Firebase Authentication (Google), Sentry and RevenueCat may process data in the **United States** and other countries where they operate. If you live in Türkiye or another country outside these regions, this means your data is transferred abroad when you sign in, share summaries, send a crash report or make a purchase.

## 10. Security

Data sent from the app is encrypted in transit (HTTPS). Access to our database is restricted by security rules and to our own administrative accounts.

## 11. Not a medical service

Dozelight does not diagnose, treat or prevent any condition and does not provide medical advice. If you have ongoing trouble sleeping, talk to a doctor.

## 12. Changes to this policy

When we update this policy, we change the effective date above. If a change affects how your data is used, the app will let you know.

## 13. Contact

Noronaru — **noronaru@proton.me**
