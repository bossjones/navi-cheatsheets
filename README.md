# navi-cheatsheets

[Navi](https://github.com/denisidoro/navi) cheat sheets by bossjones.

## Quick Start

Install [navi](https://github.com/denisidoro/navi#installation), then add this repo in one command:

```sh
navi repo add bossjones/navi-cheatsheets
```

Launch navi and start searching:

```sh
navi
```

To preview all snippets from this repo without modifying your global install:

```sh
navi --path /path/to/navi-cheatsheets
```

## Configuration

Navi reads `~/.config/navi/config.yaml` (override with `$NAVI_CONFIG`).  
Cheatsheet directories are taken from `$NAVI_PATH` or the `cheats.paths` list in the config file.

Suggested config block:

```yaml
cheats:
  paths:
    - ~/.local/share/navi/cheats          # default community cheats (navi repo add …)
    - ~/dev/bossjones/navi-cheatsheets    # this repo, if cloned locally

style:
  tag:
    color: blue
  comment:
    color: white
  snippet:
    color: green

finder:
  overrides: "--height 60% --layout=reverse --border"
```

> **Tip:** Run `navi info cheats-path` to print the directories navi is currently searching.

## Tools

| Tool | Description | Link | Cheatsheet |
| --- | --- | --- | --- |
| RustScan | Fast, modern port scanner written in Rust | [GitHub](https://github.com/bee-san/RustScan) | [rustscan.cheat](./rustscan.cheat) |
| tmux | Terminal multiplexer for managing multiple sessions, windows, and panes | [GitHub](https://github.com/tmux/tmux) | [tmux.cheat](./tmux.cheat) |
| LunarVim | Opinionated, batteries-included Neovim distribution / IDE layer | [GitHub](https://github.com/LunarVim/LunarVim) | [lunarvim.cheat](./lunarvim.cheat) |
| bandwhich | Terminal bandwidth utilization tool showing per-process/connection network usage | [GitHub](https://github.com/imsnif/bandwhich) | [bandwhich.cheat](./bandwhich.cheat) |
| grex | Generates regular expressions from user-provided example strings | [GitHub](https://github.com/pemistahl/grex) | [grex.cheat](./grex.cheat) |
| difftastic | Structural diff tool that compares files based on syntax | [GitHub](https://github.com/Wilfred/difftastic) | [difftastic.cheat](./difftastic.cheat) |
| yazi | Blazing-fast terminal file manager written in Rust | [GitHub](https://github.com/sxyazi/yazi) | [yazi.cheat](./yazi.cheat) |
| sd | Intuitive find & replace CLI, a simpler alternative to `sed` | [GitHub](https://github.com/chmln/sd) | [sd.cheat](./sd.cheat) |
| procs | Modern, human-friendly replacement for `ps` written in Rust | [GitHub](https://github.com/dalance/procs) | [procs.cheat](./procs.cheat) |
| dust | More intuitive version of `du` for visualizing disk usage | [GitHub](https://github.com/bootandy/dust) | [dust.cheat](./dust.cheat) |
| yt-dlp | Feature-rich command-line audio/video downloader (youtube-dl fork) | [GitHub](https://github.com/yt-dlp/yt-dlp) | [yt-dlp.cheat](./yt-dlp.cheat) |
| gallery-dl | Command-line tool for downloading image galleries from various sites | [GitHub](https://github.com/mikf/gallery-dl) | [gallery-dl.cheat](./gallery-dl.cheat) |
| lms (lumins) | Fast and parallel file/directory copy and sync utility written in Rust | [GitHub](https://github.com/wchang22/lumins) | [lms.cheat](./lms.cheat) |
| tre | Tree alternative that respects `.gitignore` and outputs numbered shell aliases for quickly opening listed files | [GitHub](https://github.com/dduan/tre) | [tre.cheat](./tre.cheat) |
| gping | `ping`, but with a graph in the terminal | [GitHub](https://github.com/orf/gping) | [gping.cheat](./gping.cheat) |
| dua-cli | Interactive disk usage analyzer that quickly measures space used by directories | [GitHub](https://github.com/byron/dua-cli) | [dua.cheat](./dua.cheat) |
| delta | Syntax-highlighting pager for `git`, `diff`, and `grep` output | [GitHub](https://github.com/dandavison/delta) | [delta.cheat](./delta.cheat) |
| dnstop | Console tool to analyze DNS traffic captured from a network interface or pcap file, grouping by source, destination, and query name. | [GitHub](https://github.com/measurement-factory/dnstop) | [dnstop.cheat](./dnstop.cheat) |
| doggo | Modern, human-friendly command-line DNS client written in Go with colored output, JSON support, and DoH/DoT transports. | [GitHub](https://github.com/mr-karan/doggo) | [doggo.cheat](./doggo.cheat) |
| http-prompt | Interactive command-line HTTP client built on HTTPie and prompt-toolkit with autocomplete, syntax highlighting, and persistent session state. | [GitHub](https://github.com/httpie/http-prompt) | [http-prompt.cheat](./http-prompt.cheat) |
| HTTPie | User-friendly command-line HTTP client and cURL replacement with intuitive syntax, JSON support, colorized output, and form and file uploads. | [GitHub](https://github.com/httpie/cli) | [httpie.cheat](./httpie.cheat) |
| httpstat | Curl wrapper that visualizes HTTP connection and response timings (DNS, TCP, TLS, TTFB, transfer) with an ASCII diagram. | [GitHub](https://github.com/reorx/httpstat) | [httpstat.cheat](./httpstat.cheat) |
| LazySSH | Terminal-based SSH session manager that reads your SSH config and lets you browse, search, and connect to hosts interactively. | [GitHub](https://github.com/adembc/lazyssh) | [lazyssh.cheat](./lazyssh.cheat) |
| NetHogs | Net-top style tool that groups live network bandwidth usage by process instead of by connection, Linux-focused. | [GitHub](https://github.com/raboof/nethogs) | [nethogs.cheat](./nethogs.cheat) |
| Nmap | Industry-standard network discovery and security auditing tool for host discovery, port scanning, service and OS detection, and NSE scripting. | [GitHub](https://github.com/nmap/nmap) | [nmap.cheat](./nmap.cheat) |
| bat | Clone of `cat` with syntax highlighting, Git integration, line numbers, themes, paging, and diff rendering for source files. | [GitHub](https://github.com/sharkdp/bat) | [bat.cheat](./bat.cheat) |
| figlet | Banner-like program that prints strings as large ASCII-art text using selectable fonts, widths, and justification. | [Official](http://www.figlet.org/) | [figlet.cheat](./figlet.cheat) |
| gawk | GNU implementation of awk for pattern scanning, field extraction, and text processing with powerful programmable one-liners. | [GNU](https://www.gnu.org/software/gawk/) | [gawk.cheat](./gawk.cheat) |
| jq | Lightweight command-line JSON processor for querying, filtering, transforming, and pretty-printing JSON with a functional expression language. | [GitHub](https://github.com/jqlang/jq) | [jq.cheat](./jq.cheat) |
| ripgrep | Blazing fast recursive search tool respecting gitignore, with file-type filters, globs, context lines, and JSON output. | [GitHub](https://github.com/BurntSushi/ripgrep) | [ripgrep.cheat](./ripgrep.cheat) |
| fd | Simple, fast, user-friendly alternative to `find` with sensible defaults, smart case, and colorized parallel execution. | [GitHub](https://github.com/sharkdp/fd) | [fd.cheat](./fd.cheat) |
| fzf | General-purpose interactive fuzzy finder for files, history, and any stdin with preview windows and keybindings. | [GitHub](https://github.com/junegunn/fzf) | [fzf.cheat](./fzf.cheat) |
| duf | Disk Usage/Free utility, a better `df` | [GitHub](https://github.com/muesli/duf) | [duf.cheat](./duf.cheat) |
| eza | Modern, maintained replacement for `ls` | [GitHub](https://github.com/eza-community/eza) | [eza.cheat](./eza.cheat) |
| fdupes | Identify or delete duplicate files | [GitHub](https://github.com/adrianlopezroche/fdupes) | [fdupes.cheat](./fdupes.cheat) |
| ncdu | NCurses disk usage analyzer | [Official](https://dev.yorhel.nl/ncdu) | [ncdu.cheat](./ncdu.cheat) |
| lsof | List open files, sockets, and connections | [GitHub](https://github.com/lsof-org/lsof) | [lsof.cheat](./lsof.cheat) |
| mactop | Real-time Apple Silicon system monitor TUI with CPU, GPU, memory, and thermal metrics | [GitHub](https://github.com/metaspartan/mactop) | [mactop.cheat](./mactop.cheat) |
| pstree | Show running processes as a tree | [Official](http://www.thp.uni-duisburg.de/pstree/) | [pstree.cheat](./pstree.cheat) |
| fastfetch | Fast system info fetcher (neofetch-like) | [GitHub](https://github.com/fastfetch-cli/fastfetch) | [fastfetch.cheat](./fastfetch.cheat) |
| pv | Pipe viewer, monitor data progress through pipes | [Official](https://www.ivarch.com/programs/pv.shtml) | [pv.cheat](./pv.cheat) |
| git | Distributed revision control system | [GitHub](https://github.com/git/git) | [git.cheat](./git.cheat) |
| GitHub CLI (gh) | GitHub command-line tool | [GitHub](https://github.com/cli/cli) | [gh.cheat](./gh.cheat) |
| ghq | Remote repository management made easy | [GitHub](https://github.com/x-motemen/ghq) | [ghq.cheat](./ghq.cheat) |
| hub | Add GitHub support to git on the command-line | [GitHub](https://github.com/mislav/hub) | [hub.cheat](./hub.cheat) |
| Vim | Vi 'workalike' with many additional features | [GitHub](https://github.com/vim/vim) | [vim.cheat](./vim.cheat) |
| 1Password CLI (op) | Command-line interface for 1Password | [Docs](https://developer.1password.com/docs/cli) | [op.cheat](./op.cheat) |
| FFmpeg | Play, record, convert, and stream audio/video | [GitHub](https://github.com/FFmpeg/FFmpeg) | [ffmpeg.cheat](./ffmpeg.cheat) |
| Graphviz (dot) | Graph visualization software from AT&T and Bell Labs | [GitLab](https://gitlab.com/graphviz/graphviz) | [graphviz.cheat](./graphviz.cheat) |
| ImageMagick | Tools and libraries to manipulate images | [GitHub](https://github.com/ImageMagick/ImageMagick) | [imagemagick.cheat](./imagemagick.cheat) |
| fnm | Fast and simple Node.js version manager | [GitHub](https://github.com/Schniz/fnm) | [fnm.cheat](./fnm.cheat) |
| just | Handy way to save and run project-specific commands | [GitHub](https://github.com/casey/just) | [just.cheat](./just.cheat) |
| retry | Retry a command until it succeeds | [GitHub](https://github.com/kadwanev/retry) | [retry.cheat](./retry.cheat) |
| GNU Screen | Terminal multiplexer with VT100/ANSI emulation | [GNU](https://www.gnu.org/software/screen/) | [screen.cheat](./screen.cheat) |
| uv | Extremely fast Python package installer and resolver | [GitHub](https://github.com/astral-sh/uv) | [uv.cheat](./uv.cheat) |
| Repomix | Pack repository contents into a single AI-friendly file | [GitHub](https://github.com/yamadashy/repomix) | [repomix.cheat](./repomix.cheat) |
| ty | Extremely fast Python type checker and language server, written in Rust | [GitHub](https://github.com/astral-sh/ty) | [ty.cheat](./ty.cheat) |
| eget | Easily install prebuilt binaries from GitHub releases, with automatic OS/arch detection | [GitHub](https://github.com/zyedidia/eget) | [eget.cheat](./eget.cheat) |
| uvtemplate | Bootstrap modern Python projects with uv, ruff, type checking, and GitHub Actions | [GitHub](https://github.com/jlevy/uvtemplate) | [uvtemplate.cheat](./uvtemplate.cheat) |
| playwright-cli | Token-efficient CLI for browser automation, recording, and session management | [GitHub](https://github.com/microsoft/playwright-cli) | [playwright-cli.cheat](./playwright-cli.cheat) |
| guarddog | Identify malicious PyPI, npm, Go, RubyGems, GitHub Actions, and VSCode packages | [GitHub](https://github.com/DataDog/guarddog) | [guarddog.cheat](./guarddog.cheat) |
| getnf | Interactive installer and manager for Nerd Fonts | [GitHub](https://github.com/getnf/getnf) | [getnf.cheat](./getnf.cheat) |
| wtp | Git worktree manager with automatic setup hooks and shell navigation | [GitHub](https://github.com/satococoa/wtp) | [wtp.cheat](./wtp.cheat) |
| adt | Bundled Ansible developer tools: lint, navigator, molecule, builder, and creator | [GitHub](https://github.com/ansible/ansible-dev-tools) | [adt.cheat](./adt.cheat) |
| ruff | Extremely fast Python linter and code formatter, written in Rust | [GitHub](https://github.com/astral-sh/ruff) | [ruff.cheat](./ruff.cheat) |
| Homebrew (brew) | Package manager for macOS (and Linux) — formulae, casks, services, taps, bundles | [GitHub](https://github.com/Homebrew/brew) | [brew.cheat](./brew.cheat) |
| macOS | macOS power-user one-liners: Finder defaults, diskutil, networksetup, pmset, screencapture, clipboard | [Docs](https://support.apple.com/guide/terminal/welcome/mac) | [osx.cheat](./osx.cheat) |
| Network | General network troubleshooting: find IPs, ports, DNS, routes, interfaces, DNS cache flush | [Docs](https://man7.org/linux/man-pages/dir_section_8.html) | [network.cheat](./network.cheat) |
| cURL | Command-line HTTP client and file transfer tool supporting dozens of protocols | [GitHub](https://github.com/curl/curl) | [curl.cheat](./curl.cheat) |
