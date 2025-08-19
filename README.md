**LocalLLM: Running Llama3 on Your Mac**
================================

### Step 1: Install Llama macOS

[Download](https://ollama.com/download/Ollama-darwin.zip)

More details [Llama GitHub repository](https://github.com/ollama/ollama) 

### Step 2: Start Llama and download the Model weights
Run the command 

```bash
ollama run gpt-oss:20b
```

in your terminal to start Llama.

### Step 3: Install Docker
[Download](https://desktop.docker.com/mac/main/arm64/Docker.dmg?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-mac-arm64)
More Details  [Docker for Mac installation page](https://docs.docker.com/desktop/install/mac-install/)

### Step 4: Install Chat UI & Run Docker Container
Run the command:

```bash
docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
```
This will start a new Docker container running the Open-WebUI.

More details: Go to the [Open-WebUI GitHub repository](https://github.com/open-webui/open-webui).

### Step 5: Access Chat UI

* Go to your Docker dashboard and click on the "Open in Browser" button next to the `open-webui` container.
* Sign in with your account (create one if you don't have one already).
* Start chatting!

# Check the license on the projects:
Ollama: https://github.com/ollama/ollama/blob/main/LICENSE
Open-Webui: https://github.com/open-webui/open-webui/blob/main/LICENSE
Docker: https://docs.docker.com/desktop/install/mac-install/

