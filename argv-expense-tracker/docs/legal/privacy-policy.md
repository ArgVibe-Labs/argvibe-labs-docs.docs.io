# Product release checklist

Do not add or delete checklist items without confirming with the app owner first. Keep the release target fixed unless the app owner approves a change.

Check an item only after it has been verified for this release. Keep release-specific work here; use the Privacy Policy, Terms, and implementation docs for details.

## Release 1.0.0+1 — Android MVP (Preparing)

### Implemented

- [x] Local guest and Google profiles with separate data.
- [x] Expense and income tracking, budgets, categories, and insights.
- [x] Google Drive profile backup, history, restore, and optional automatic backup.
- [x] Require an 18+ self-confirmation before guest or Google sign-in; store only a device-local confirmation.
- [x] Provide in-app deletion of a guest or Google profile and its local receipt photos, with an option to delete that Google profile's Drive backups.
- [x] Add Android and iOS launcher icons and use the same artwork in the login and dashboard brand mark; provide an Android adaptive icon for circular launchers.
- [x] Draft the Privacy Policy and Terms of Service for ArgVibe Labs LLP and make both readable from the guest and Google sign-in screens.

### Completed reviews

- [x] Compare the current Privacy Policy and Terms against the checked-in app flows and dependency lockfile. They cover local records, Google Sign-In, receipt photos and on-device ML Kit, Drive snapshots, device backups, sharing, security, retention, and deletion.
- [x] Verify in code that the 18+ and legal agreement boxes start unchecked, block Continue until selected, and open the bundled Terms and Privacy Policy.
- [x] Check the current dependency lockfile and source for ads, Firebase, Crashlytics, and developer analytics packages; none are present.
- [x] Check the current India DPDP commencement schedule: the main obligations and Rule 14 of the 2025 Rules are scheduled for 13 May 2027; Rule 14 provides for a published grievance period not exceeding 90 days. See the [official commencement notification](https://egazette.gov.in/WriteReadData/2025/267647.pdf) and [2025 Rules](https://www.meity.gov.in/static/uploads/2025/11/53450e6e5dc0bfa85ebd78686cadad39.pdf).

### Must finish before publishing on Google Play

#### App and release build

- [ ] Set the final Android application ID and store-facing app identity. Replace debug signing with production signing and build a signed Android App Bundle.
- [ ] Configure the production Google OAuth consent screen and clients, register the release and Play app-signing fingerprints, and confirm Google Sign-In and Drive access in the release build. The app requests the non-sensitive `drive.appdata` scope; confirm the production OAuth app is ready for public users.
- [ ] Run the automated tests and a release-build smoke test on supported Android devices: guest and Google entry, adding and deleting records, receipt capture, backup and restore, profile and Drive-backup deletion, and launcher icon.

#### Privacy, legal, and support

- [ ] Publish a working public Privacy Policy URL. Check the final policy against the Android build, including Google Sign-In, Drive, ML Kit, device backups, deletion, and any SDK data transmission. Local-only app data does not by itself mean "no data collected" in Play's Data safety form.
- [ ] Fix the in-app Terms-to-Privacy Policy cross-reference or clearly direct users to the separate legal-document links. Test both documents and the 18+ and agreement flow in the release build.
- [ ] Confirm the Terms match the launch price and actual backup, restore, export, and deletion behavior. Have ArgVibe Labs LLP approve the liability and venue clauses before publishing them.
- [ ] Confirm that contact@argvibe.com works and assign someone to handle support, privacy requests, and reports of security incidents. Provide any third-party license notices required by the shipped dependencies.
- [ ] Review privacy and consumer-law requirements for the countries where the Android app will actually be available, including a fresh check of India's DPDP commencement schedule. Because the intended availability is global, resolve any applicable EU/UK representation and other material launch requirements before enabling those countries. Keep the published policy's security description accurate; app-level encryption is a separate product decision.

#### Play Console

- [ ] Complete the store listing and Play declarations: Data safety and data deletion, target audience (18+), ads, app access, content rating, Financial features, and developer contact details. Answer the Financial features form based on the app's actual features.
- [ ] Resolve whether the Google-linked profile counts as an app account under Play's account-deletion policy. If it does, publish the required deletion-request web page and enter its URL in Play Console; explain that device-local data must be deleted on the device and that users can remove Drive backups in the app or their Google account.
- [ ] Confirm the signed bundle meets current Play submission requirements, then submit it for review.

### After the MVP, or only if the scope changes

- Prepare iOS signing, Google OAuth URL scheme, App Store privacy information, and applicable Apple login rules before an iOS release.
- Add renewed acceptance and version/time records if a later legal-document change requires fresh consent; retain the published versions needed to explain what users saw.
- Revisit child-directed rules if the target audience changes to include minors. Revisit data disclosures and security decisions whenever SDKs or data flows change.
