# Entity VSCode Extension

**Hi! I'm Aliza Hashmat**, a passionate software engineer and full-stack developer. This extension is designed to simplify the management and generation of entities in your projects, whether you're working with databases or complex data structures. The extension provides a streamlined workflow that accelerates development, saving you time and effort.
---

## 📋 Features

- **Entity Management**: Create and manage entities easily within VSCode.
- **Database Integration**: Seamlessly integrate entities with databases like MongoDB.
- **Customizable Templates**: Modify the entity generation templates to suit your project's needs.
- **Quick Commands**: Generate entities with a simple command, making coding faster and more efficient.

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:
- [Visual Studio Code](https://code.visualstudio.com/)
- [Node.js](https://nodejs.org/) (Version 14.x or higher)
- [npm](https://www.npmjs.com/)

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

3. **Open the Project in VSCode**

    Use Visual Studio Code to open the project directory.

4. **Run the Extension in Development Mode**

    - Open the **Debug Panel** in VSCode.
    - Select **"Run Extension"**.
    - This will open a new instance of VSCode with the extension loaded.

---

## 💻 Usage

### Command Palette

1. **Open the Command Palette**:  
   Press `Ctrl + Shift + P` (or `Cmd + Shift + P` on Mac) to bring up the Command Palette in VSCode.

2. **Use the `Generate Entity` Command**:  
   Start typing `Generate Entity` and select the command when it appears.


3. **Define Entity Properties**:  
   You will be prompted to define your entity's name and properties. Example:
    - Entity Name: `Customer`
    - Properties: 
      - `name`: `String`
      - `email`: `String`
      - `age`: `Number`
      - `isPremium`: `Boolean`


4. **Entity Generated**:  
   The extension will generate an entity file using your input, following a template you can customize. Example:

    ```javascript
    class Customer {
        constructor(name, email, age, isPremium) {
            this.name = name;
            this.email = email;
            this.age = age;
            this.isPremium = isPremium;
        }

        getDetails() {
            return `${this.name}, ${this.email}, Age: ${this.age}, Premium: ${this.isPremium}`;
        }
    }

    module.exports = Customer;
    ```

---

## ⚙️ Customization

### Customizing the Entity Template

You can modify the entity template to fit your needs. This customization can be done in the extension's settings or directly in the code.

### Database Integration

The extension supports database integration with systems like MongoDB. Here’s an example of using the generated entity with MongoDB:

```javascript
const mongoose = require('mongoose');

const customerSchema = new mongoose.Schema({
    name: String,
    email: String,
    age: Number,
    isPremium: Boolean,
});

const Customer = mongoose.model('Customer', customerSchema);

module.exports = Customer;
```

---

## 🛠️ Project Structure

Here is an overview of the project files and directories:

```text
entity-vscode-extension-main/
  ├── src/
  │     ├── extension.js           # Main extension file
  │     └── utils.js               # Utility functions
  ├── package.json                 # Project configuration and dependencies
  ├── README.md                    # Project documentation
  ├── LICENSE                      # License for the extension
  ├── .vscode/
  │     └── settings.json          # VSCode-specific settings
  ├── images/                      # Images used in the README and documentation
  │     ├── command-palette.png
  │     ├── generate-entity-command.png
  │     ├── entity-properties.png
  │     └── custom-template.png
```

## Demo: How the Extension Works

Here’s a quick demo of how the extension works:

### 1. Install the Extension

Install the **Entity VSCode Extension** from the VSCode marketplace or run it in development mode as explained above.

### 2. Use the `Generate Entity` Command

Open the **Command Palette** (`Ctrl + Shift + P`), type `Generate Entity`, and follow the prompts to create your entity.

### 3. Customize Templates

Customize your entity templates as shown in the customization section.

---

## 🌟 Want to Contribute?

Contributions are welcome! If you'd like to contribute to this project, feel free to submit a pull request or report issues.

---

## Commands

| Command                       | Description                                           |
|-------------------------------|-------------------------------------------------------|
| `npm install`                 | Installs the necessary dependencies                   |
| `npm run dev`                 | Starts the extension in development mode              |
| `vsce package`                | Packages the extension for deployment                 |
| `vsce publish`                | Publishes the extension to the VSCode marketplace     |

---

## 📦 Publishing

1. **Create a Publisher Account**:  
   To publish the extension to the marketplace, you must first create a publisher account on the [VSCode Marketplace](https://marketplace.visualstudio.com/).

2. **Package the Extension**:  
   Run the following command to package the extension:
   ```bash
   vsce package
   ```

3. **Publish the Extension**:
   ```bash
   vsce publish
   ```

---

## Contact

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/aliza-hashmat) or check out more of my work on [GitHub](https://github.com/AlizaHashmat-eng).

---

### ⭐ If you like this extension, don't forget to give it a star! ⭐
