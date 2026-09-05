<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Oracle/Oracle%20Cloud%20Infrastructure%202026%20Generative%20AI%20Professional.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Oracle Cloud Infrastructure 2026 Generative AI Professional</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Fundamentals of Large Language Models](#fundamentals-of-large-language-models) (6 questions)
- [Implement RAG using OCI Generative AI Service](#implement-rag-using-oci-generative-ai-service) (6 questions)
- [Using OCI Generative AI RAG Agents Service](#using-oci-generative-ai-rag-agents-service) (6 questions)
- [Using OCI Generative AI Service](#using-oci-generative-ai-service) (12 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:46:15.751Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Fundamentals of Large Language Models | 6 |
| Implement RAG using OCI Generative AI Service | 6 |
| Using OCI Generative AI RAG Agents Service | 6 |
| Using OCI Generative AI Service | 12 |

---

### **Fundamentals of Large Language Models**

### 1. What is a large language model (LLM)?

- [ ] **A)** A neural network trained on massive text data to understand and generate language
- [ ] **B)** A database that stores prewritten responses
- [ ] **C)** A list of hand-coded grammatical rules
- [ ] **D)** A program that only recognizes images

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> LLMs are neural networks trained on massive text corpora. They learn statistical patterns in language and can generate coherent text. Databases, rule systems, and image classifiers are not LLMs.
 
 
</details>

### 2. Which of the following are core characteristics of large language models? Select all that apply.

- [ ] **A)** They are pretrained on large collections of text.
- [ ] **B)** They are often based on transformer architectures.
- [ ] **C)** They generate text by predicting likely next tokens.
- [ ] **D)** They require a labeled dataset for every new task.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> LLMs are pretrained on large text corpora, usually use transformer architectures, and generate text by predicting next tokens. They support transfer learning and do not require labeled data for every new task.
 
 
</details>

### 3. Review the Python code in the code block. What is the primary task of the loaded pipeline in this script?

```python
from transformers import pipeline

generator = pipeline('text-generation', model='gpt2')
prompt = 'The future of AI is'
output = generator(prompt, max_length=20, num_return_sequences=1)
print(output[0]['generated_text'])
```

- [ ] **A)** Generate a continuation of the prompt text
- [ ] **B)** Classify the sentiment of the prompt
- [ ] **C)** Translate the prompt into another language
- [ ] **D)** Summarize the prompt in one sentence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The pipeline is created with the text-generation task. It receives the prompt and returns a model-generated continuation. This is not classification, translation, or summarization.
 
 
</details>

### 4. What does the self-attention mechanism allow a transformer model to do?

- [ ] **A)** Determine how relevant each token is to other tokens
- [ ] **B)** Store all text in a key-value database
- [ ] **C)** Apply punctuation rules to every sentence
- [ ] **D)** Convert text into a fixed-size image

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Self-attention computes relationships between all tokens in a sequence. It tells the model how much each token should influence the representation of another token.
 
 
</details>

### 5. Which statements about tokenization in LLMs are correct? Select all that apply.

- [ ] **A)** A tokenizer splits text into words or subword units.
- [ ] **B)** The tokenizer maps tokens to numeric IDs before model input.
- [ ] **C)** LLMs have a fixed vocabulary size defined by the tokenizer.
- [ ] **D)** Each token always represents exactly one character.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Tokenizers convert text into word or subword tokens and then to numeric IDs. Each model has a fixed vocabulary. A token is not limited to one character.
 
 
</details>

### 6. When the code block runs, which statements are true about the text generation logic? Select all that apply.

```python
import torch
from transformers import AutoTokenizer, AutoModelForCausalLM

tokenizer = AutoTokenizer.from_pretrained('gpt2')
model = AutoModelForCausalLM.from_pretrained('gpt2')

def generate(prompt, max_tokens=20):
    input_ids = tokenizer(prompt, return_tensors='pt').input_ids
    for _ in range(max_tokens):
        logits = model(input_ids).logits[:, -1, :]
        next_token_id = logits.argmax(dim=-1)
        input_ids = torch.cat([input_ids, next_token_id.unsqueeze(0)], dim=-1)
    return tokenizer.decode(input_ids[0])
```

- [ ] **A)** The generation loop repeats for max_tokens iterations.
- [ ] **B)** At each step, argmax selects the token with the highest predicted score.
- [ ] **C)** This strategy is equivalent to random top-k sampling.
- [ ] **D)** The decoded result contains the original prompt and the generated tokens.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> The loop executes max_tokens times, uses argmax over the final logits to choose the highest probability token, and decodes the concatenated prompt and generated tokens. It is deterministic, not random sampling.
 
 
</details>


---

### **Implement RAG using OCI Generative AI Service**

### 7. When a large language model trains on text data, what core statistical relationship does it primarily learn?

- [ ] **A)** SQL schema for storing relational tables
- [ ] **B)** Physical data center geographic coordinates
- [ ] **C)** Probability of the next token given previous tokens
- [ ] **D)** Network packet routing table settings

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> An LLM learns statistical relationships between tokens, estimating the most probable next token from prior tokens. This next-token prediction underlies its text generation.
 
 
</details>

### 8. Which capabilities of a large language model directly contribute to answering a query using retrieved context in RAG?

- [ ] **A)** Generating coherent text conditioned on context
- [ ] **B)** Performing low-level disk storage compression
- [ ] **C)** Learning semantic patterns in natural language
- [ ] **D)** Executing embedding index scans automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> An LLM contributes language generation and semantic understanding, while vector index scans and storage compression are handled by supporting infrastructure, not the model.
 
 
</details>

### 9. Review the code sample and identify the role of the object created before any text generation request is made.

```python
import oci
from oci.generative_ai_inference import GenerativeAiInferenceClient

config = oci.config.from_file()
generative_ai_client = GenerativeAiInferenceClient(config)
```

- [ ] **A)** Creates a virtual cloud network
- [ ] **B)** Manages API calls to OCI Generative AI
- [ ] **C)** Configures an object storage bucket
- [ ] **D)** Deletes model fine-tuning jobs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code imports GenerativeAiInferenceClient and constructs a client from OCI config, enabling calls to the OCI Generative AI inference service.
 
 
</details>

### 10. When text is provided to a large language model, what is the term used to describe a single text unit such as a subword?

- [ ] **A)** Authentication key for the inference API
- [ ] **B)** Container instance in a compute cluster
- [ ] **C)** Smallest text unit processed by the model
- [ ] **D)** SQL statement used to query the database

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> A token is a discrete text unit, usually a word, subword, or character segment, created by a tokenizer before the model computes token probabilities.
 
 
</details>

### 11. Which statements correctly describe how the temperature parameter influences text output from a large language model?

- [ ] **A)** Controls how random the generated text is
- [ ] **B)** Always increases generated response length
- [ ] **C)** Sets the maximum input context size
- [ ] **D)** Lower values generally produce more deterministic outputs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, D**
 
> 💡  **Explanation** 
> 
> Temperature affects the token probability distribution used during sampling. Lower values make outputs more focused and deterministic, while higher values increase randomness; it does not control length.
 
 
</details>

### 12. Which of the following best describes the main goal of the code sample in preparing content for RAG retrieval?

```python
def prepare_documents(documents):
    embeddings = embed_documents(documents)
    vector_index.add(embeddings)
    return vector_index
```

- [ ] **A)** Creates a backup of the source files
- [ ] **B)** Employs embeddings to enable semantic search
- [ ] **C)** Encrypts documents with a symmetric key
- [ ] **D)** Compiles code into a deployable artifact

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Embedding models convert documents into vector representations. Storing these vectors in an index enables the retriever to find semantically relevant passages for a user query.
 
 
</details>


---

### **Using OCI Generative AI RAG Agents Service**

### 13. What is the fundamental role of a large language model (LLM) inside an OCI Generative AI RAG agent?

- [ ] **A)** It generates the final answer in natural language based on retrieved context.
- [ ] **B)** It creates vector indexes for all source documents.
- [ ] **C)** It routes API traffic between the agent and OCI services.
- [ ] **D)** It enforces IAM policies on the knowledge base.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The LLM is the generator in a RAG pipeline: it receives the user prompt plus retrieved documents and produces a natural-language answer. Indexing, routing, and security are separate concerns.
 
 
</details>

### 14. Which elements are necessary for the retrieval-augmented generation (RAG) pattern to work with OCI Generative AI Agents?

- [ ] **A)** A source of knowledge, such as PDFs or web pages, indexed as a knowledge base.
- [ ] **B)** A retriever that searches the indexed content for relevant textual chunks.
- [ ] **C)** A generative LLM that composes an answer from the retrieved chunks.
- [ ] **D)** A physical database server deployed in the customer's data center.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> RAG must combine an indexed knowledge base, a retrieval step, and a generator LLM. No on-premises physical server is required because OCI provides managed services.
 
 
</details>

### 15. Review the inference parameters in the code block. How should you adjust the configuration to obtain more consistent, less random answers from the OCI Generative AI model?

```python
inference_params = {
    "temperature": 0.7,
    "top_p": 0.9,
    "max_tokens": 200
}
```

- [ ] **A)** Lower the temperature from 0.7 to 0.1.
- [ ] **B)** Raise the temperature from 0.7 to 1.5.
- [ ] **C)** Change max_tokens from 200 to 50.
- [ ] **D)** Set top_p to 1.0.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Sampling parameters, especially temperature, control randomness. Lowering temperature sharpens the model's token distribution and makes responses more consistent.
 
 
</details>

### 16. In an OCI RAG knowledge base, what representation is used to search for semantically similar text?

- [ ] **A)** Numerical vector embeddings of text chunks.
- [ ] **B)** Raw PDF files as originally uploaded.
- [ ] **C)** SQL queries from user sessions.
- [ ] **D)** Training weights from the foundation model.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Documents are chunked, and each chunk is converted into an embedding vector. The retriever measures embedding similarity to find semantically related passages.
 
 
</details>

### 17. Which statements about the knowledge base in an OCI Generative AI RAG agent are correct?

- [ ] **A)** Documents are normally broken into smaller chunks before indexing.
- [ ] **B)** Embedding models generate vector representations for the text.
- [ ] **C)** Search results are ranked based on semantic similarity.
- [ ] **D)** User queries must contain the exact keywords from the original document.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The RAG knowledge base pipeline uses chunking, embeddings, and similarity search. Retrieval is semantic, so exact keyword matching is unnecessary.
 
 
</details>

### 18. You run the OCI Generative AI Agents CLI command shown in the code block. Which conditions must hold for the agent to use RAG against your enterprise knowledge base?

```bash
oci generative-ai-agent chat --agent-endpoint-id "ocid1.genaiagentendpoint.oc1.iad.xxx" --session-id "ocid1.genaiagentsession.oc1.iad.yyy" --user-message "What does the OCI security guide say about encryption?"
```

- [ ] **A)** The agent endpoint must be associated with a configured knowledge base.
- [ ] **B)** The session ID must correspond to an existing session that is valid for the agent endpoint.
- [ ] **C)** The user's message must match the exact title of a stored document.
- [ ] **D)** The agent endpoint must be publicly accessible without authentication.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RAG relies on the endpoint's linked knowledge base and session context. It does not require exact title matching, and the endpoint must not be unauthenticated.
 
 
</details>


---

### **Using OCI Generative AI Service**

### 19. What is the main function of a large language model in generative AI?

- [ ] **A)** Text predictor trained on massive data
- [ ] **B)** Application for entering numerical data
- [ ] **C)** Relational database management system
- [ ] **D)** Routing protocol for cloud networks

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A large language model learns language patterns from massive text corpora to generate coherent and contextually relevant text.
 
 
</details>

### 20. Which two components are considered foundational to how large language models process text?

- [ ] **A)** Tokenization
- [ ] **B)** Attention mechanism
- [ ] **C)** Indexing
- [ ] **D)** Compression

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> LLMs process text into tokens and use attention mechanisms to understand the relationships among those tokens during generation.
 
 
</details>

### 21. What is the action performed by the code block when the client method is called?

```python
client.generate_text(
    model_id="cohere.command",
    prompt="Explain OCI Generative AI in two sentences."
)
```

- [ ] **A)** Calling a model to generate text
- [ ] **B)** Creating an object storage bucket
- [ ] **C)** Deleting a compute instance
- [ ] **D)** Provisioning a load balancer

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code sends a prompt to the model and receives generated text as the response.
 
 
</details>

### 22. What is the meaning of token when used by large language models during text processing?

- [ ] **A)** Subword unit of text
- [ ] **B)** CPU cache memory
- [ ] **C)** Row in a SQL table
- [ ] **D)** Network packet header

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A token is a basic text unit, typically a word or subword, used as the model's smallest processing element.
 
 
</details>

### 23. Which two model parameters control the randomness of generated text during inference?

- [ ] **A)** Temperature
- [ ] **B)** Top-p
- [ ] **C)** Thread count
- [ ] **D)** Batch size

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Temperature and top-p control sampling randomness, making generated text more diverse or more focused depending on their values.
 
 
</details>

### 24. What is the intended outcome of the function call shown in the code block?

```python
models = client.list_models(compartment_id=compartment_id)
for model in models.data:
    print(model.id)
```

- [ ] **A)** List available language models
- [ ] **B)** Generate a text response
- [ ] **C)** Store result in a database
- [ ] **D)** Configure an identity policy

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code calls the model listing operation to show accessible language models in the compartment.
 
 
</details>

### 25. What does the context window of a large language model represent in a generation task?

- [ ] **A)** Maximum tokens considered for generation
- [ ] **B)** Amount of free memory on a GPU
- [ ] **C)** Number of layers in the neural network
- [ ] **D)** Time required to train a model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The context window defines the maximum number of tokens the model can consider when producing a response.
 
 
</details>

### 26. Which two common tasks can a generative AI text model effectively perform?

- [ ] **A)** Text summarization
- [ ] **B)** Language translation
- [ ] **C)** Disk partitioning
- [ ] **D)** SSH key generation

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> LLMs are commonly used for summarization and translation, where they generate fluent and context-aware text.
 
 
</details>

### 27. In the code block, what is the result of setting the temperature parameter to zero?

```python
client.generate_text(
    model_id="cohere.command",
    prompt="Suggest a cloud architecture",
    temperature=0
)
```

- [ ] **A)** More deterministic response
- [ ] **B)** Fully random response
- [ ] **C)** Guaranteed longer output
- [ ] **D)** No model inference

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A temperature of zero makes sampling more deterministic, leading to more predictable model output.
 
 
</details>

### 28. What is meant by hallucination when a large language model produces an answer?

- [ ] **A)** Plausible but incorrect information
- [ ] **B)** Text copied exactly from a database
- [ ] **C)** Intentional security alert
- [ ] **D)** Network timeout error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A hallucination is generated content that appears fluent and credible but is not grounded in facts.
 
 
</details>

### 29. Which two methods can reduce hallucination by providing the model with relevant external information?

- [ ] **A)** Retrieval augmented generation
- [ ] **B)** Grounding with source documents
- [ ] **C)** Raising temperature to maximum
- [ ] **D)** Removing all context

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RAG and grounding give the model relevant source context, reducing unsupported or invented answers.
 
 
</details>

### 30. What is the main purpose of the embedding operation shown in the code block?

```python
embeddings = client.embed_text(
    model_id="cohere.embed-english-v3",
    texts=["OCI provides managed AI services"]
)
print(embeddings)
```

- [ ] **A)** Convert text into vector embeddings
- [ ] **B)** Generate new tokens from a prompt
- [ ] **C)** Backup files to object storage
- [ ] **D)** Create an IAM group

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Embedding transforms text into dense numeric vectors used for semantic similarity and retrieval.
 
 
</details>
