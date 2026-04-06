# Foma Render Engine (FRE) - VS Code Extension

The official extension for **.fre** language support within the **Foma** ecosystem.

---

## Features

- **Syntax Highlighting**: Full support for HTML and handlebar logic (`{{each}}`, `{{if}}`, etc.).

- **Visual Identity**: Custom icon for all `.fre` files in the VS Code Explorer.

## 🛠 Installation

### Via the .VSIX file (Recommended)
1. Download the file `foma-render-engine-1.0.0.vsix`.

2. In VS Code, go to the **Extensions** tab (`Ctrl+Shift+X`).

3. Click on the `...` (top right) and choose **Install from VSIX...**.

4. Select the downloaded file.

### Enabling Icons
To see the Foma logo in your file explorer:

1. Press `Ctrl + Shift + P`.

2. Type **"File Icon Theme"**.

3. Select **"Foma Icons"**.

## Structure of a .fre file

`.fre` files leverage the power of Handlebars to inject dynamic data into your email or invoice templates.

```handlebars
<div class="foma-card">
<h1>Hello {{userName}}!</h1>
{{#if isPremium}}
<p>Thank you for your trust in FomaBank.</p>

{{/if}}
</div>
```