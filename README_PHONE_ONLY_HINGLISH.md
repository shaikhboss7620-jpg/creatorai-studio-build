# CreatorAI Studio — Cloud APK build (phone-only instructions)

Important: this is a free cloud-build attempt, not a prebuilt or tested APK. The APK only contains the existing basic dashboard. It does NOT yet generate AI videos, automatically edit videos, upload/schedule YouTube videos, or connect channel analytics.

## Files
- `CreatorAI_Studio_Android_Source.zip` — the Android source project.
- `build-apk.yml` — GitHub Actions workflow text. You will create a workflow file in your GitHub repository and paste this text.

## Phone-only steps

1. Download and extract this kit on your Android phone.
2. Open https://github.com/ in Chrome and sign in/create a GitHub account.
3. Create a **new PUBLIC repository** named `creatorai-studio-build`. Do not upload passwords, API keys, personal information, or YouTube login details.
4. In the repository, tap **Add file → Upload files** and upload `CreatorAI_Studio_Android_Source.zip`. Commit the upload.
5. Return to the repository and tap **Add file → Create new file**.
6. For the filename, type exactly: `.github/workflows/build-apk.yml`
7. Open the `build-apk.yml` file from this kit in a text editor, copy all its contents, and paste them into GitHub's new-file editor.
8. Commit the new file. GitHub Actions should start the build. If it does not, open the **Actions** tab, select **Build CreatorAI Studio APK**, and tap **Run workflow**.
9. Wait for the workflow to finish. Green tick means the build job succeeded; a red cross means it failed.
10. Open the completed workflow run, scroll to **Artifacts**, and download `CreatorAI-Studio-debug-APK`. Extract the downloaded artifact ZIP and tap `app-debug.apk` to install it. Android may ask you to allow installs from that browser/file manager.

## Free-plan note
GitHub Actions usage and limits can change. Public repository workflows are generally available without a paid plan, but the workflow is not guaranteed to succeed on every project/environment. This project has not been built or tested in this environment. If it fails, send a screenshot of the error.

## What this APK is
A starter dashboard with channel/topic planning templates and shortcuts. It is not a complete AI creator or automatic channel-management app yet. A debug APK is for personal testing, not Play Store release.
