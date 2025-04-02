# Installation Guide for The-IT-Obsidian-Vault

Follow these steps to set up the vault locally with Git integration in Obsidian.

---

## 1. Install Prerequisites

- **[Obsidian](https://obsidian.md/)** – Download and install the app for your operating system.
- **[Git](https://git-scm.com/)** – Install Git to enable version control and sync functionality. (make sure to have git configured with your user.mail and user.name)

---

## 2. Clone the Vault into Obsidian

You can clone the repository directly from within Obsidian using the Git Community plugin:

1. Open **Obsidian** and create a new vault in a location of your choice.
2. Go to **Settings > Community Plugins**, search for `Git`, install it, and enable the plugin.
3. Press `Ctrl + P` (or `Cmd + P` on macOS) to open the **Command Palette**.
4. Type and select **`Git: Clone an existing remote repo`**.
5. When prompted, enter the repository URL:

   ```
   https://github.com/BlurryMelleFace/The-IT-Obsidian-Vault
   ```

   > 🔐 If you have contributor access, use the token-based URL instead:  
   > `https://<your_token>@github.com/BlurryMelleFace/The-IT-Obsidian-Vault`

6. Enter `Vault Root` as the target folder name.
7. When asked **"Does your remote repo contain a .obsidian directory at the root?"**, choose **Yes** and continue.

---

## 3. Open the Vault

- After cloning, Obsidian will prompt you to open the vault — choose **"Yes"**.
- If not prompted, use the **Open Folder as Vault** option and select the folder manually.

---

## 4. Install Required Plugins

### Core Plugins (already included, just enable them):

- File Explorer  
- Graph View  
- Backlinks  
- Daily Notes  
- Templates  
- Outline

### Community Plugins (install and enable manually):

1. Open **Settings > Community Plugins**.
2. Turn off **Safe Mode**.
3. Click **Browse** and search for:
   - `obsidian-git` – Enables Git-based syncing and commits.
   - `dataview` – Allows querying structured data from markdown notes.
4. Install and enable both.

---

