# Filer Sidebar privacy policy

Filer Sidebar displays and manages files through the Filer Windows app on the same computer. The extension connects only to `http://127.0.0.1:47821`, a loopback address served by that app. It does not read web pages, browsing history, tabs, or other browser activity. It has no advertising or telemetry.

The extension processes the folders, file names, previews, searches, and file operations you request. Those requests go to the local Filer app. Filer stores settings, recent items, operation history, and optional content-search indexes on your computer. The extension stores a connection token in browser local storage so you can reconnect after restarting the browser or the app. The token expires after seven days and can be revoked in **Filer → Settings → Connected browsers**. Uninstalling the extension removes its browser storage; you can also revoke its connection in Filer.

Filer does not send your files or browser activity to the publisher. If you separately enable **AI ranking** in the Windows app and provide a TypeSafe API key, that optional feature sends search words and limited candidate metadata to TypeSafe AI as described in Filer's settings. The extension itself does not add any other remote service.

The browser store may process installation and update information under its own privacy policy. For questions about this policy, [open an issue](https://github.com/kRrIsH-T/filer-downloads/issues).

Last updated: 13 October 2026.
