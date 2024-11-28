# **Guide: Save Your SwiftUI Project Progress to GitHub Using XCode 15+**

> A step-by-step guide for backing up an existing Xcode project to GitHub without using the terminal.
> This guide uses the updated "Integrate" option from Xcode 15 (used to be under "Source Control"). 

---

## **Step 1: Create a GitHub Repository**

1. Open Safari.
2. Navigate to GitHub at <https://github.com/>.
3. Log in to your GitHub account.
4. While logged in, click the **+** icon in the top-right corner and select **New repository**.

  ![Create a new GitHub Repository](https://docs.github.com/assets/cb-29762/mw-1440/images/help/repository/repo-create-global-nav-update.webp)

5. Important: Name the repository **exactly the same name** as your Xcode project folder (e.g., MySwiftApp).
6. Important: Leave **Initialize this repository with a README** unchecked.
7. Click **Create repository**.

---

## **Step 2: Enable Git in Your Xcode Project**

1. Open your project in **Xcode**.
2. Go to the menu bar and click **File > Integrate > New Git Repository**.
3. Choose the location (usually the root folder of your project) and click "Create".
   - This initializes Git for your project.
  
     ![File / Integrate / New Git Repository](https://i.sstatic.net/xitVc.png)

See [Step 2 for Existing Projects in this article for more](https://swiftandtips.com/how-to-create-a-remote-github-repository-from-xcode).
---

## **Step 3: Link Your Xcode Project to GitHub**

1. Open **Xcode Settings** (formerly Preferences) by clicking **Xcode > Settings** from the menu bar.
2. Go to the **Accounts** tab.
3. Click the **+** button in the bottom-left corner and select **GitHub**.
4. Log in to your GitHub account. Enter your credentials or use a personal access token (if required).
5. Ensure your GitHub account is visible and connected.

---

## **Step 4: Add the Remote Repository**

1. In the Xcode navigator, select the **Source Control Navigator** (icon with two branches, usually on the left panel).
2. Locate your project under **Local Repositories**.
3. Right-click your project and select **Configure Remotes...**.
4. In the **Remotes** section, click **Add Remote**.
5. Enter the following details:
   - **Name:** `origin`
   - **URL:** Copy the repository URL from your GitHub repository page (e.g., `https://github.com/yourusername/MySwiftApp.git`).
6. Click **Add** to save the remote repository.

---

## **Step 5: Commit Your Changes**

1. In Xcode, go to **Integrate > Commit...** from the menu bar.
2. Review the changes you’ve made (your SwiftUI files should be listed).
3. Write a descriptive commit message, such as `Initial commit`.
4. Click **Commit** to save the changes locally.

---

## **Step 6: Push Your Changes to GitHub**

1. After committing, go to **Integrate > Push...**.
2. Select the remote repository (`origin`) you added earlier.
3. Click **Push**.
   - Your project is now saved on GitHub!

---

## **Step 7: Verify Your Repository on GitHub**

1. Go back to your GitHub repository page in the browser.
2. Refresh the page to see your code uploaded.

---

### **Tips**

- Commit your changes often to track progress.
- Use descriptive commit messages to explain what you've done.


