---
marp: true
theme: default
class: invert
paginate: true

footer: "Stu Eggerton - September 2025"
html: true

allowlocalfiles: true


---
# GenAI for developers 

---
# 🤖 What is AI?

- **Artificial Intelligence (AI)** = Computers performing tasks that normally need human intelligence  
- **Key abilities:**
  - 📚 Learning & improving  
  - 🧠 Reasoning & decision-making  
  - 🗣️ Understanding language  
  - 👀 Recognizing patterns/images/sounds  
  - 🚗 Acting autonomously  😱😱😱

<!-- like giving a toddler the keys to your electric car or trusting your dog with your favourite food-->

---
# 🤖 What is AI NOT?

- 🔮 Magic  
- 🔪 A crazy that will replace everything we do

---
# 🤖 How is it going?
- People continue to overestimate AI
- We don't have General Artificial Intelligence Yet
- AI is helping us write documents, generate memes, use energy, generate code
- Hallucinations - a bad word for 

---
# 🤔 Why AI Won’t Replace Humans (Yet)

- 🎨 **Creativity & Imagination** → AI recombines patterns, humans invent  
- 🧠 **Common Sense & Context** → struggles with nuance & ambiguity  
- ❤️ **Emotions & Empathy** → simulates, but doesn’t *feel*  
- ⚖️ **Ethics & Values** → no built-in sense of right/wrong  
- 🌍 **Real-World Adaptability** → good in narrow tasks, poor in messy situations  

👉 **Bottom line:**  
AI = fast & scalable  
Humans = creative, ethical, adaptable  
**Together, they’re stronger.**

---
# 🧩 How Does an LLM Work?

- 📚 **Training**: Learns patterns from massive text datasets  
- 🔢 **Neural Networks**: Billions of parameters adjust to capture language structure  
- 🧮 **Tokenization**: Breaks text into tokens (chunks of words/characters)  
- 🎲 **Prediction**: For each token, predicts the *most likely* next token  
- 🔄 **Iteration**: Repeats prediction → builds sentences, paragraphs, conversations  
- 🚀 **Fine-tuning & Alignment**: Trained further to follow instructions, stay safe, and be useful  

👉 In short:  
LLMs don’t “know” like humans — they **predict patterns of language** based on data.  

---
# 📖 What is RAG?

- 🔍 **Retrieval**: Searches external knowledge (docs, databases, web)  
- 🧩 **Augmentation**: Injects retrieved info into the prompt  
- 🤖 **Generation**: LLM uses both context + knowledge to answer  

👉 **Why it matters:**  
- ✅ Reduces hallucinations  
- ✅ Keeps answers up-to-date  
- ✅ Combines AI reasoning with real data  

**In short:**  
RAG = *Search + AI* → More accurate, grounded answers  

---
# 🏗️ Preparing RAG

- 📚 **Collect Knowledge** → domain docs, PDFs, web pages, FAQs  
- ✂️ **Chunking** → split into small, retrievable pieces  
- 🔤 **Embedding** → convert chunks into vector representations  
- 🏦 **Vector Database** → store embeddings for fast semantic search  


---
# 🪜 Steps of a RAG query
🔍 **Retrieval** → find the most relevant chunks at query time  
↓
🧩 **Augmentation** → inject retrieved context into the prompt  
↓
🤖 ** LLM Generation** → LLM produces grounded Grounded Response ✅ 

<br/>
<br/><br/>
👉 **Result:** AI that reasons with real data instead of just memory  

---
# Solution on a Page and demo