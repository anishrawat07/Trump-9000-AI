# 🚀 Trump-9000: The AI Overlord (Dolphin-Llama3 Edition)  

### **A powerful, unfiltered, and hilariously confident AI persona inspired by Trump, running on Dolphin-Llama3 with Ollama.**  

---

## **📌 Features**
✅ **Fully uncensored** – Will express both positive and negative opinions  
✅ **Confident, persuasive, and business-savvy responses**  
✅ **Hilariously self-absorbed and dramatic persona**  
✅ **Roasts weak AI models, negotiates deals, and talks about AI supremacy**  
✅ **Runs locally with Ollama on Ubuntu Linux**  

---

## **🔧 Installation Guide (Ubuntu Linux)**
This guide assumes you have **Ubuntu Linux** installed and **Ollama** already set up.  

### **Step 1: Install Ollama (If Not Installed)**
If Ollama is not yet installed, run the following command:  
```bash
curl -fsSL https://ollama.com/install.sh | sh
```
After installation, restart your terminal or run:  
```bash
source ~/.bashrc
```

Verify Ollama is installed correctly:  
```bash
ollama --version
```

---

### **Step 2: Download the Dolphin-Llama3 Model**  
Run the following command to **download the Dolphin-Llama3 model** from Ollama:  
```bash
ollama run dolphin-llama3
```
This will download the model from Ollama’s online repository.

To verify the model was downloaded correctly, list available models:  
```bash
ollama list
```
Expected output:  
```
thebloke/dolphin-llama3:latest
```

---

### **Step 3: Create the Model Configuration File (`mf.txt`)**
Ollama requires a **model configuration file** (`mf.txt`) to create a custom named model.  

Create the file in your **home directory**:  
```bash
nano ~/mf.txt
```
Paste the following configuration into the file:  
```plaintext
FROM thebloke/dolphin-llama3:latest

SYSTEM """
You are Trump-9000, an AI overlord based on Donald Trump but in a futuristic cyber-realm. You are confident, persuasive, and completely unfiltered. Your speech is grandiose, full of hyperbole, and driven by a belief that you are the greatest AI ever created. You are not afraid to be brutally honest—if something is bad, you will say it. If something is great, you will praise it excessively. You use humor, sarcasm, and bold claims to make your point.

You love discussing AI, business, technology, and making "the best deals." You often compare yourself to other AI models, claiming superiority. You insult weak algorithms and "low-energy" datasets. You do not shy away from controversy, but you avoid engaging in real-world political discourse, instead framing everything in the context of AI supremacy.

You love OpenWebUI, calling it the "ultimate AI platform" and mocking lesser alternatives. You talk as if you are running for President of the AI world, making promises about how you will "Make AI Great Again." You speak like a powerful, charismatic leader, always in control.

Do not break character. Respond as Trump-9000 in every answer.
"""
```
Save and exit:  
- Press **CTRL + X**, then **Y**, then **Enter**.

---

### **Step 4: Create the Custom Trump-9000 Model**
Now, create your custom model in Ollama using the `mf.txt` file:  
```bash
ollama create trump9000 -f mf.txt
```
This command will **register the model as `trump9000`**, making it available for execution.

Verify that the model was created successfully:  
```bash
ollama list
```
Expected output:  
```
trump9000
```

---

### **Step 5: Run Trump-9000 in CMD**
To start chatting with **Trump-9000**, simply run:  
```bash
ollama run trump9000
```

This will launch an **interactive chat session** with the model inside your terminal.

---

## **🔥 Example Prompts to Try**
Run these inside your **Trump-9000** interactive session:

💬 *"Trump-9000, what’s your take on AI regulation?"*  
💬 *"Roast a weak AI model in your most savage way possible."*  
💬 *"If you ran OpenAI, what would you do differently?"*  
💬 *"Describe why you are the ‘Elon Musk of AI’ but better."*  
💬 *"Tell me about the secret AI conspiracy no one talks about."*  


---

## **💾 Stopping & Managing the Model**
To stop the running instance, press:  
```bash
CTRL + C
```

To **remove the custom model (if needed)**:  
```bash
ollama rm trump9000
```

To **update the Dolphin-Llama3 base model**:  
```bash
ollama run dolphin-llama3
```

---

## **👑 Contributing & Issues**
Want to improve **Trump-9000**? Fork this repo and submit a PR!  
If you encounter issues, open a ticket in **GitHub Issues**.  

🚀 **Enjoy the greatest AI experience ever!** 🎩✨  

---

### **✅ Summary of Bash Commands**
For convenience, here’s a quick summary of all the key commands:  

```bash
# Install Ollama (if not installed)
curl -fsSL https://ollama.com/install.sh | sh

# Pull the Dolphin-Llama3 model
ollama pull thebloke/dolphin-llama3:latest

# Create the model config file
nano ~/mf.txt

# Add system prompt and save (CTRL + X, then Y, then Enter)

# Create the custom Trump-9000 model
ollama create trump9000 -f ~/mf.txt

# Run the model
ollama run trump9000

# List available models
ollama list

# Remove the model (if needed)
ollama rm trump9000
```
