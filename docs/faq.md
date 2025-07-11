# Frequently Asked Questions

## General Questions

### What is Droidnet Comlink?
Droidnet Comlink is an iOS app that provides hands-free voice control for astromech droids. It listens for your droid's name and sends commands via WiFi to control lights, sounds, and movements.

### What droids are supported?
Any droid that can receive serial commands through a Droidnet Signal Booster (or compatible system) can work with the app. This includes R2-D2, BB-8, BD-1, and custom builds.

### Do I need special hardware?
Yes, you need a Droidnet Signal Booster (a Raspberry Pi running special software) connected to your droid's control system.

### Does it work offline?
Yes! All voice processing happens on your device. You only need WiFi to communicate with your droid - no internet required.

## Setup Questions

### Why does the app need so many permissions?
- **Microphone**: To hear your voice commands
- **Speech Recognition**: To convert speech to text
- **Local Network**: To send commands to your droid

### Can I use multiple wake words?
Currently, you can set one wake word at a time, but you can change it anytime in Settings.

### How do I connect multiple droids?
In the Droidnet tab, you can select multiple Signal Boosters. Commands will be sent to all selected droids simultaneously.

## Usage Questions

### Why must the app stay in foreground?
iOS restrictions prevent apps from using the microphone in the background for privacy reasons. The screen can be dimmed to save battery.

### What's the command format?
Say your wake word, pause briefly, then say the command. Example: "R2... play cantina band"

### Can I create custom commands?
Yes! Go to Commands tab, tap +, and create your own. You can set multiple voice triggers for each command.

### How accurate is voice recognition?
The app uses advanced phonetic matching to handle variations. For example, if you say "are you" it understands you mean "R2".

## Troubleshooting

### Commands aren't working
1. Check the Control tab - is it in Test Mode?
2. Verify your Signal Booster is selected in Droidnet tab
3. Check Command History to see what was recognized
4. Ensure your wake word is set correctly

### The app says "Session Refreshing"
This is normal - Apple limits speech recognition sessions to 45 minutes. The app automatically refreshes with minimal interruption.

### My Signal Booster isn't appearing
- Ensure it's on the same WiFi network
- Check that it's powered on and running
- Try pull-to-refresh in the Droidnet tab
- Verify local network permission is granted

### Voice recognition seems slow
- This usually improves after the first few commands
- Ensure you have a strong WiFi signal
- Try restarting the app

## Privacy & Security

### Is my voice data sent to servers?
No. All speech processing happens on your iPhone. Voice data never leaves your device.

### What data does the app collect?
The app stores your commands and settings locally. No personal data is collected or transmitted.

### Can others control my droid?
Only devices on your WiFi network can communicate with your Signal Booster. Use standard WiFi security practices.

## Advanced Features

### Can I share my command sets?
Yes! Use the export feature in Commands tab to share your custom commands with other builders.

### Is there an Apple Watch app?
Not yet, but it's planned for a future update.

### Can I use Siri Shortcuts?
This feature is planned for version 1.1.

---

Have a question not answered here? [Ask in our support forum](https://github.com/travisccook/droidnet-comlink-support/issues/new?labels=question)!