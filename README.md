# invoice_info_extractor_using_llama
 
 *The **Invoice Info Extractor Using LLama** tool is a Streamlit based app that uses LLAMA API to extract invoice info such as product name, price, purchase date, due date etc. from the invoice. The invoice is typically invoice about product purchased details.*<br>


# Invoice data processing LLM RAG on CPU with Ollama and ChromaDB

### RAG runs offline on local CPU
   
1. Install the requirements: 

```
pip install -r requirements.txt
```

2. Install <a href="https://ollama.ai">Ollama</a> and pull LLM model specified in config.yml

3. Copy text PDF files to the `data` folder.
   
4. Run the script, to convert text to vector embeddings and save in Chroma vector storage: 

```
python ingest.py
```

5. Run the script, to process data with LLM RAG and return the answer: 

```
python main.py "What is the client name?"
```