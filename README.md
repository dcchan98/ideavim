# IdeaVim Configuration

This document outlines the custom key bindings and configurations for IdeaVim in IntelliJ IDEA.

## Global Configuration

- **Leader Key**: `Space` (` `)
- **Refactor Mode**: Keep current mode during refactoring
- **Timeout Settings**: No timeout for leader key combinations
- **Plugins**: vim-highlightedyank for visual feedback on yanked text

## Key Bindings Reference

### Window Management (`<leader><leader>` prefix)

| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `<leader><leader>t` | Activate Terminal | Open terminal tool window |
| `<leader><leader>l` | Activate TODO | Open TODO tool window |
| `<leader><leader>e` | Activate Project | Open project explorer |
| `<leader><leader>d` | Activate Debug | Open debug tool window |
| `<leader><leader>g` | Activate Git/Commit | Open commit tool window |
| `<leader><leader>x` | Hide All Windows | Hide all tool windows |

### Split Management (`<leader>s` prefix)

| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `<leader>sv` | Split Vertically | Create vertical split |
| `<leader>sh` | Split Horizontally | Create horizontal split |
| `<leader>smv` | Move Tab Right | Move current tab to right group |
| `<leader>smh` | Move Tab Down | Move current tab down |
| `<leader>sog` | Move to Opposite Group | Move editor to opposite tab group |
| `<leader>ss` | Maximize Split | Maximize current editor in split |

### Navigation

#### Enhanced Movement
| Key | Action | Description |
|-----|--------|-------------|
| `J` | Move 20 lines down | Fast downward movement |
| `K` | Move 20 lines up | Fast upward movement |

#### Window Navigation (`Space` prefix)
| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `Space h` | Move to left split | Navigate to left window |
| `Space j` | Move to bottom split | Navigate to bottom window |
| `Space k` | Move to top split | Navigate to top window |
| `Space l` | Move to right split | Navigate to right window |

#### Code Navigation (`g` prefix)
| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `gd` | Go to Declaration | Jump to symbol declaration |
| `gi` | Go to Implementation | Jump to symbol implementation |
| `ge` | Go to Next Error | Navigate to next error |
| `gE` | Go to Previous Error | Navigate to previous error |
| `gu` | Find Usages | Find all usages of symbol |
| `gh` | Quick Documentation | Show quick documentation |
| `gs` | Go to Super Method | Navigate to parent method |
| `gt` | Go to Type Declaration | Jump to type declaration |
| `gb` | Go Back | Navigate backwards in history |
| `gf` | Go Forward | Navigate forwards in history |

### Search and Find

#### Basic Search
| Key | Action | Description |
|-----|--------|-------------|
| `f` | Search Forward | Find text forward (replaces `/`) |
| `F` | Search Backward | Find text backward (replaces `?`) |
| `Enter` | Next Match | Go to next search result |
| `Shift+Enter` | Previous Match | Go to previous search result |

#### Advanced Find (`<leader>f` prefix)
| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `<leader>ff` | Go to File | Quick file navigation |
| `<leader>fg` | Find in Path | Search text across project |
| `<leader>fc` | Go to Class | Navigate to class |
| `<leader>fs` | Go to Symbol | Navigate to symbol |
| `<leader>fa` | Go to Action | Search IDE actions |

### Bookmarks (`<leader>m` prefix)

| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `<leader>mm` | Toggle Bookmark | Add/remove bookmark |
| `<leader>ml` | Show Bookmarks | List all bookmarks |
| `<leader>mf` | Next Bookmark | Go to next bookmark |
| `<leader>mb` | Previous Bookmark | Go to previous bookmark |

### Code Folding (`z` prefix)

| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `zc` | Collapse Region | Fold current code region |
| `zo` | Expand Region | Unfold current code region |
| `<leader>zc` | Collapse All | Fold all code regions |
| `<leader>zo` | Expand All | Unfold all code regions |

### Run & Debug (`<leader>r` prefix)

| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `<leader>rr` | Rerun | Execute last run configuration |
| `<leader>rc` | Choose Configuration | Select run configuration |
| `<leader>rb` | Toggle Breakpoint | Add/remove line breakpoint |
| `<leader>ro` | Step Over | Debug: step over current line |
| `<leader>ri` | Step Into | Debug: step into function |
| `<leader>ru` | Step Out | Debug: step out of function |
| `<leader>rc` | Continue/Resume | Debug: continue execution |

### Code Actions (`<leader>c` prefix)

| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `<leader>ca` | Code Actions | Show intention actions/quick fixes |
| `<leader>cp` | Code Prettier | Reformat current code |

### Configuration Management

| Key Combination | Action | Description |
|-----------------|--------|-------------|
| `<leader><leader><leader><leader>i` | Edit Config | Open .ideavimrc file |
| `<leader><leader><leader><leader>r` | Reload Config | Reload IdeaVim configuration |

### Visual Mode Enhancements

| Key | Action | Description |
|-----|--------|-------------|
| `<` | Indent Left | Decrease indentation (stays in visual mode) |
| `>` | Indent Right | Increase indentation (stays in visual mode) |

## Configuration Features

- **Case Insensitive Search**: Search ignores case by default
- **Incremental Search**: Shows matches as you type
- **Highlighted Yank**: Visual feedback when copying text
- **Smart Timeouts**: Leader key waits indefinitely, escape sequences timeout quickly

## Setup Instructions

1. Copy the configuration to your `.ideavimrc` file in your home directory
2. Restart IntelliJ IDEA or reload the configuration using `<leader><leader><leader><leader>r`
3. Ensure IdeaVim plugin is installed and enabled in IntelliJ IDEA

## Tips

- The leader key (Space) creates logical groupings of related commands
- Double leader combinations (`<leader><leader>`) are used for window management
- Triple/quadruple leader combinations are reserved for configuration management
- Most navigation follows Vim conventions with IDE-specific enhancements
- Use `J`/`K` for fast movement through large files (20 lines at a time)

## Customization

To modify this configuration:
1. Use `<leader><leader><leader><leader>i` to open the config file
2. Make your changes
3. Use `<leader><leader><leader><leader>r` to reload without restarting the IDE
