# SpendCanvas Privacy Policy

**Effective date:** 15 October 2026  
**App:** SpendCanvas  
**Developer:** ArgVibe Labs LLP  
**Privacy and grievance contact:** contact@argvibe.com

SpendCanvas is an expense and income tracker. You can use it as a guest on your device or sign in with Google. Google sign-in enables a separate local profile and optional backup and restore through your Google Drive. SpendCanvas does not operate its own account or financial-data server.

## Information the app uses

- **Financial records and settings.** The app stores the expenses, income, amounts, dates, descriptions, categories, recurring entries, budgets, currency, display name, and other preferences you enter in a local database on your device. Guest and Google profiles are kept separate in that database.
- **Google account details.** If you sign in with Google, the app receives and stores your Google account ID, email address, display name, and profile photo URL to identify and show your profile. Google handles authentication; SpendCanvas does not receive your Google password.
- **Receipt photos and scanned text.** If you choose to use a receipt, the app accesses a photo from your camera or photo library, lets you crop it, and saves the cropped image in app storage on your device. Google ML Kit reads the image on the device to suggest a merchant, amount, or date. You can review or change those suggestions before saving an expense. The app does not include receipt image files or their local file paths in its own Google Drive profile snapshots.
- **Age and consent choices.** The app stores a device-local flag recording that you confirmed you are 18 or older. It does not ask for or store your date of birth or an identity document. It also stores the Google profile's acceptance of the sign-in terms locally; this acceptance is not included in Drive snapshots.
- **Technical data from ML Kit.** Google says ML Kit may collect device and app information, identifiers, performance and usage metrics, configuration details, and error codes for diagnostics and service improvement. Google says receipt image input and recognized text are processed on the device and are not sent to its servers by ML Kit. See [Google's ML Kit privacy information](https://developers.google.com/ml-kit/terms) and [Android data disclosure guidance](https://developers.google.com/ml-kit/android-data-disclosure).

## How information is used

SpendCanvas uses your information to show your accounts and reports, keep guest and Google profiles separate, display your profile, read receipt details at your request, and perform the backup and restore actions you select. The app does not contain an advertising SDK or a developer-operated analytics service. ArgVibe Labs LLP does not sell personal information or share it for cross-context behavioral advertising. Information obtained through Google APIs is used for the sign-in and Drive features described here, in accordance with the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including its Limited Use requirements. It is not used for advertising, lending, or creditworthiness decisions.

Google Sign-In and Google Play services may exchange account, device, and technical information with Google when those services are used. Google's handling of that information is described in its [Privacy Policy](https://policies.google.com/privacy).

## Google Drive backups

Google Drive access is optional and uses the `drive.appdata` permission for SpendCanvas's hidden application-data folder in your Google account. The app may request this permission when you open backup history, enable automatic backup, or use backup or restore. A signed-in account with an empty local profile may also be offered an existing backup to restore. Manual uploads occur when you choose **Back up now**; automatic uploads occur only if you enable automatic backup. Automatic backup runs while the app is active, rather than as a guaranteed background service.

A snapshot contains the selected profile's financial records and settings, including a custom display name, plus a Google account ID and backup metadata such as creation time and format version. It does not contain receipt image files, local receipt paths, Google email address, Google profile photo URL, or Google terms acceptance. Snapshots travel directly from the app to Google's Drive API over HTTPS and are stored in your account's hidden app-data folder. They are not stored on a SpendCanvas server. Google processes this information under its [Privacy Policy](https://policies.google.com/privacy). The folder is not shown in the normal Drive file list, but it is accessible to SpendCanvas after you authorize it and can be removed through the app or your Google account settings. See [Google's description of Drive app data](https://developers.google.com/workspace/drive/api/guides/appdata).

The app keeps separate manual and automatic snapshots. After a successful automatic backup, it tries to remove older redundant automatic snapshots according to your selected three- or six-month retention setting while protecting the latest snapshot. Cleanup may be delayed if Drive is unavailable. Manual snapshots are not removed by that automatic cleanup; they remain until you delete them in backup history, delete all app backups with your profile, or remove the app's Drive data from your Google account. A backup is a snapshot, not live synchronization between devices. Restoring one replaces that profile's local financial records and settings.

## Device system backups

Android may separately back up or transfer app data according to your device and Google backup settings. On iPhone, iCloud or a computer backup may also include app data. These operating-system features are distinct from SpendCanvas's optional Drive snapshot feature and may include the app's local database and receipt images. SpendCanvas's receipt exclusion applies to its own Drive snapshots only. System backup retention and deletion are controlled by your device and backup provider, not by the in-app backup history. See [Android's Auto Backup information](https://developer.android.com/identity/data/autobackup) and [Apple's iCloud Backup information](https://support.apple.com/en-gb/108770).

## Storage, security, and sharing

Local records and receipt images are stored in the app's device storage, subject to the device's security and backup settings. The app uses HTTPS for its direct Google Drive requests. It does not add its own end-to-end encryption to the local database or to Drive snapshots. Protect access to your device and Google account if you use these features.

Camera and photo-library access is used when you choose to add a receipt. Where your device requests permission, you can decline it or change it later in device settings. Only add receipts that you have the right to use; they may contain information about other people.

The app shares data with Google when you choose Google sign-in or Drive features, and the ML Kit SDK may send the technical metrics described above to Google. Your device's operating system or backup provider may also process app data when system backup or device transfer is enabled. SpendCanvas does not send your financial records to an advertiser or a developer-operated server. Google and your device provider may process data in other countries under their own policies.

## Your choices and deletion

You can use SpendCanvas as a guest without Google sign-in. You can edit or delete individual records in the app, turn automatic Drive backup off, and review or delete eligible snapshots in **Profile → Backup & restore**. You can remove a profile from **Profile → Delete profile and data**. That action removes the profile's local records, settings, and receipt files from the device. For a Google profile, you can choose to delete its SpendCanvas Drive snapshots as part of the same flow or leave them in your Google Drive for a later restore. The app reports an error if a requested Drive deletion cannot be completed, rather than treating the profile as fully deleted.

Local data normally remains until you delete the profile, clear the app's data, or uninstall the app. Uninstalling the app does not by itself delete its snapshots from your Google Drive. Device system backup copies may remain under your device or backup-account settings even after in-app deletion. Google and Apple may retain information according to their own policies.

Depending on where you live, applicable law may give you rights to access, correct, delete, obtain a copy of, restrict, or object to processing of your personal information; withdraw consent where processing relies on it; nominate another person to exercise rights; and raise a privacy grievance or complaint with a regulator. You can exercise many of these choices by editing or deleting data in the app, managing Drive backups, or stopping use of optional features. You may also email **contact@argvibe.com** with a request or grievance. Because SpendCanvas does not keep your financial records on a developer-operated server, we cannot retrieve local records or Drive snapshots that we do not hold. We will respond to requests within the time required by applicable law and may need enough information to verify the request. For information held by Google, Apple, or your device backup provider, contact that provider or use its account controls.

Where laws require a legal basis for processing, we use the information needed to provide the app features you request and rely on your choice to use optional Google sign-in, Drive backup, and receipt features where consent is required. You can stop using those optional features and delete associated data as described above. Google and device-backup providers may process information in countries outside your own under their respective policies. If we learn of a data incident affecting information we handle, we will notify affected people and authorities where required by applicable law.

## Children

SpendCanvas is intended for people aged 18 or older. The app asks for an 18+ self-confirmation before guest or Google sign-in; it does not verify age or collect a date of birth. The app is not directed to children. If you are under 18, do not use the app. If we learn that a user is under 18, we will ask them to stop using it and delete their profile and any Drive snapshots using the controls above.

## Changes to this policy

If SpendCanvas's data practices change, we will update this policy and its effective date. We will provide notice of material changes in the app or through another appropriate channel before they take effect where required by law. The current policy is available in the app; a public version will be linked from the store listing when published.

## Contact

For privacy questions, rights requests, or grievances, contact **contact@argvibe.com**. The developer is **ArgVibe Labs LLP**.
