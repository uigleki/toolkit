# Abandoned Tools & Why

## GitUI

vs lazygit

- Requires numeric keys (1-5) to switch panels
- Uses arrow keys instead of hjkl for navigation by default

## Neovim

vs helix

- Completely unable to connect to system clipboard
- Treesitter fails in poor network conditions, leading to subsequent freezes
- Treesitter may freeze during compilation
- If you want to use it, use LazyVim plugin to save unnecessary configuration time

## Nushell

vs fish

- No ghost text suggestions for commands
- Focuses on structured output while neglecting basic shell interactions

## Skim

vs fzf

- Noticeably slower with large datasets
- Higher memory consumption
- Less optimized implementation

## Zellij

vs tmux

- Higher resource consumption
- Lower framerate and slower key response in SSH sessions
- More prone to freezing
- Occupies excessive default keybindings, interfering with other shortcuts (Workaround: set `default_mode "locked"`)
