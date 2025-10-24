# Ollama-run

Just a small .sh that displays a menu to choose which local Large Language Model (LLM) will be run at the time.

## Usage

Just run

```bash
ollama-run
```

It will start ollama server (if not started yet) and display the available models to choose, and run it

![Example](example.png)

It is possible to quickly filter (it uses grep) the models by typing a name or part of it. For example, if you type `qwen`, it will display only the models that contain the word `qwen`.

```bash
$ ollama-run qwen

= Ollama is running =
--------------------
Available models:
1) qwen3:0.6b | size: 522 MB | modified: 5 months ago
2) qwen2.5-coder:7b | size: 4.7 GB | modified: 5 months ago
3) qwen2.5-coder:14b | size: 9.0 GB | modified: 5 months ago

Select a model (1-3):
(Press ctrl+c to cancel)
```

## Installation Steps

1) Save it in your computer
2) give it running permission with `chmod +x ollama_run`
3) add to your PATH env

```bash
# download the file
wget https://raw.githubusercontent.com/SoaresAlisson/ollama-run/refs/heads/main/ollama-run

# Create a local bin directory (if it doesn't exist):
mkdir -p ~/.local/bin

# Move the script to this directory:
mv ollama-run ~/.local/bin/ollama-run

# Make it executable
chmod +x ~/.local/bin/ollama-run

# Add the directory to your PATH 
export PATH="$HOME/.local/bin:$PATH"

# Reload your shell configuration:
## for bash:
source ~/.bashrc  
# or for zsh 
source ~/.zshrc
```
