# Repo for implementing Whisper model for Lives project 

Python code for implementing the [Whisper model](https://github.com/openai/whisper) to transcribe English and Spanish interviews and to translate Spanish interviews to English translation. 

## Setup 
You will need to set up an appropriate coding environment:

* [Python (version 3.7 or higher)](https://www.python.org/downloads/)
* [PyTorch](https://pytorch.org)
* The following command will pull and install the latest commit from openai/whipser repository.
```
pip install git+https://github.com/openai/whisper.git
```
* It also required the command-line tool ```ffmpeg``` to be installed on your system, which is available from most package managers:
```
# on Ubuntu or Debian
sudo apt update && sudo apt install ffmpeg

# on Arch Linux
sudo pacman -S ffmpeg

# on MacOS using Homebrew (https://brew.sh/)
brew install ffmpeg

# on Windows using Chocolatey (https://chocolatey.org/)
choco install ffmpeg

# on Windows using Scoop (https://scoop.sh/)
scoop install ffmpeg
```
* You may need ```rust``` installed as well, in case [tokenizers](https://pypi.org/project/tokenizers/) does not provide a pre-built wheel for your platform. 
```
pip install setuptools-rust
```
## Models and languages
Whisper provides five model sizes, we use ```base``` model here which is a multilingual model and has 71,825,920 parameters. If you want to implement different sizes of models and consider the approximate memory requirements and relative speed, please go to ```Available models and languages``` section [here](https://github.com/openai/whisper#readme).









