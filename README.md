# Small shell - a minimal Unix shell imitating Bash
This project was carried out as a team of two with <a href="https://github.com/kaloliina">@kaloliina</a>.\
We build the program for a 42 curriculum project called minishell at Hive Helsinki. 
The goal of this project was to build a Bash-inspired minimal Unix shell written in C.
<br><br>
## Quick Start 🚀
### 1. Clone the repository:
```bash
git clone https://github.com/sonjasonjao/small_shell.git
cd small_shell
```
### 2. Compile:

#### Prerequisites
- macOS: `brew install readline`
- Linux (Ubuntu/Debian): `sudo apt install libreadline-dev libncurses-dev`

#### Build (depending on your system)

**Linux (Ubuntu/Debian):**
```bash
make
```

**macOS (Apple Silicon):**
```bash
export CPPFLAGS="-I/opt/homebrew/opt/readline/include"
export LDFLAGS="-L/opt/homebrew/opt/readline/lib"
make
```

**macOS (Intel):**
```bash
export CPPFLAGS="-I/usr/local/opt/readline/include"  
export LDFLAGS="-L/usr/local/opt/readline/lib"
make
```
### 3. Run:
```bash
./small_shell
```
### 4. When program runs and opens standard input, give any command, such as
```bash
small shell > echo Hello world
Hello world
```
<br><br>
## My areas of responsibility
- Input parsing and validation: splitting into tokens and lexing
- Environment variable expansion handling
- Implementation of heredoc, and built-in commands: cd, echo, env, exit, export, pwd, and unset
- Signal handling: SIGINT, SIGQUIT (and ctrl+D)
<br><br>
## Personal learnings
- Unix shell commands and how they work under the hood (builtins)
- Input parsing to cover all possible edge cases
- How to implement heredoc functionality
- Readline functions: readline, rl_on_new_line, rl_redisplay, rl_replace_line, add_history
- Basics of signals and handling them
- Collaborating in a project, merging branches, solving merge conflicts, making codebase consistent with two contributors
