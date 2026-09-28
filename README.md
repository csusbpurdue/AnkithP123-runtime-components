# Runtime Components

A curated repository of runtime configuration (rc) files to keep shell, editor, debugger, and version control configurations synchronized and reproducible across machines (local environments, servers, lab machines, etc.).

## Contents

- `.bashrc`: Bash interactive shell configuration with custom prompt showing git branch, command aliases, and history settings.
- `.zshrc`: Zsh shell configuration for macOS/Linux, with support for oh-my-zsh and standalone Git prompt fallback.
- `.vimrc`: Vim editor configuration with indentation standards, line numbering, syntax highlighting, search settings, and Makefile tab preservation.
- `.gdbinit`: GDB configuration with command history, pretty printing for structs, and disabled pagination.
- `.gitconfig`: Global Git aliases (`st`, `br`, `sw`, `lg`, `unstage`), auto-coloring, and rebase pull settings.
- `install.sh`: Automated installation script to safely backup existing configurations, copy runtime component files into your home directory (`~`), link `.gitconfig.rc`, and optionally install oh-my-zsh.

## Usage

Make the installation script executable:
```bash
chmod +x install.sh
```

Run the installation script:
```bash
./install.sh
```

### Options:
- `./install.sh --dry-run`: Test run showing what files would be changed or backed up without modifying anything.
- `./install.sh --no-omz`: Skip installing oh-my-zsh.
