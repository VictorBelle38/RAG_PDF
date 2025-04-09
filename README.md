# 📚 RAG com PDF usando GROQ, Pinecone e Cohere

Este é um projeto educacional com o objetivo de demonstrar como utilizar a técnica de **RAG (Retrieval-Augmented Generation)** para responder perguntas com base no conteúdo de um **PDF**, utilizando ferramentas modernas de IA.

## 🎯 Objetivo

Permitir que um usuário faça perguntas em linguagem natural e receba respostas geradas com base nas informações contidas em um documento PDF. A ideia é unir **busca semântica** e **geração de texto** para oferecer respostas contextuais e precisas.

## ⚙️ Como funciona

1. O conteúdo do PDF é lido e dividido em pequenos trechos (chunks).
2. Esses trechos são transformados em vetores numéricos com **Cohere** (embeddings).
3. Os vetores são armazenados em um índice vetorial no **Pinecone**.
4. Quando uma pergunta é feita, ela também é transformada em vetor.
5. O vetor da pergunta é comparado com os vetores dos trechos do PDF para encontrar os mais relevantes.
6. Os trechos encontrados são enviados, junto com a pergunta, para um modelo LLM da **GROQ**, que gera uma resposta em linguagem natural com base nessas informações.

## 🧠 Tecnologias utilizadas

- **Python** – Linguagem principal do projeto
- **PyPDFLoader ** – Extração de texto do PDF
- **Cohere** – Geração de embeddings (representações vetoriais dos textos)
- **Pinecone** – Armazenamento e recuperação vetorial de dados
- **GROQ** – Provedor de LLMs para geração de respostas baseadas nos dados recuperados
- **dotenv** – Gerenciamento seguro de chaves e variáveis de ambiente

## 📌 Aplicação

Este projeto é voltado para aprendizado prático de conceitos fundamentais de RAG e integração entre LLMs e bases vetoriais. É uma ótima introdução para quem deseja explorar o uso de IA generativa com dados personalizados.

## 👨‍💻 Autor

Desenvolvido por [Seu Nome] como parte do aprendizado em aplicações de IA generativa com foco em NLP e recuperação de informações.
