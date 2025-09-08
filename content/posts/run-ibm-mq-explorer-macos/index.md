---
title: "How to Run IBM MQ Explorer on macOS"
date: 2025-09-07T22:48:00-03:00
tags: ["guide", "mqexplorer", "eclipse", "macos"]
---
This guide provides step-by-step instructions for installing and configuring IBM MQ Explorer on macOS using the Eclipse IDE.

## 1. Install Eclipse IDE

You have two options for installing the Eclipse IDE:

*   **Using `brew` (Recommended):**

    Open your terminal and run the following command:

    ```bash
    brew install --cask eclipse-ide
    ```

*   **From the official Eclipse site:**

    Download the installer directly from the Eclipse website:
    [https://www.eclipse.org/downloads/packages/release/2025-06/r/eclipse-ide-eclipse-committers](https://www.eclipse.org/downloads/packages/release/2025-06/r/eclipse-ide-eclipse-committers)

## 2. Install IBM MQ Explorer in Eclipse IDE

1.  Launch Eclipse. From the main menu, navigate to **Help > Eclipse Marketplace**.

    ![Eclipse IDE with the Help menu open, highlighting the Eclipse Marketplace option.](./01.png)

2.  In the Eclipse Marketplace window, search for "mq explorer" and click **Install** for "IBM MQ Explorer Version 9.4.1 9" (or the highest version available).

    ![The Eclipse Marketplace window showing search results for 'mq explorer' with the Install button for IBM MQ Explorer highlighted.](./02.png)

3.  Accept the license agreement to proceed.

    ![The 'Review Licenses' dialog where the 'I accept the terms of the license agreement' radio button is selected.](./03.png)

4.  The installation progress will be displayed.

    ![The bottom-right corner of the Eclipse IDE showing an 'Installing Software' progress bar.](./04.png)

5.  A window will appear asking you to trust the content authorities. Click **Select All** and then **Trust Selected**.

    ![The 'Trust Authorities' security dialog listing certificates to trust, with the 'Select All' and 'Trust Selected' buttons available.](./05.png)

6.  A second window for trusting artifacts will appear. Repeat the previous step by clicking **Select All** and then **Trust Selected**.

    ![The 'Trust Artifacts' security dialog for unsigned content, showing options to trust the content.](./06.png)

7.  Once the installation is complete, you will be prompted to restart the Eclipse IDE. Click **Restart Now**.

    ![The 'Software Updates' dialog box prompting the user to restart the IDE, with the 'Restart Now' button highlighted.](./07.png)

## 3. Open the IBM MQ Explorer Perspective

1.  From the main menu, go to **Window > Perspective > Open Perspective > Other...**.

    ![Eclipse main menu showing the navigation path: Window > Perspective > Open Perspective > Other....](./08.png)

2.  Select **MQ Explorer** from the list and click **Open**.

    ![The 'Open Perspective' dialog with 'MQ Explorer' highlighted from the list of choices.](./09.png)

3.  The MQ Explorer perspective is now active. You can access it directly from **Window > Perspective > Open Perspective > MQ Explorer**.

    ![Eclipse main menu showing that 'MQ Explorer' is now a direct option under the 'Open Perspective' submenu.](./10.png)

4.  Click the **Hide** icon on the Welcome screen to close it.

    ![The Eclipse 'Welcome' screen with the 'Hide' button in its top-right corner highlighted.](./11.png)

5.  You are now in the IBM MQ Explorer environment. ✅

    ![The main IBM MQ Explorer interface within Eclipse, showing the Navigator panel on the left and the 'Welcome' content panel on the right.](./12.png)

## 4. Import MQ Queues (from XML)

1.  In the MQ Explorer Navigator, right-click on **IBM MQ** and select **Import MQ Explorer Settings...**.

    ![A right-click context menu on the 'IBM MQ' item in the Navigator panel, with the 'Import MQ Explorer Settings...' option highlighted.](./13.png)

2.  Select **MQ Explorer Settings** and click **Next**.

    ![The 'Import' wizard dialog with the 'MQ Explorer Settings' option selected under the 'MQ Explorer' category.](./14.png)

3.  Browse to and select the XML file containing your MQ queue configurations.

    ![The 'Import MQ Explorer Settings' dialog showing a file path to an XML file selected for import.](./15.png)

4.  A list of Gateways for accessing the MQ queues will be displayed.

    ![The MQ Explorer Navigator panel populated with an expanded list of Queue Managers after a successful import.](./16.png)

---

> Eclipse will automatically reopen the MQ Explorer perspective on startup if it was the last one you used.
