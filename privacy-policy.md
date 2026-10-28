---
title: Dozelight — Privacy Policy
permalink: /privacy-policy
---

<!--
  Approved by the owners for publishing on 2026-10-27. A lawyer's review (KVKK and GDPR: sleep
  as health-related data, explicit consent, transfers abroad) is still to come; the "Lawyer
  review" notes below are its checklist. Keep this in sync with the app: section 3's shared
  fields must match ecosystemAccount.shareConsent and the SharedNight contract
  (packages/ecosystem/src/sharedNights.ts), and section 8 src/crashReporting/. Updated on
  2026-10-28 for Plus on sale: no ads, no Plus day. Publish it with the release that sells Plus.
-->

# Privacy Policy

**Effective date:** 2026-10-28

Dozelight ("the app") is provided by **Noronaru** ("we", "us"). Noronaru is the data controller for the personal data described in this policy. You can reach us at **noronaru@proton.me**.

## In short

- Your sleep log — nights, ratings, tags, notes, naps and what the app reads from Health Connect — is stored **on your phone**. We do not upload it.
- Signing in with Google is **optional**. You need it to connect Dozelight with our Hydrorep and InnerWeather apps, and for Plus.
- If you turn on **Share with my other apps**, a **summary of each night** is stored in your account in the European Union, for our other apps to read. Your notes, your own tags, sleep stages and body measurements stay on your phone.
- If crash reporting is on, an **anonymous crash report** can be sent when the app crashes. It never contains your sleep data, and you can turn it off in Settings.
- There are **no ads, no analytics and no tracking**, and we do not sell your data.
- Dozelight is **not a medical service**.

## 1. Information that stays on your phone

The following is stored only in the app's storage on your phone:

- Your nights: bed and wake times, how well you slept, tags, notes, caffeine and naps
- Tags you create, your sleep goal, reminder times, your language and other app preferences
- Data the app reads from **Health Connect** with your permission (section 2)
- Small records the app needs, such as whether you have finished onboarding and which milestones you have reached

We have no access to this information. Android's backup to your Google account does not include Dozelight's data, so to keep your nights when you change phones, use **Export** in **Settings → Your data**. Uninstalling the app, clearing its data, or **Settings → Your data → Delete all data** deletes it from your phone.

**Exporting your data.** When you export your nights as JSON or CSV, the app creates a file and opens your phone's share menu. Where the file goes is your choice, and that service's own privacy terms apply to it.

**Your other apps.** To show our other apps in its app bar, Dozelight asks Android whether Hydrorep and InnerWeather are installed on your phone. The answer stays on your phone.

## 2. Health Connect

With your permission, Dozelight **reads** from Health Connect your sleep sessions and sleep stages and, only if you turn on **Show body metrics from Health** in **Settings → Health & wearables**, your heart rate, blood oxygen and body temperature during sleep, when a watch or ring has written them. Dozelight never writes to Health Connect.

It uses this data to fill in your nights and show your sleep in the app. Sleep stages, heart rate, blood oxygen and body temperature never leave your phone. The bed and wake times and how long you slept become part of your night, so if you turn on **Share with my other apps** (section 3), they are shared like those of any other night.

Dozelight's use of information received from Health Connect adheres to the [Health Connect Permissions policy](https://support.google.com/googleplay/android-developer/answer/12991134), including its Limited Use requirements. Health Connect data is never sold, never used for advertising, and never used for anything other than the features described here.

## 3. Google sign-in and your other apps (optional)

Hydrorep is our workout tracker, with its own [privacy policy](https://noronaru.github.io/hydrorep-legal/privacy-policy), and InnerWeather is our mood journal, with its own [privacy policy](https://noronaru.github.io/innerweather-legal/privacy-policy). If you use them with the same Google account, Dozelight can show your sleep next to your training and mood.

**Signing in with Google.** Sign-in is handled by Firebase Authentication, a Google service. When you sign in, it receives your Google account's email address, name and a unique account identifier. To protect sign-in from abuse, it also processes your IP address and information about your phone. We use this only to identify your account, to connect Dozelight with our other apps and for Plus. Signing in to them with the same Google account gives you **one account for all three**, so deleting it in any of them deletes it for all (section 13).

**What is shared, and only after you agree.** Nothing is shared until you turn on **Share with my other apps** in **Settings → Connected apps** and confirm it. From then on, starting with the last 90 days, Dozelight stores for each night you log:

- the date
- how well you slept (a rating from 0 to 4) and how long
- your bed and wake times
- which of the five built-in tags you picked (late caffeine, stressed, alcohol, screen before bed, napped)
- your last caffeine time
- the day's nap minutes

This summary is stored in Google Cloud Firestore, in the European Union, under your account. Security rules allow only your signed-in account to read or change it, and our Hydrorep and InnerWeather apps read it when you are signed in there with the same account. **Not shared:** your notes, tags you created, sleep stages, heart rate, blood oxygen and body temperature.

**How our other apps use your nights.** Hydrorep and InnerWeather show them next to your training and mood. Their AI features — InnerWeather's AI insights and Hydrorep's AI coach — can include your nights only if you turn that on in those apps; the nights are then sent to **Anthropic** in the United States, as their privacy policies describe.

**What Dozelight reads.** When you are signed in, Dozelight reads what you chose to share from our other apps: InnerWeather's daily mood score, and Hydrorep's daily training summary (the number of workouts, training time, average difficulty and when the last workout finished). It shows them on a night's "The day after", in **Cross-app insights** (from Trends) and in the **Your apps** sheet, and with Plus uses them for more comparisons and for today's recovery. Dozelight reads them from your account when it needs them and does not keep them.

**Stopping.** You can turn sharing off at any time in **Settings → Connected apps**, and sign out from your account at the top of **Settings**. Dozelight then stops sending summaries and deletes the ones it shared from your account. Turning sharing off needs a connection and stays on when it fails; signing out without a connection leaves the summaries there until you delete your account (section 13).

Because sleep data can be considered health-related data, we share it only with your explicit consent, which you give when you turn sharing on and can withdraw at any time.

<!-- Lawyer review: confirm the in-app sharing consent satisfies KVKK explicit consent
     requirements for health-related data and for transferring it abroad. -->

## 4. Plus

Plus is one subscription for Dozelight, Hydrorep and InnerWeather, sold through **Google Play**, which handles payment; we never see your payment details. It belongs to your Google account, so buying it needs Google sign-in.

To check and restore Plus in all three apps, the apps and our server use **RevenueCat** (United States). While you are signed in, RevenueCat receives your account's identifier, your purchases and subscription status from Google Play (such as the product, price and dates), and basic information about your phone and the app, such as the Android version, app version, country and IP address. Dozelight does not contact RevenueCat while you are signed out. Learn more in [RevenueCat's privacy policy](https://www.revenuecat.com/privacy).

## 5. Our server

When you delete your account, Dozelight asks our server — on Google Cloud in the United States, the same server that runs our other apps' AI features — to delete what it keeps on your account: your subscription record at RevenueCat and the usage counts of those AI features. The request carries your account's identifier. Dozelight sends nothing else to our server.

## 6. No ads

Dozelight shows no ads and contains no advertising SDK; it does not use your phone's advertising ID.

## 7. Reminders and sleep sounds

Reminders are scheduled on your phone, and sleep sounds play from files inside the app. We do not operate a notification or streaming server.

## 8. Crash reports

To find and fix crashes, Dozelight can use **Sentry**. When the app crashes, it sends a report with the error, the app version and basic information about your phone (such as its model and Android version). Reports are configured not to include personal data, and they **never include your sleep data**, notes or account. Crash reporting is on by default; you can turn it off at any time in **Settings → Privacy → Share crash reports**.

## 9. What we do not do

Dozelight contains no analytics, does not track you across other apps or websites, and we do not sell your personal data.

## 10. Children

Dozelight is not directed at children under 13, and we do not knowingly collect personal data from them. If you are under 18, please use the app only with permission from a parent or guardian.

## 11. Where your data is processed

- **European Union:** the night summaries you share, and what you read from our other apps (Google Cloud Firestore).
- **United States:** Google sign-in (Firebase Authentication), our server (Google Cloud), purchases (RevenueCat) and crash reports (Sentry).

If you live in Türkiye, the European Union or another country, this means some of your data is transferred abroad. We rely on the safeguards the law requires for these transfers.

<!-- Lawyer review: name the transfer mechanism for each provider - KVKK art. 9 as amended in
     2024 and GDPR chapter V - and whether the EU storage needs one, given Firebase is a US
     company. -->

## 12. Legal bases

<!-- Lawyer review: confirm each basis under both KVKK (arts. 5 and 6) and GDPR (arts. 6 and 9). -->

- **Your explicit consent** for sharing your nights with our other apps. Sleep can reveal information about your health, so it is only shared after you agree in the app. You can withdraw your consent at any time by turning sharing off.
- **Providing the service you ask for** (our contract with you) for Google sign-in, Plus and deleting your account.
- **Our legitimate interests** in keeping the app working and secure: crash reports, which you can turn off.

## 13. Your rights

Depending on where you live — including under the Turkish Personal Data Protection Law (KVKK) and the EU General Data Protection Regulation (GDPR) — you may have the right to access, correct or delete your personal data, to receive a copy in a portable format, to object to or restrict its processing, and to withdraw consent at any time.

- **Data on your phone:** you can edit or delete nights in the app, export them, use **Settings → Your data → Delete all data**, or uninstall the app.
- **Your account and shared summaries:** in Dozelight, tap your account at the top of **Settings**, then **Delete account**. This deletes your sign-in account and every shared night right away, and asks our server to delete what it keeps on your account (section 5). Because Dozelight, Hydrorep and InnerWeather share one account, it also deletes what those apps keep in your account, such as InnerWeather's cloud backup of your journal. It does not cancel a subscription in Google Play. Your nights stay on your phone.
- **Without the app:** email **noronaru@proton.me** from the address of your Google account and ask us to delete your account. We will delete your sign-in account, everything stored under it and any related purchase record held by RevenueCat within 30 days. Purchases themselves stay on record with Google Play under its own terms. Step-by-step instructions: [Delete your account](./delete-account).

For any other request or question, write to **noronaru@proton.me**. We will answer within 30 days. You also have the right to lodge a complaint with a data protection authority — in Türkiye, the Personal Data Protection Authority (KVKK); in the EU, the authority where you live or work.

## 14. How long we keep data

- **On your phone:** until you delete it.
- **Shared night summaries:** until you turn sharing off, sign out, or delete your account.
- **Your Google account:** until you delete your account.
- **Crash reports:** deleted by Sentry after its retention period, at most 90 days.

## 15. Security

Data sent from the app is encrypted in transit (HTTPS). Access to our database is restricted by security rules and to our own administrative accounts.

## 16. Not a medical service

Dozelight does not diagnose, treat or prevent any condition and does not provide medical advice. If you have ongoing trouble sleeping, talk to a doctor.

## 17. Changes to this policy

When we update this policy, we change the effective date above. If a change affects how your data is used, the app will let you know.

## 18. Contact

Noronaru — **noronaru@proton.me**
