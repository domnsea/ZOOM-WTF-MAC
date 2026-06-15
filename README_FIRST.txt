ZOOM.WTF PC-TO-MAC RELEASE BUILDER

WHAT THIS IS
This pack lets you build a Mac-safe ZIP from a PC using GitHub Actions.

FINAL USER FLOW
1. User downloads ZOOM.WTF-mac.zip
2. User double-clicks the ZIP
3. User double-clicks ZOOM.WTF.app
4. ZOOM.WTF installs itself into Applications
5. ZOOM.WTF reopens automatically

IMPORTANT
Do not use normal Windows ZIP for the public Mac download.
GitHub Actions will run on macOS and create the ZIP using ditto, which preserves Mac app structure and permissions.

WHAT YOU MUST REPLACE
Replace this file:

ZOOM.WTF.app/Contents/Resources/main_app.sh

with your real Master/Guest GUI startup.

Keep the logging at the top if possible.
The placeholder currently only shows a success dialog.

HOW TO USE FROM PC
1. Create a GitHub repo.
2. Upload everything inside this folder to the repo.
3. Go to the repo on GitHub.
4. Click Actions.
5. Click Build ZOOM.WTF Mac ZIP.
6. Click Run workflow.
7. Download the artifact named ZOOM-WTF-Mac-ZIP.
8. Put ZOOM.WTF-mac.zip on your website.

FILES CREATED BY BUILD
ZOOM.WTF-mac.zip
ZOOM.WTF-mac.zip.sha256

SECURITY NOTE
For private/testing use, this is fine.
For public release with fewer Mac warnings, you still need Apple Developer ID signing and notarization.
