Claro! Aqui está um README.md completo e profissional para a extensão:

# **MaiaScript for Visual Studio Code**

[![Version](https://img.shields.io/badge/version-0.1.0-blue.svg)](https://marketplace.visualstudio.com/items?itemName=yourname.vscode-maiascript)
[![License](https://img.shields.io/badge/license-Apache%202.0-green.svg)](https://opensource.org/licenses/Apache-2.0)

![MaiaScript Logo](images/maiascript.png)

**MaiaScript Language Support** provides comprehensive syntax highlighting, code snippets, and theme support for the MaiaScript programming language in Visual Studio Code.

## 📋 **Features**

### ✨ **Syntax Highlighting**
Full syntax highlighting for all MaiaScript language elements:
- **Control Flow Keywords**: `if`, `for`, `while`, `return`, `break`, `continue`
- **Declaration Keywords**: `namespace`, `function`, `async`, `kernel`, `constructor`
- **Type Keywords**: `i32`, `i64`, `f32`, `f64`, `null`, `true`, `false`
- **Operators**: All MaiaScript operators (`:=`, `?=`, `||||`, `&&`, `||`, etc.)
- **Strings & Numbers**: Proper highlighting for quoted strings and numeric literals
- **Comments**: Single-line (`//`) and block (`/* */`) comments

### 🎨 **Custom Theme**
A dedicated dark theme optimized for MaiaScript:
- **Roxo** (#c586c0): Control flow keywords
- **Azul** (#569cd6): Declaration keywords  
- **Verde Água** (#4ec9b0): Type keywords
- **Amarelo** (#dcdcaa): Function names
- **Verde** (#6a9955): Comments
- **Laranja** (#ce9178): Strings
- **Dourado** (#ffd700): Brackets and parentheses

### 🚀 **Code Snippets**
Productivity-enhancing snippets for common MaiaScript patterns:

| Snippet | Description |
|---------|-------------|
| `namespace` | Create a new namespace |
| `function` | Define a new function |
| `async` | Create an async function |
| `kernel` | Create a kernel function |
| `if` | If statement |
| `ifelse` | If-else statement |
| `for` | For loop |
| `foreach` | Foreach loop |
| `try` | Try-catch block |

### ⚙️ **Editor Support**
- **Auto-closing brackets**: `{}`, `[]`, `()`
- **Auto-surrounding pairs**
- **Code folding markers**: `// #region` / `// #endregion`
- **Line and block comments** toggling

---

## 📥 **Installation**

### **From VSIX File**
1. Download the latest `.vsix` file from the [releases page](https://github.com/souzamonteiro/maia-vscode-extension/releases)
2. Open VS Code
3. Press `Ctrl+Shift+P` to open the command palette
4. Type "Install from VSIX" and select the downloaded file

### **From Command Line**
```bash
code --install-extension vscode-maiascript-0.1.0.vsix
```

### **From VS Code Marketplace** (Coming Soon)
Search for "MaiaScript" in the Extensions view (`Ctrl+Shift+X`)

---

## 🎯 **Usage**

### **File Associations**
Files with the following extensions are automatically recognized as MaiaScript:
- `.maia`
- `.maiascript`

### **Syntax Highlighting Example**
```maia
// This is a comment
namespace example {
    async function calculate(a, b) {
        i32 result = a + b
        string message = "Result: " + result
        
        if (result > 100) {
            for (i = 0; i < 10; i = i + 1) {
                // Process something
            }
        }
        
        try {
            return(message)
        } catch (error) {
            return("Error: " + error)
        }
    }
}
```

### **Using Snippets**
1. Type a snippet prefix (e.g., `namespace`)
2. Press `Tab` or `Enter`
3. The snippet expands with placeholders
4. Use `Tab` to navigate between placeholders

---

## 🎨 **Theme Preview**

![MaiaScript Theme Preview](https://raw.githubusercontent.com/souzamonteiro/maia-vscode-extension/main/images/theme-preview.png)

The custom theme is automatically activated when opening `.maia` files. You can also manually select it:
1. Press `Ctrl+K Ctrl+T`
2. Search for "MaiaScript Dark"

---

## 🔧 **Configuration**

The extension works out of the box, but you can customize it through VS Code settings:

```json
{
  "editor.tokenColorCustomizations": {
    "[MaiaScript Dark]": {
      "comments": "#your-color",
      "keywords": "#your-color",
      "strings": "#your-color",
      "numbers": "#your-color"
    }
  }
}
```

---

## 📦 **Extension Structure**

```
maia-vscode-extension/
├── .vscode/
│   └── launch.json          # Debug configuration
├── images/
│   ├── maiascript-dark.png  # Dark theme icon
│   └── maiascript-light.png # Light theme icon
├── snippets/
│   └── maiascript.json      # Code snippets
├── syntaxes/
│   └── maiascript.tmLanguage.json  # Syntax grammar
├── themes/
│   └── maia-color-theme.json       # Color theme
├── language-configuration.json      # Editor configuration
├── package.json                     # Extension manifest
└── README.md                        # This file
```

---

## 🤝 **Contributing**

Contributions are welcome! Here's how you can help:

1. **Report Bugs**: Open an issue describing the problem
2. **Suggest Features**: Share ideas for new features or improvements
3. **Submit PRs**: Fix bugs or add new functionality

### **Development Setup**
```bash
# Clone the repository
git clone https://github.com/souzamonteiro/maia-vscode-extension.git

# Install dependencies
npm install -g vsce

# Package the extension
vsce package

# Install locally
code --install-extension vscode-maiascript-0.1.0.vsix
```

### **Testing the Extension**
1. Open the project in VS Code
2. Press `F5` to launch a new Extension Development Host window
3. Open or create a `.maia` file to test

---

## 📄 **License**

This extension is licensed under the **Apache License 2.0**.

```
Copyright 2020 Roberto Luiz Souza Monteiro,
           Renata Souza Barreto,
           Hernane Borges de Barros Pereira.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

---

## 🙏 **Acknowledgments**

- The MaiaScript language creators and maintainers
- Visual Studio Code team for the amazing extension API
- All contributors and users of this extension

---

## 📞 **Support**

- **Documentation**: [MaiaScript Official Docs](https://www.maiascript.com)
- **Issues**: [GitHub Issues](https://github.com/souzamonteiro/maia-vscode-extension/issues)
- **Email**: roberto@souzamonteiro.com

---

**Enjoy coding with MaiaScript!** 🚀

---

## **Quick Reference Card**

| Feature | Description |
|---------|-------------|
| **File Extensions** | `.maia`, `.maiascript` |
| **Default Theme** | MaiaScript Dark |
| **Comment Toggle** | `Ctrl+/` |
| **Block Comment** | `Shift+Alt+A` |
| **Snippet Trigger** | Type prefix + `Tab` |
| **Auto-closing Brackets** | `{}`, `[]`, `()` |
| **Code Folding** | `// #region` / `// #endregion` |
