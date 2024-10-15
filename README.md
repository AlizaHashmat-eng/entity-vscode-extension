# Entity VSCode Extension

**Hi there! I'm Aliza Hashmat,** a passionate software engineer and full-stack developer. This repository contains the **Entity VSCode Extension**, a powerful tool designed to enhance your productivity while working with entities in your projects. Whether you're dealing with databases or complex data structures, this extension simplifies your workflow and helps you focus on building great projects.

Feel free to star this project, share it with others, or contribute!

---

![example page](pageexample.png)

---

<h3 align="center">
 ⭐ Leave a star if you like this project! ⭐
</h3>

---

## 🚀 Features

- **Entity Management**: Easily create, modify, and manage entities in your project.
- **Database Integration**: Seamless integration with databases for generating entity structures.
- **Customization**: Tailor the extension to fit your project's needs with flexible options.
- **Efficiency Boost**: Accelerate your coding with entity templates and quick commands.
- **VSCode Integration**: Fully integrated with Visual Studio Code, making it accessible directly in your IDE.

---

## 📂 Project Structure

```text
entity-vscode-extension-main/
  ├── src/
  │     ├── extension.js
  │     └── utils.js
  ├── package.json
  ├── README.md
  ├── LICENSE
  └── .vscode/
        └── settings.json
```

---

## 📝 Customization Guide

### Internal Extension Customization

- **`entityType`**: Define the type of entity you’re working with (e.g., class, object, database table).
- **`properties`**: Add custom properties and their data types to your entities.
- **`generateEntityCommand`**: Run this command to generate new entities based on predefined templates.
- **`integrationOptions`**: Customize database connections or integrations with other systems.

### File Management

- **Extension Source Code**: Located in the `src/` folder. The core logic of the extension is in `extension.js`.
- **Utils**: Common utility functions are in the `utils.js` file.
- **Settings**: Customize VSCode-specific settings in `.vscode/settings.json`.
- **Package**: Modify the extension configuration in `package.json`.

---

## 📋 Getting Started

### Prerequisites

- **Visual Studio Code**: Make sure you have [VSCode](https://code.visualstudio.com/) installed.
- **Node.js**: Install [Node.js](https://nodejs.org/) for extension development.
- **npm**: Ensure you have npm installed, which comes with Node.js.

### Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/AlizaHashmat-eng/entity-vscode-extension-main.git
    cd entity-vscode-extension-main
    ```

2. **Install Dependencies**

    ```bash
    npm install
    ```

3. **Open in VSCode**

    - Open the cloned directory in Visual Studio Code.

### Running the Extension in Development Mode

1. **Open the Debug Panel** in VSCode (on the left side).
2. **Click on "Run Extension"**.
3. A new VSCode window will open with the extension loaded in development mode.

---

## 🚀 Publishing the Extension

To publish the extension to the VSCode marketplace:

1. **Create a VSCode Publisher Account**:
   - Follow the instructions to [create a publisher account](https://code.visualstudio.com/api/working-with-extensions/publishing-extension) on the VSCode marketplace.

2. **Package the Extension**:
   - Install the `vsce` tool:
     ```bash
     npm install -g vsce
     ```
   - Package the extension:
     ```bash
     vsce package
     ```

3. **Publish the Extension**:
   ```bash
   vsce publish
   ```

---

## 📋 Commands Overview

| Command                       | Action                                                 |
|-------------------------------|--------------------------------------------------------|
| `npm install`                 | Installs the dependencies                              |
| `npm run dev`                 | Starts development mode to test the extension          |
| `vsce package`                | Packages the extension for publishing                  |
| `vsce publish`                | Publishes the extension to the VSCode marketplace      |

---

## Want to Contribute?

Contributions are always welcome! Feel free to submit a pull request or report issues.

---

## 👀 Want to Learn More?

- Learn more about VSCode extensions in the [VSCode API documentation](https://code.visualstudio.com/api).
- Join the [VSCode community](https://code.visualstudio.com/community) for support and discussions.

---

## Contact

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/aliza-hashmat) or check out my projects on [GitHub](https://github.com/AlizaHashmat-eng).

---

### ⭐ If you found this project useful, don't forget to give it a star! ⭐

