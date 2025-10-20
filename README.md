# Solo Tech

🦜 **Welcome!** This repository contains the documentation build pipeline for Solo Tech model finetuning as well as deployment for HuggingFace's LeRobot SO-101.

\* 🏠 `docs.getsolo.tech`](https://docs.getsolo.tech/) is our docs home, centralizing finetuned Solo Server models. This site is hosted on [Mintlify](https://mintlify.com).

[**Follow the full installation guide**](https://github.com/GetSoloTech/solo-server/blob/main/README.md)

## Development

Install the uv package manager to acquire solo-server. The following block contains the full installation instructions.

```
# uv package manager installation, skip if uv already exists
# Mac & Linux
curl -LsSf https://astral.sh/uv/install.sh | sh  
# Windows Powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

# Create Python virtual environment, recommended Python version 3.12
uv venv --python 3.12
# Mac & Linux
source .venv/bin/activate
# Windows
source .venv/scripts/activate

#Choose one of the following for solo-server installation
#1. Install solo server from PyPI python manager
uv pip install solo-server

#2. Install solo server from source
git clone https://github.com/GetSoloTech/solo-server.git
cd solo-server
uv pip install -e .

# Solo commands
solo --help
```

Alternatively, you can perform a quick, automated installation for Mac.

```
# Clone the repository
git clone https://github.com/GetSoloTech/solo-server.git
cd solo-server

# Make the installation script executable
chmod +x install_mac.sh

# Run the automated installation
./install_mac.sh
```