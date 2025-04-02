# Installation Guide for The-IT-Obsidian-Vault

Follow these steps to set up the vault locally with Git integration in Obsidian.

---

## 1. Install Prerequisites

- **[Obsidian](https://obsidian.md/)** – Download and install the app for your operating system.
- **[Git](https://git-scm.com/)** – Install Git to enable version control and syncing features. Make sure Git is configured with your `user.email` and `user.name`.

---

## 2. Clone the Vault into Obsidian

You can clone the repository directly from within Obsidian using the Git Community plugin:

1. Open **Obsidian** and create a new vault in a location of your choice.
2. **Delete** the Welcome file
3. Go to **Settings > Community Plugins**, search for `Git`, install it, and enable the plugin.
4. Press `Ctrl + P` (or `Cmd + P` on macOS) to open the **Command Palette**.
5. Type and select **`Git: Clone an existing remote repo`**.
6. When prompted, enter the repository URL:

   ```
   https://github.com/BlurryMelleFace/The-IT-Obsidian-Vault
   ```

   > 🔐 If you have contributor access, use the token-based URL instead:  
   > `https://<your_token>@github.com/BlurryMelleFace/The-IT-Obsidian-Vault`

6. Enter `Vault Root` as the target folder name.
7. When asked **"Does your remote repo contain a .obsidian directory at the root?"**, choose **Yes** and continue with the deletion process and press enter.

---

## 3. Restart the Vault

After the cloning process is complete:

- Reopen the vault in Obsidian to ensure that all additional community plugins and settings from the repository are properly recoagnized and loaded.

---

