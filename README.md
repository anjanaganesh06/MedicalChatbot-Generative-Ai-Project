# Medical Chatbot

This work presents a medical chatbot built using the MedQuad dataset to assist in medical question answering.The data was preprocessed through lowercasing, removal of special characters, tokenization, stop-
word removal, and lemmatization. Structured features like tokenized words, original sentences, and question types were created and stored in a cleaned CSV format.Linguistic insights were gained via POS tagging and visualized through frequency plots. We trained Word2Vec embeddings and visualized them using t-SNE to capture semantic relationships betweenmedical terms.
For generation tasks, prompt engineering was applied on Gemini 1.5 flash model and the Flan-T5 model, and evaluation was performed using BLEU (1–4), ScareBLEU, ROUGE and F1 scores. Retrieval-augmented generation was enabled using ChromaDB vector store, allowing the model to fetch relevant information dynamically.
A multimodal(on text and images) agentic AI workflow was integrated using LangGraph to handle richer inputs. Finally,the TinyLlama/TinyLlama-1.1B-Chat-v1.0 model was fine-tuned on 100 curated medical QA pairs,improving domain-specific fluency and accuracy.
