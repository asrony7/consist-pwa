CONSIST PWA STARTER
===================

Files:
- index.html: the Consist prototype with PWA links and service-worker registration
- manifest.json: app name, theme, start URL, and install icons
- service-worker.js: caches the app shell for repeat/offline visits
- icons/: 192px and 512px PNG icons

PHONE-ONLY DEPLOYMENT OVERVIEW
1. Extract this ZIP on your phone.
2. Upload the contents (index.html, manifest.json, service-worker.js, icons folder) to a static website host that serves HTTPS.
3. Ensure index.html is at the published site's root and the other files retain their paths.
4. Open the HTTPS URL in Chrome on Android.
5. Open Chrome's three-dot menu and choose "Install app" or "Add to Home screen" if offered.
6. Open the installed app once while online, then test it offline.

Important:
- Opening index.html directly as file:// is not enough for installability; PWA install and service workers require HTTPS or localhost.
- The script generator is currently template-based, not live AI.
- The reel editor currently previews a video and text overlay; it does not export edited MP4.
- Local data is stored in the browser/app origin. Changing the published domain can make the old local data appear missing, so export a JSON backup first.
