[![Download Here](https://img.shields.io/badge/⬇_Download-Here-success?style=for-the-badge)](https://chromewebstore.google.com/detail/auto-flow-prompt-automati/lhcmnhdbddgagibbbgppakocflbnknoa)

# 🎬 Auto Flow v7.5.5 - Automation for Google VEO AI [![Tiếng Việt](https://img.shields.io/badge/Tiếng%20Việt-green)](README_vi.md) [![English](https://img.shields.io/badge/English-blue)](README.md) 

**Auto Flow** is a powerful Chrome Extension designed to automate the video creation process on Google Flow (VEO). This tool allows you to go "AFK" (Away From Keyboard) and generate hundreds of videos from text or images without the need for repetitive manual interaction.

-----

## ✨ Key Features

  * **🚀 Smart Queue:** Add a batch of prompts or images to the waiting list. The tool will automatically process tasks one by one.
  * **📝 Text-to-Video:** Support importing `.txt` files containing hundreds of prompts.
  * **🖼️ Image-to-Video:** Automatically upload images, crop aspect ratios, and generate motion.
  * **💾 Auto Download:** Automatically save videos to your machine immediately after rendering finishes. Supports folder organization by project name.
  * **🛡️ Retry Mechanism:** Automatically retry when encountering network errors or when Google's queue is full.
  * **⚙️ Deep Customization:**
      * Select Model (Veo 2, Veo 3.1...).
      * Select Aspect Ratio (16:9, 9:16).
      * Set number of video variants per prompt (1-4 variants).

-----

## 📥 Installation

1.  Visit [Auto Flow on Chrome Web Store](https://chromewebstore.google.com/detail/auto-flow-automation-for/lhcmnhdbddgagibbbgppakocflbnknoa).
2.  Click **Add to Chrome**.
3.  Access the [Google Flow](https://labs.google/fx/tools/flow) page.
4.  Open the Chrome Side Panel (the icon on the right side of the address bar) and select **Auto Flow**.

-----

## 📖 User Guide

### 1\. Text-to-Video Mode

1.  Select **Text-to-Video** mode in the Control tab.
2.  Enter prompts into the empty box (each prompt separated by a blank line) OR click the **Import file (.txt)** button to upload a list of prompts.
3.  Set the number of videos and aspect ratio.
4.  Click **Add to Queue** -\> **Start Queue**.

### 2\. Image-to-Video Mode

1.  Select **Image-to-Video** mode.
2.  Click **Select images** to upload (supports selecting multiple images at once).
3.  *(Optional)* Enter a supporting prompt. If left blank, AI will infer the context from the image.
4.  Click **Add to Queue** -\> **Start Queue**.

### 3\. Queue Management

  * Click the **Manage** button to view the list of pending tasks.
  * You can **Delete** excess tasks or **Reset** failed tasks to run them again.

-----

## 🔧 Troubleshooting

| Issue | Cause & Solution |
| :--- | :--- |
| **"Queue Full" Error** | Google Flow limits the number of videos processed simultaneously. **Don't worry**, the Extension will automatically wait and retry every 30s until a slot becomes available. |
| **Video not downloading** | Go to Chrome Settings -\> Downloads -\> **Turn off** *"Ask where to save each file before downloading"*. |
| **"Policy Error"** | Your prompt or image violates Google's content policy. The tool will automatically skip this task and proceed to the next one. |
| **Screen Zoomed Out** | This is an automatic feature of the tool to cover the interface and locate buttons accurately. Please do not adjust the zoom manually while the tool is running. |

-----

## 🔒 Privacy & Data

  * **Local Operation:** Auto Flow runs entirely on your browser.
  * **No Data Collection:** We do not collect your prompts, images, or videos. All data is stored only in your own `Chrome Local Storage` to remember settings.
  * **Permissions:** The extension only requests access to `labs.google/*` pages to perform automation tasks.

-----

## ☕ Support the Author

This software is developed and maintained for free. If this tool helps you save time and improve work efficiency, please consider buying the author a coffee\! ❤️

[duckmartians.info](https://duckmartians.info)

-----

## 📜 License

Copyright © 2025 **Dang Minh Duc (duckmartians)**. All Rights Reserved.

This software is proprietary property. Unauthorized copying, modification, distribution of source code, or resale in any form without written permission from the author is strictly prohibited.

-----

*Disclaimer: This extension is an independent project and is not affiliated with, endorsed by, or connected to Google or the Google Flow team.*
