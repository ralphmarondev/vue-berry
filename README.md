# Vue 3 + TypeScript + Vite - Vue-Berry

This repository is created to practice and enhance my knowledge of **Vue 3**, **Vite**, and **TypeScript**. It is a
simple project, and suggestions or contributions are always welcome! You can open an issue or submit a pull request with
your improvements or ideas.

- **Maintained by**: Ralph Maron Eda
- **Email**: [edaralphmaron@gmail.com](mailto:edaralphmaron@gmail.com)
- **GitHub**: [https://github.com/ralphmarondev](https://github.com/ralphmarondev)

## Project Setup

This guide helps you create and run a **Vue 3** project with **Vite** and **TypeScript**, using **Yarn** as the package
manager.

### Recommended IDE (Optional)

While you can use any editor or IDE of your choice, we recommend using **WebStorm** for the best development experience
with this project. **WebStorm** offers excellent support for **Vue 3**, **TypeScript**, and **Vite**, along with useful
features like advanced debugging and refactoring tools.

If you prefer another editor, such as **VSCode**, **Sublime Text**, or **Atom**, feel free to use that instead! The
setup and usage will remain the same.

## Prerequisites

Ensure the following tools are installed on your system:

- **Node.js** (LTS version recommended)
- **Yarn** (for package management)

### Installing Yarn

If you don't have Yarn installed, you can install it globally using **npm**:

```bash
npm install -g yarn
```

---

## 1. Create the Project Using Vite

You can create a new Vue 3 project with **Vite** and **TypeScript** using Yarn:

```bash
yarn create vite vue-berry --template vue-ts
```

- Replace `vue-berry` with your preferred project name.

---

## 2. Install Dependencies

Once the project is created, navigate to the project folder and install the dependencies:

```bash
cd vue-berry
yarn install
```

---

## 3. Open the Project in WebStorm

1. Launch **WebStorm**.
2. Go to **File > Open** and select the folder of the newly created project (`vue-berry`).
3. Click **OK** to open it in WebStorm.

---

## 4. Configure the Run Configuration in WebStorm

To run the Vite development server directly from WebStorm:

1. Go to **Run > Edit Configurations**.
2. Click the **+** icon to add a new configuration.
3. Select **npm** (or **yarn** if available) from the list.
4. Set the following configuration options:
    - **Name**: `Vite Dev Server`
    - **Package Manager**: Select **Yarn** (if not already selected).
    - **Command**: Leave as **run**.
    - **Script**: Set this to `dev`.

Your configuration should look like:

- **Package Manager**: Yarn
- **Command**: run
- **Script**: dev

5. Click **OK** to save the configuration.

---

## 5. Run the Development Server

To run the development server:

1. Click the **Run** button (green play icon) at the top-right corner of WebStorm.
2. The **Vite dev server** will start, and you can open the app in your browser at:

   ```plaintext
   http://localhost:5173
   ```

   **Output in WebStorm Terminal:**
   ```
   VITE v5.4.10  ready in 1702 ms

   ➜  Local:   http://localhost:5173/
   ➜  Network: use --host to expose
   ➜  press h + enter to show help
   ```

---

## 6. Running the Project from the Command Line (CLI)

If you prefer working with the command line (e.g., in **VSCode** or any terminal-based environment), you can still run
the development server directly from your terminal.

1. **Open your terminal** inside the project directory (`vue-berry`).
2. Run the following command to start the development server:

   ```bash
   yarn dev
   ```

   This will start the **Vite dev server**, and you can access the app at:

   ```plaintext
   http://localhost:5173
   ```

   You’ll see output similar to this in the terminal:

   ```
   VITE v5.4.10  ready in 1702 ms

   ➜  Local:   http://localhost:5173/
   ➜  Network: use --host to expose
   ➜  press h + enter to show help
   ```

---

## 7. Opening the Project in WebStorm

If you prefer, you can always open the project in **WebStorm** directly by launching **WebStorm** and navigating to:

- **File > Open**
- Select the project folder (`vue-berry`)
- Click **OK** to load the project in WebStorm

---

## 8. Additional Notes

- **Yarn** is used as the package manager, but you can switch to **npm** if needed by changing the package manager in
  the WebStorm **Run Configuration**.
- WebStorm automatically detects **Yarn** as the package manager, but you can manually configure it if needed.
- If you're using **VSCode**, ensure the **Yarn** or **npm** executable is installed and available in your system's *
  *PATH** for seamless CLI operations.

---

## Troubleshooting

If you run into issues where **Yarn** is not found, ensure it is installed globally and added to your system's **PATH**.
Run the following command to verify **Yarn** installation:

```bash
yarn --version
```

If you're using **npm**, run:

```bash
npm --version
```

---

## License

This project is licensed under the **MIT License**. You can view the license in the [LICENSE.txt](LICENSE.txt) file.

---

## Summary

- Created a **Vue 3** project using **Vite** and **TypeScript** with **Yarn**.
- Set up a **Run Configuration** in **WebStorm** to start the Vite development server using **Yarn**.
- **VSCode** and other editors can also be used with the CLI to run the project via `yarn dev`.
- You can now develop your app with **Vue 3**, **Vite**, and **TypeScript** seamlessly in **WebStorm** or any
  terminal-based editor!

Happy coding! 🎉