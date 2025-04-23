# SVG-Smuggling
## Embedding a Malicious File in an SVG Image

This demo illustrates SVG-based malware delivery.

1 - A script that launches PowerShell and prints "SVG Payload Activated!" is saved as `launch_powershell.bat`.

2 - The script is packed into a self-extracting `launch_powershell.exe` archive.

3 - The Base64-encoded SFX archive is embedded in an SVG file that imitates a Chrome crash page.

4 - A JavaScript code snippet is included with the archive to decode and launch the download automatically.

5 - When opened in a browser, user sees a fake browser crash page and is prompted to download the file.

6 - Upon clicking, the `launch_powershell.bat` file is extracted, and opening it triggers PowerShell, printing "SVG Payload Activated!" on user's screen.

## How to run:

Open `CrashSVG.svg` and follow the prompts.

