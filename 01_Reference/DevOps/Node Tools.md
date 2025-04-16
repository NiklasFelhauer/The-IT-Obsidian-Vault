
## NVM (Node Version Manager)

### Install & Use Node Versions

1. **List available Node.js versions:**
   ```shell
   nvm ls-remote
   ```

2. **Install a specific Node.js version:**
   ```shell
   nvm install <version>
   ```

3. **Install latest LTS version:**
   ```shell
   nvm install --lts
   ```

4. **Use a specific Node.js version:**
   ```shell
   nvm use <version>
   ```

5. **Set a default Node.js version:**
   ```shell
   nvm alias default <version>
   ```

6. **Show installed Node.js versions:**
   ```shell
   nvm ls
   ```

7. **Check current Node.js version:**
   ```shell
   node -v
   ```

8. **Check currently active `nvm` version:**
   ```shell
   nvm current
   ```

---

## NPM (Node Package Manager)

### Init & Install

1. **Initialize a new project (create `package.json`):**
   ```shell
   npm init
   ```

2. **Install all dependencies from `package.json`:**
   ```shell
   npm install
   ```

3. **Install a specific package:**
   ```shell
   npm install <package-name>
   ```

4. **Install a package as a dev dependency:**
   ```shell
   npm install <package-name> --save-dev
   ```

5. **Install a global package:**
   ```shell
   npm install -g <package-name>
   ```

6. **Install a specific version of a package:**
   ```shell
   npm install <package-name>@<version>
   ```

### Update & Remove

7. **Update all packages:**
   ```shell
   npm update
   ```

8. **Update a specific package:**
   ```shell
   npm update <package-name>
   ```

9. **Uninstall a package:**
   ```shell
   npm uninstall <package-name>
   ```

10. **Uninstall a global package:**
   ```shell
   npm uninstall -g <package-name>
   ```

### List & Info

11. **List all installed local packages:**
   ```shell
   npm list
   ```

12. **List globally installed packages:**
   ```shell
   npm list -g --depth=0
   ```

13. **View outdated packages:**
   ```shell
   npm outdated
   ```

14. **Show details of a package:**
   ```shell
   npm view <package-name>
   ```

### Scripts & Run

15. **Run a script defined in `package.json`:**
   ```shell
   npm run <script-name>
   ```

16. **Run tests (if `test` script is defined):**
   ```shell
   npm test
   ```

17. **Add custom script to `package.json`:**
   ```json
   "scripts": {
     "start": "node index.js"
   }
   ```
