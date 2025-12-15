# Abandoned Tools & Why

Documenting specific issues with abandoned tools to prevent future reconsideration.

## Desktop

### Logseq

- Orphaned images remain after page deletion
- No built-in way to detect or clean orphaned media files
- Manual cleanup required for deleted page attachments

### AppFlowy

vs Anytype

- Critical sync issues between desktop and mobile
- Mobile notes can become completely empty without warning
- Data recovery depends on desktop version availability
- Previously documented iOS sync issues remain unfixed

## Terminal

### GitUI

vs LazyGit

- Requires numeric keys (1-5) to switch panels
- Uses arrow keys instead of hjkl for navigation by default

### Neovim

vs Helix

- Completely unable to connect to system clipboard
- Treesitter fails in poor network conditions, leading to subsequent freezes
- Treesitter may freeze during compilation
- If you want to use it, use LazyVim plugin to save unnecessary configuration time

### Nushell

vs Fish

- No ghost text suggestions for commands
- Focuses on structured output while neglecting basic shell interactions

### Skim

vs fzf

- Performs worse than fzf in all benchmarks
- Core design less optimized than fzf
- Author acknowledges issues but abandoned improvements

### Zellij

vs tmux

- Higher resource consumption
- Lower framerate and slower key response in SSH sessions
- More prone to freezing
- Occupies excessive default keybindings, interfering with other shortcuts (Workaround: set `default_mode "locked"`)
