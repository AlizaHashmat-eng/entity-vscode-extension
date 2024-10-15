# Entity VSCode Extension

## Overview

The **Entity VSCode Extension** simplifies managing and generating entities in your projects. Whether you’re working with databases or complex data structures, this extension enhances your workflow and accelerates development. Here's a detailed walkthrough of how to use it.

---

## Demo: How the Extension Works

### 1. Install the Extension

First, install the **Entity VSCode Extension** from the [VSCode marketplace]() or clone the repository and load the extension in **development mode**.

### 2. Open the Command Palette

Press `Ctrl + Shift + P` (or `Cmd + Shift + P` on Mac) to open the **Command Palette** in VSCode.

![Command Palette](images/command-palette.png)

---

### 3. Use the `Generate Entity` Command

Type `Generate Entity` into the Command Palette and select it. This command initiates the process of creating a new entity.

![Generate Entity Command](images/generate-entity-command.png)

---

### 4. Define Entity Properties

Next, you'll be prompted to enter details for the new entity. Define the entity name and its properties, such as fields and data types.

**Example**:
- **Entity Name**: `Customer`
- **Properties**:
  - `name` (String)
  - `email` (String)
  - `age` (Number)
  - `isPremium` (Boolean)

![Entity Properties](images/entity-properties.png)

---

### 5. Generated Entity

After providing the properties, the extension will automatically generate an entity file based on the template. Here’s an example of the generated **Customer Entity**:

```javascript
// Customer Entity

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

### 6. Customize Templates

If you wish to customize the generated templates, you can modify them via the extension settings. Tailor the structure and formatting to your project needs.

Here’s an example of where to change the template:

![Custom Template](images/custom-template.png)

---

### 7. Database Integration

The extension supports integration with databases. Here’s how you can use the generated entity with MongoDB:

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

With this, you can connect the entities to a MongoDB database and manage your data more efficiently.

---

## Example Screenshots

Here are a few more examples of the extension in action:

- **Command Palette**:
  ![Command Palette](images/command-palette-example.png)

- **Generated Entity File**:
  ![Generated Entity](images/generated-entity-example.png)

- **Custom Template**:
  ![Custom Template](images/custom-templates-example.png)

---

## Ready to Use?

1. **Install the extension** or clone the repository.
2. **Generate your first entity** using the command palette.
3. **Customize the templates** to fit your project.

---

### ⭐ If you like this extension, please give it a star on GitHub! ⭐

---

## Contact

For more information, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/aliza-hashmat) or check out more of my work on [GitHub](https://github.com/AlizaHashmat-eng).

---

This page is designed to walk users through the usage of the **Entity VSCode Extension**, showing them how to get started and customize it according to their needs. The visuals make it easy to understand how the extension functions, and the example code provides real-world applications.

You can use this content for your **example page** and integrate the screenshots (`images/command-palette.png`, etc.) into your repository.

Let me know if you need further adjustments!
### ⭐ If you found this project useful, don't forget to give it a star! ⭐

