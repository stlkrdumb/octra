# How to Run Octra Pre Client for Sending TX?

![image](https://github.com/user-attachments/assets/5a33fa96-d5ba-43b0-b682-e8b2cd5ee898)


**Installing uv (Python version manager)**
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
source $HOME/.local/bin/env
```
**Checking uv installation success with**
```bash
uv --version
```

**Downloading the client** 
```bash
git clone https://github.com/octra-labs/octra_pre_client.git
cd octra_pre_client
```

**Activate virtual environment**
```bash
uv venv
source .venv/bin/activate 
uv pip install -r requirements.txt
cp wallet.json.example wallet.json
```
**Open `wallet.json` file**
```
nano wallet.json
```
**Edit `"private key here"`, `"octxxxx"` & Save the file**

**Running the script**
```
uv run cli.py
```
