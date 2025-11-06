# Auto Flow User Guide [![Tiếng Việt](https://img.shields.io/badge/Tiếng%20Việt-green)](README_vi.md) [![English](https://img.shields.io/badge/English-blue)](README.md) 

## 1. Introduction

**Auto Flow** is a Chrome extension designed to automate the bulk video creation workflow on the Google Flow platform.

This tool saves you time by automatically submitting batches of prompts or images for video generation, supporting the latest models like VEO (Veo 2, Veo 3.1), and automatically downloading the results.

## 2. Setup & Requirements

### Mandatory Requirements
1.  **Google Flow Project Page:** This extension **only works** when you have a Google Flow project page open (e.g., `https://labs.google/fx/tools/flow/project/...`). If opened on any other page, the extension will display a notification and a button to navigate to Flow.
2.  **Download Settings (Crucial):** For the "Auto-download videos" feature to work seamlessly, you **must** disable the "Ask where to save..." setting in your browser.
    * Open Chrome Settings: `chrome://settings/downloads`
    * Turn OFF the option: **Ask where to save each file before downloading**.
    * You can also click the "Configure folder" link in the extension's Settings Tab to open this page quickly.

## 3. Detailed User Guide

The Auto Flow interface is divided into 4 main tabs.

### 3.1. "Control" Tab

This is where you set up and initiate the automation process.

#### Step 1: Choose Creation Mode

You have two modes for video creation:

* **Text-to-Video:**
    * **Purpose:** Create videos in bulk using only a list of text prompts.
    * **Usage:** Select this mode and proceed to Step 2.
* **Image-to-Video:**
    * **Purpose:** Create videos in bulk by combining a list of images and a list of prompts.
    * **Usage:**
        1.  Click **"Select multiple images"** to upload your image files.
        2.  Use the **"Sort images"** dropdown to select the processing order (A-Z, Z-A, Newest, Oldest).
        3.  Proceed to Step 2 to input your prompts. These prompts will be used cyclically for your image list (e.g., 5 images and 2 prompts: images 1, 3, 5 use prompt 1; images 2, 4 use prompt 2).

#### Step 2: Input Data (Prompts/Images)

* **Input Prompts:**
    * **Type Manually:** Type your prompts into the "Prompt List" text area. **Important:** Each prompt must be **separated by at least ONE BLANK LINE** (press Enter twice).
    * **Import from File:** Click **"Import from file (.txt)"** to upload a text file. Prompts in the file must also be separated by blank lines.
* **Input Images:** (For Image-to-Video mode only) Completed in Step 1.

#### Step 3: Start the Process

Click the **"Start"** button. You will be presented with two choices:

1.  **🚀 Create New Project:**
    * The tool will automatically navigate to the Flow homepage, create a new project, and then begin running your tasks in that new project.
    * *Recommended for starting a completely new batch of work.*
2.  **➡️ Run on This Page:**
    * The tool will immediately start running on the project you currently have open.
    * *Recommended for continuing work on an existing project.*

#### Other Controls:

* **Pause / Continue:** While running, the "Start" button becomes a "Pause" button. Click to pause the process, and click again ("Continue") to resume from where it left off.
* **Stop:** Click this button to completely cancel the currently running process.

### 3.2. "Settings" Tab

Fine-tune the parameters to fit your needs.

* **Videos per task:** Choose the number of videos (1-4) that Flow should generate for EACH prompt or EACH image.
* **Start from (Prompt/Image):** Enter the number of the task you want to start from. E.g., if you have 100 prompts and want to start at prompt #50, enter `50`.
* **Video creation wait time (sec):** Set a random wait time range (min - max) after submitting each task. The tool will pick a random duration within this range to wait for the video to be generated before submitting the next task.
* **Model (Optional):** Select the VEO model you wish to use (Fast or Quality). "Default" is typically Veo 3.1 - Fast.
* **Ratio (T2V & I2V Crop):** Choose the aspect ratio for your videos (Landscape 16:9 or Portrait 9:16).
* **Language:** Change the extension's interface language (English / Tiếng Việt).
* **Auto-download videos:**
    * When enabled, the tool will automatically scan for and download newly generated videos.
    * **Note:** This feature requires you to disable "Ask where to save..." in your browser settings (see section 2. Setup & Requirements).

### 3.3. "History" Tab

Monitor and debug your workflow.

* **Detailed Log:** Shows a step-by-step log of what the tool is doing (task submitted, waiting, video downloaded, error, etc.).
* **Failed Tasks:** Lists all prompts or image filenames that failed (e.g., due to a Google policy error, network issue, or an inability to process).
    * The tool will automatically retry a failed task up to 5 times before marking it as failed.
* **Copy Failed Prompts/Images:** Click this button to copy the entire list of failed tasks to your clipboard. You can paste this list into a new `.txt` file or directly into the prompt box to run them again.

### 3.4. "More Tools" Tab

Discover other useful extensions from the author.

---

## 4. Tips and Notes

* **Policy Errors:** If Google Flow reports a policy error for a prompt or image, the tool will automatically detect it, log it in the History tab, and skip the task to continue the queue.
* **Keep Tab Open:** Always keep the Google Flow tab (where the tool is running) open and visible for stable operation.
* **Be Patient:** If you have a list of hundreds of tasks, be patient. The tool needs time to process and wait for Google Flow to generate the videos.

## ☕ Support the author

If you find this widget useful in your work, don't hesitate to buy the author a cup of coffee to support future projects!

[http://duckmartians.info](http://duckmartians.info)

## 📜 License

This project is licensed under the MIT License.
