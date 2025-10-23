# Ollama-run

Just a small .sh that displays a menu to choose which local Large Language Model (LLM) will be run

## Steps

1) Save it in your computer
2) give it permission with `chmod +x ollama_run`
3) add to your PATH env

```{bash }
# Create a local bin directory (if it doesn't exist):
mkdir -p ~/.local/bin

# Move the script to this directory:
mv ollama-run ~/.local/bin/ollama-run

# Make it executable
chmod +x ~/.local/bin/ollama-run

# Add the directory to your PATH by adding this line to your shell configuration file:
export PATH="$HOME/.local/bin:$PATH"

# Reload your shell configuration:
## for bahs:
source ~/.bashrc  
# or for zsh 
source ~/.zshrc
```

![Example](example.png)
