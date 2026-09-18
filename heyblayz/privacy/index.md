---
layout: heyblayz-legal
title: Privacy policy
description: How HeyBlayz handles your records, Google account and Drive sync, AI inputs, security information, retention and deletion requests.
legal_kind: privacy
---

HeyBlayz is a voice-first fitness and nutrition application developed by **{{ site.data.heyblayz.publisher }}** ("we"). This policy covers HeyBlayz and its website, not the separate LogIt app. For privacy questions or requests, email [{{ site.data.heyblayz.contact_email }}](mailto:{{ site.data.heyblayz.contact_email }}).

Your records are stored on your device. If you connect Google, synchronization uses hidden app-data storage in **your own Google Drive**. AI requests are a separate operation: their inputs and relevant context pass through our proxy to Google Gemini. We do not operate a central database of your synced fitness records, but our infrastructure does retain security and operational information described below.

<div class="contents" markdown="1">

- [Information we process](#information-we-process)
- [Google account and Drive access](#google-account-and-drive-access)
- [AI, search and third-party services](#ai-search-and-third-party-services)
- [Storage, security and retention](#storage-security-and-retention)
- [Your choices and deletion](#your-choices-and-deletion)
- [Your rights and contact](#your-rights-and-contact)

</div>

## Information we process

- **Content you provide:** workout and meal records, sets, repetitions, weights, food and exercise catalogs, measurements, goals, notes, selected photos, voice inputs, conversations and remembered preferences. Profile details can include age, sex, height, weight, nutrition targets and a city you enter. This content can reveal health-related information.
- **App-generated content:** AI responses, proposed or accepted actions, conversation summaries, quiz progress, reminders, event-search results, record changes and sync conflict history.
- **Google account information:** Google Sign-In provides an account identifier and email, and can return basic profile information such as a name or profile image. HeyBlayz uses the identifier to separate account databases and the email to identify the connected account. Native Google sign-in software manages authorization credentials; they are not included in record sync or sent to the AI proxy.
- **Security and technical information:** a generated device identifier, app identity, App Attest verification information, public verification keys, request counters and timestamps. Hosting and service providers also process connection and diagnostic information, which can include IP addresses, request metadata and error details.
- **Support correspondence:** information you choose to email us. Do not send passwords, authorization tokens or unnecessary health information.

Microphone, camera, photo-selection and notification access are used for the features you invoke, subject to your device permissions. A city entered for nearby-event searches can be sent as search context. HeyBlayz does not require access to your Google contacts, Gmail or ordinary Drive documents for synchronization.

## Google account and Drive access

Google sign-in and sync are optional when starting with local data. Connecting an account requires your authorization. The Drive permission is `https://www.googleapis.com/auth/drive.appdata`: it allows access to this app's hidden application-data storage, not general access to your Drive files.

The app uploads and downloads saved content and change history to synchronize your records, catalogs, preferences, goals, measurements, conversations and attached images, memories and summaries, reminders, quizzes, saved text requests and app-generated caches. Device security credentials and device-specific notification permission choices are excluded. Changes and deletions are merged rather than replacing the entire database. Different Google accounts use separate local databases and Drive storage; there is no cross-account sync. Copying existing local records into the first connected account requires your confirmation.

Sync runs on opening or returning to the app and through **Sync now**. The app shows status and errors. Access is used to provide these user-facing functions, not to inspect unrelated Google data. The hidden folder is not a normal folder you browse in Drive; see [Google's application-data documentation](https://developers.google.com/workspace/drive/api/guides/appdata).

### Google data use commitments

We follow the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including its Limited Use requirements. We do not sell Google user data, use it for advertising or credit decisions, or use it to train general-purpose AI models. Transfers are limited to providing the features you request, security needs, legal obligations, or another use requiring your separate consent. Human access is limited to information you choose to provide for support, authorized troubleshooting, necessary security investigations or legal requirements.

Records restored from Drive remain your app records. When you use Blayz, relevant records can be included in AI context as described below; Google sign-in alone does not send your Drive library to Gemini.

## AI, search and third-party services

**Blayz and Google Gemini:** submitted text, recordings, images, recent conversation context, stored summaries and remembered facts can be sent through our proxy to Google's hosted Gemini service. Requested tools can supply relevant records, goals, profile information or catalog entries. Conversation summarization also uses Gemini. This processing supplies answers, extraction, suggestions and actions within the app; it is not limited to the words in your latest message. Avoid including sensitive information that is unnecessary for your request.

**Search:** web-search and nearby-event features can send queries and relevant location context to Google's search-grounded AI services. Following a source or other external link opens a third-party service with its own privacy practices.

**Other providers:** Google provides sign-in, Drive storage and cloud processing; Apple provides iPhone permissions, device security and notification infrastructure; GitHub hosts this website. They may process information in countries other than your own. We do not promise that all processing stays in a particular country or that providers have zero retention. See [Google's privacy policy](https://policies.google.com/privacy), [Google Cloud's AI data-governance documentation](https://cloud.google.com/vertex-ai/generative-ai/docs/data-governance), [Apple's privacy policy](https://www.apple.com/legal/privacy/), and [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

This website adds no analytics scripts, advertising or tracking cookies of its own. GitHub can still process information needed to serve and secure the site.

## Storage, security and retention

- **Local records:** app databases, conversation archives and account-specific copies remain on the device until removed. Signing out hides the account's records from the signed-out app but does not erase its local database. Device backups may retain copies separately.
- **Drive sync:** records and change batches remain in your app-data storage until that data is removed. The current sync journal has no automatic age-based purge. Deleting a record removes it from the active view and synchronizes a deletion marker, but earlier values and conflict versions can remain in local and Drive change history. Retiring a memory or clearing the current conversation is not a complete erasure of all copies and summaries.
- **AI proxy:** it forwards requests rather than maintaining a database of your conversations or fitness records. Security state is stored separately. Current application expiry settings are five minutes for attestation challenges, two days for daily rate-limit counters, and one year for device-verification records, renewed when verification state is updated. Expiry is not a promise of immediate physical deletion from provider backups or logs.
- **Operational logs and support:** infrastructure logs can contain connection metadata and error details, including portions of provider errors. They are governed by the configured hosting-provider retention, which is separate from the application expiry settings above. Support correspondence is kept as needed to address your request, security issues and applicable obligations. Contact us for the information or deletion available for your case.

Network requests use HTTPS. Native platform mechanisms protect sign-in and device credentials; we do not claim end-to-end encryption of sync records or AI requests. No storage or transmission system can guarantee absolute security.

## Your choices and deletion

You can edit or delete active records in the app, manage remembered facts and reminders, and change device permissions in system settings. Export functions cover the data types offered in the app; they are not a guarantee of a complete export of every internal sync version.

**To stop Google access:** sign out in HeyBlayz and remove its authorization in [Google Account connections](https://myaccount.google.com/connections). Removing access prevents future authorized access but does not itself delete app data already stored. See [Google's instructions](https://support.google.com/accounts/answer/13533235).

**To remove cloud and device copies:** first stop sync on all connected devices and revoke access. Use Google Drive's app-management controls to delete HeyBlayz's hidden app data. Remove the local app data from each device as well; on iPhone, deleting the app is different from offloading it, which keeps data. Manage device or cloud backups separately. Retained local copies or later edits can reintroduce data if you reconnect them, so do not reconnect a copy you intended to erase. These steps do not automatically delete separate provider logs or support correspondence.

For assistance with full deletion, security records, summaries or retained history, contact [{{ site.data.heyblayz.contact_email }}](mailto:{{ site.data.heyblayz.contact_email }}). We may need proportionate information to identify the relevant data, but will not ask for your password or access tokens. We cannot directly erase your private Drive storage without your authorization.

## Your rights and contact

We process information to provide the functions you request, with your authorization for optional connected services and device permissions, and to protect the service from abuse. Where applicable, the legal bases include performing our agreement with you, consent for optional processing, legitimate interests in security and reliability, and compliance with legal obligations. Health-related information may require additional protection or consent under your local law; do not provide information you do not want processed for the requested features.

Depending on your location, you may have rights to access, correction, deletion, restriction, objection and portability, and to withdraw consent. Withdrawing consent does not undo processing already lawfully performed. You may also complain to your local data-protection authority. Contact **{{ site.data.heyblayz.publisher }}** at [{{ site.data.heyblayz.contact_email }}](mailto:{{ site.data.heyblayz.contact_email }}) to exercise your rights or ask about international processing and retention. Some information may need to be retained for legal or security reasons; we will explain relevant limitations in response to your request.

HeyBlayz is not designed for use by children. If you believe a child has provided personal information, contact us so we can assess and address it.

We will date policy updates on this page. Material new uses of Google data require notice and, where required, renewed consent before that new use. See also the [HeyBlayz terms of service](../terms/).
