# langchain-langgraph

--- 
### 1. Documentos (A Matéria-Prima)
São seus arquivos (PDFs, TXT, DOCX). Eles contêm o conhecimento bruto que a IA ainda não conhece, pois não fez parte do treinamento original dela.

### 2. Chunks ou Fragmentação (Recorte)
Como os documentos podem ser gigantes, o **LangChain** corta o texto em pedaços menores (ex: parágrafos de 500 caracteres).
> **Contexto:** É como cortar um livro em fichas bibliográficas para facilitar a localização de uma informação específica depois.

### 3. Embeddings (A Tradução para Números)
É um modelo matemático que transforma cada pedaço de texto em uma lista de números (vetores).
> **Contexto:** É a ponte entre a linguagem humana e a máquina. O "Embedding" entende que "cachorro" e "pet" são numericamente próximos, mesmo sendo palavras diferentes.

### 4. Vector Database / Vetorização (O Arquivo de Aço)
É o banco de dados onde esses números (vetores) ficam guardados e organizados por "vizinhança".
> **Contexto:** Imagine um mapa 3D onde assuntos parecidos moram no mesmo bairro. Isso permite que a busca seja instantânea.


### 5. Retrieval / Recuperação (A Busca por Similaridade)
Quando o usuário faz uma pergunta, ela também vira um vetor e o sistema vai ao banco buscar os "vizinhos" mais próximos.
> **Contexto:** É o "filtro" que separa o que é útil para aquela pergunta específica no meio de milhares de documentos.

### 6. RAG - Retrieval-Augmented Generation (A Estratégia)
É o nome de todo esse processo de "recuperar para gerar". É a técnica de dar um "livro aberto" para a IA consultar antes de responder.
> **Contexto:** Sem o RAG, a IA tenta adivinhar (alucinar). Com o RAG, ela consulta o fato antes de falar.

### 7. LiteLLM (O Tradutor Universal / Gateway)
Uma ferramenta que padroniza a conversa com diferentes "cérebros".
> **Contexto:** Ele serve para que o seu código fale uma língua só, não importa se você está usando o Ollama local ou uma IA paga na nuvem.

### 8. LLM - Large Language Model (O Cérebro)
É o motor (ex: Llama 3 via Ollama) que recebe o texto recuperado e a pergunta do usuário.
> **Contexto:** Ele não guarda os dados, ele apenas **processa**. Ele lê o que o RAG entregou e redige uma resposta coerente e educada.

---
