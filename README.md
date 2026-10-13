# Filer downloads

Filer is a Windows 11 file manager with a browser sidebar. File access is local by default. The sidebar requires the Filer Windows companion, which runs at `127.0.0.1:47821`. An optional AI ranking feature in the Windows app can send search terms and limited candidate metadata to TypeSafe AI when you enable it.

## Install

1. Download `filer-windows-0.3.2.zip` from the [latest release](https://github.com/kRrIsH-T/filer-downloads/releases/latest) and extract the entire ZIP.
2. Open PowerShell in the extracted folder and run:

   ```powershell
   powershell -ExecutionPolicy Bypass -File .\scripts\setup.ps1 -SkipBuild
   ```

3. Setup installs the signed Everything search service if needed, adds Filer to the Start menu, and starts it at Windows sign-in. The Filer app and extension folder are installed under `%LOCALAPPDATA%\Filer\app`.
4. For Edge, Chrome, or Brave, open the browser's Extensions page, enable Developer mode, choose **Load unpacked**, and select `%LOCALAPPDATA%\Filer\app\extension\chromium`. Pin Filer Sidebar. It remains installed after browser restarts and when Filer is closed, as long as you keep the installed folder and browser profile.
5. Click the extension icon, click **Connect**, and approve the matching six-digit code in the Windows dialog. If Filer is closed later, the sidebar offers **Start Filer**.

The extension is being prepared for Edge Add-ons and Firefox Add-ons. Firefox's `about:debugging` install is temporary and is removed at restart; wait for the Mozilla-signed listing for a permanent Firefox install. Chrome Web Store publication requires Google's one-time developer fee.

## Privacy and safety

See the [Filer Sidebar privacy policy](PRIVACY.md). The sidebar requests local storage and access to the loopback companion only. It does not read visited pages or browser history. Check `SHA256SUMS.txt` in the release against your download. The Windows executable is currently unsigned, so Windows may show a publisher warning; the separate Everything installer is signed by voidtools and checked by setup.

The bundled `THIRD_PARTY_NOTICES.md` lists third-party software. Support and issues can be filed in this repository.
