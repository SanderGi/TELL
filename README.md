# TELL
Token-level constrained generation for efficient language learning with conversational LLMs

0. `git clone https://github.com/KoelLabs/server.git`
1. Install Python 3.8.10 or higher
    - [Install pyenv](https://github.com/pyenv/pyenv?tab=readme-ov-file#installation)
    - Run `pyenv install 3.10.12`
    - Pyenv should automatically use this version in this directory. If not, run `pyenv local 3.10.12`
2. Create a virtual environment
    - Run `python -m venv ./venv` to create it
    - Run `. venv/bin/activate` when you want to activate it
        - Run `deactivate` when you want to deactivate it
    - Pro-tip: select the virtual environment in your IDE, e.g. in VSCode, click the Python version in the bottom left corner and select the virtual environment
3. Install dependencies
    - Run `pip install -r requirements.txt`
    - [Install the huggingface cli](https://huggingface.co/docs/huggingface_hub/en/guides/cli) with `pip install -U "huggingface_hub[cli]"`
    - Run `huggingface-cli login` using an [Access Token](https://huggingface.co/docs/hub/security-tokens) with read access from your [Settings Page](https://huggingface.co/settings/tokens)
4. Duplicate the `.env.example` file and rename it to `.env`. Fill in the necessary environment variables.
    - You can find your `HF_TOKEN` on your [Settings Page](https://huggingface.co/settings/tokens). It just needs read access to `gated repos`.
