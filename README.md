Chstr theme for Neovim.
===

Neovim theme based on [Chester theme from Wezterm](https://wezfurlong.org/wezterm/colorschemes/c/index.html#chester).

This theme is created with [Lush](https://github.com/rktjmp/lush.nvim).

## Preview
<!--
    TODO: add screenshots
-->

TODO

## Notes
I mainly develop this theme for personal use. As such, I cannot test the theme for every existing plugin which defines custom highlight groups (obviously, due to the lack of time and direct interest), but I'll gladly accept PR submissions.

Also, other than the basic groups, all the other groups will be set as I find them. If you find something before it has been defined, feel free to open an issue or a pull request.

# Installation
## Lazy
Add the plugin in your lazy configuration:
```
{
    'asperan/chstr.nvim',
    -- Load aduring startup if is the main colorscheme
    lazy = false,
    -- Load before all the other start plugins
    priority = 1000,
    dependencies = 'rktjmp/lush.nvim',
    -- Set the coloscheme to 'chstr'
    config = function()
        vim.cmd.colorscheme("chstr")
    end
}
```

# Configuration
You need to add this line to your configuration **ONLY** if the `config` field in the plugin manager configuration is not set.
```
vim.cmd.colorscheme("chstr")
```

# License
This theme is distributed accordingly to the [MIT License](https://mit-license.org/). Check the [LICENSE](LICENSE) file for more details.
