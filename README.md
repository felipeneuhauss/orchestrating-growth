# Orchestrating Growth Project

This repository houses the "Orchestrating Growth" project, which consists of multiple interconnected modules to create a complete user experience.

## How to Initialize and Update Submodules

To work with this repository and its submodules, follow these initial steps:

1. **Clone the Main Repository:**

   ```
   git clone <URL-of-the-main-repository>
   cd orchestrating-growth
   ```

2. **Initialize and Update Submodules:**

   Initialize the submodules with the following command:

   ```
   git submodule init
   ```

   Then, update the submodules to the versions defined in the main repository:

   ```
   git submodule update
   ```

   Alternatively, to update the submodules to their latest available versions:

   ```
   git submodule foreach git pull origin main
   ```

3. **Working with Submodules:**

   After initializing and updating the submodules, you can work with them as follows:

   - **catalog-app:** Navigate to the `catalog-app` directory to work on this specific submodule.

   - **main-app:** Navigate to the `main-app` directory to work on this specific submodule.

   - **ui-app:** Navigate to the `ui-app` directory to work on this specific submodule.

4. **Updating Submodules in the Main Repository:**

   When you make changes to a submodule and want to update the main repository to include those changes, follow these steps:

   - In the submodule directory (e.g., `catalog-app`, `main-app`, or `ui-app`), make your desired changes and commit them.

   - Navigate back to the main repository's root directory.

   - Update the main repository to track the latest changes in the submodule by running:

     ```
     git add <submodule-directory>
     git commit -m "Update submodule: <submodule-name>"
     ```

     Replace `<submodule-directory>` with the actual directory name of the submodule you modified, and `<submodule-name>` with the submodule's name.

   - Push the changes to the main repository:

     ```
     git push origin main
     ```

   This will update the main repository to reference the latest commit of the submodule with your changes.

Remember that after cloning the main repository on a new machine or after each update, you should run the submodule initialization and update commands again to ensure that you have the latest submodule versions.

