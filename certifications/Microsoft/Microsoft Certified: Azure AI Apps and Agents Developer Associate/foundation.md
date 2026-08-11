<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/Microsoft/microsoft-certified-associate-badge.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Microsoft Certified: Azure AI Apps and Agents Developer Associate</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Implement computer vision solutions](#implement-computer-vision-solutions) (4 questions)
- [Implement generative AI and agentic solutions](#implement-generative-ai-and-agentic-solutions) (10 questions)
- [Implement information extraction solutions](#implement-information-extraction-solutions) (4 questions)
- [Implement text analysis solutions](#implement-text-analysis-solutions) (4 questions)
- [Plan and manage an Azure AI solution](#plan-and-manage-an-azure-ai-solution) (8 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-08-11T02:42:19.704Z |
| Domains | 5 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Implement computer vision solutions | 4 |
| Implement generative AI and agentic solutions | 10 |
| Implement information extraction solutions | 4 |
| Implement text analysis solutions | 4 |
| Plan and manage an Azure AI solution | 8 |

---

### **Implement computer vision solutions**

### 1. Which Azure resource must be provisioned before an application can use Azure AI Video Retrieval?

- [ ] **A)** Azure AI Video Retrieval account
- [ ] **B)** Azure AI Vision (Computer Vision) resource
- [ ] **C)** Azure AI Custom Vision project
- [ ] **D)** Azure AI Document Intelligence resource

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Video Retrieval requires its own Azure AI Video Retrieval resource. A Computer Vision key cannot authenticate Video Retrieval endpoints.
 
 
</details>

### 2. Which visual features can be requested in an Image Analysis 4.0 call?

- [ ] **A)** denseCaptions
- [ ] **B)** tags
- [ ] **C)** smartCrops
- [ ] **D)** Categorize

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Image Analysis 4.0 supports denseCaptions, tags, and smartCrops. Categorize is a legacy feature and is not a valid visual feature in 4.0.
 
 
</details>

### 3. The code snippet uses the Image Analysis SDK to analyze an image. Which feature constant should replace the blank to detect objects with bounding boxes?

```python
from azure.ai.vision.imageanalysis import ImageAnalysisClient
from azure.ai.vision.imageanalysis.models import VisualFeatures
from azure.core.credentials import AzureKeyCredential

client = ImageAnalysisClient(endpoint, AzureKeyCredential(key))
result = client.analyze(image_url=image_url, visual_features=[VisualFeatures.___])
```

- [ ] **A)** OBJECTS
- [ ] **B)** TAGS
- [ ] **C)** READ
- [ ] **D)** PEOPLE

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The objects visual feature returns detected objects with names, confidence scores, and bounding boxes.
 
 
</details>

### 4. What additional information does object detection return that image tagging does not provide?

- [ ] **A)** Bounding box coordinates
- [ ] **B)** Confidence score
- [ ] **C)** Descriptive label
- [ ] **D)** Image-wide category

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Image tagging returns confidence-scored labels for the whole image, while object detection also returns bounding boxes that locate each detected object.
 
 
</details>


---

### **Implement generative AI and agentic solutions**

### 5. Which Azure service provides a unified project-based workspace for building and operationalizing generative AI applications?

- [ ] **A)** Azure AI Foundry
- [ ] **B)** Azure OpenAI Service
- [ ] **C)** Azure Machine Learning
- [ ] **D)** Azure AI Search

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure AI Foundry is the unified cloud platform for designing, developing, and operationalizing generative AI applications. Azure OpenAI Service handles model inference, not project-based app development.
 
 
</details>

### 6. Which two statements accurately describe Azure AI Foundry and Azure OpenAI Service?

- [ ] **A)** Azure AI Foundry provides the management and development plane for generative AI projects.
- [ ] **B)** Azure OpenAI Service is the inference plane that runs deployed OpenAI models.
- [ ] **C)** Azure AI Foundry makes Azure OpenAI Service unnecessary by running models directly in the hub.
- [ ] **D)** Azure OpenAI Service hosts the Azure AI Foundry evaluation dashboard and prompt flow designer.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure AI Foundry is the management and development plane, while Azure OpenAI Service is the inference plane. They are used together; Foundry does not replace OpenAI, and OpenAI does not host Foundry tooling.
 
 
</details>

### 7. Review the code snippet. In the Azure OpenAI SDK call, what does the value 'gpt-support' represent?

```python
from openai import AzureOpenAI
client = AzureOpenAI(
    azure_endpoint="https://contoso.openai.azure.com/",
    api_key=os.getenv("AZURE_OPENAI_API_KEY"),
    api_version="2024-12-01-preview"
)
response = client.chat.completions.create(
    model="gpt-support",
    messages=[{"role": "user", "content": "Hello"}]
)
```

- [ ] **A)** The deployment name
- [ ] **B)** The model family
- [ ] **C)** The resource name
- [ ] **D)** The API version

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In the Azure OpenAI SDK, the 'model' parameter receives the deployment name, not the base model name. The deployment name is defined when the model is deployed from the Azure AI Foundry model catalog.
 
 
</details>

### 8. Where does the deployment name appear in an Azure OpenAI REST API chat completion call?

- [ ] **A)** In the path after /openai/deployments/
- [ ] **B)** In the Authorization header
- [ ] **C)** In the request body as model_name
- [ ] **D)** In the query string as deployment

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The Azure OpenAI REST endpoint uses /openai/deployments/{deployment_name}/chat/completions. The deployment name is part of the URL path.
 
 
</details>

### 9. Which two authentication methods are supported for Azure AI services SDK clients?

- [ ] **A)** API key
- [ ] **B)** Microsoft Entra ID token
- [ ] **C)** Azure subscription ID
- [ ] **D)** Shared access signature

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure AI services support API keys and Microsoft Entra ID tokens. Subscription ID is not a credential, and shared access signatures are used for storage, not for Azure AI service clients.
 
 
</details>

### 10. Review the code snippet. Which Azure AI service is the target of this client?

```csharp
var client = new Azure.AI.OpenAI.AzureOpenAIClient(
    new Uri("https://contoso.openai.azure.com/"),
    new AzureKeyCredential(apiKey));
ChatClient chat = client.GetChatClient("gpt-4o-deployment");
```

- [ ] **A)** Azure OpenAI Service
- [ ] **B)** Azure AI Language
- [ ] **C)** Azure AI Vision
- [ ] **D)** Azure AI Search

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The namespace Azure.AI.OpenAI and the openai.azure.com endpoint identify Azure OpenAI Service. Other services use different namespaces and endpoints.
 
 
</details>

### 11. What is the primary purpose of a vector store in a RAG solution?

- [ ] **A)** To store embeddings and perform similarity search
- [ ] **B)** To cache chat responses
- [ ] **C)** To train a custom model
- [ ] **D)** To store user passwords securely

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Vector stores index embeddings and support similarity search. This enables retrieval of semantically relevant document chunks for grounding.
 
 
</details>

### 12. Which two Azure data services can be used as vector stores for RAG?

- [ ] **A)** Azure AI Search
- [ ] **B)** Azure Cosmos DB for MongoDB vCore
- [ ] **C)** Azure SQL Database
- [ ] **D)** Azure Blob Storage

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure AI Search and Azure Cosmos DB for MongoDB vCore support vector indexing. Azure SQL Database and Blob Storage do not provide native ANN vector indexes.
 
 
</details>

### 13. Review the code snippet. What does the value 5 specify in the vector search query?

```python
results = search_client.search(
    search_text=None,
    vector_queries=[{"kind": "vector", "vector": query_vector, "k": 5, "fields": "contentVector"}],
    select=["title", "content"]
)
```

- [ ] **A)** The number of nearest neighbor results returned
- [ ] **B)** The number of embedding dimensions
- [ ] **C)** The chunk size of documents
- [ ] **D)** The minimum similarity threshold

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> In Azure AI Search vector queries, 'k' is the top-k parameter that controls how many nearest neighbor results are returned.
 
 
</details>

### 14. What is the executable graph of LLM, Python, and tool nodes called in Azure AI Foundry?

- [ ] **A)** Prompt flow
- [ ] **B)** Batch run
- [ ] **C)** Variant
- [ ] **D)** Evaluator

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Prompt flow is the graph runtime in Azure AI Foundry. It connects LLM nodes, Python nodes, and tool nodes into an executable workflow.
 
 
</details>


---

### **Implement information extraction solutions**

### 15. Which Azure AI Document Intelligence model extracts fields from standard invoices and receipts without requiring training data?

- [ ] **A)** Prebuilt model
- [ ] **B)** Custom extraction model
- [ ] **C)** Custom classification model
- [ ] **D)** Layout model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Prebuilt models are trained on large sets of specific document types and require no training data.
 
 
</details>

### 16. Which outputs does the Azure AI Document Intelligence layout model return? Select all that apply.

- [ ] **A)** Text
- [ ] **B)** Tables
- [ ] **C)** Selection marks
- [ ] **D)** Key-value pairs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The layout model extracts text, tables, selection marks, and page-level details, but it does not extract key-value pairs.
 
 
</details>

### 17. In the provided C# code, what model identifier is passed to the document analysis operation?

```csharp
using System;
using Azure;
using Azure.AI.DocumentIntelligence;
using System.IO;

string endpoint = "https://myresource.cognitiveservices.azure.com/";
string apiKey = "my-key";

var client = new DocumentAnalysisClient(new Uri(endpoint), new AzureKeyCredential(apiKey));
using var stream = File.OpenRead("invoice.pdf");
var operation = client.AnalyzeDocument(WaitUntil.Completed, "prebuilt-invoice", stream);
AnalyzeResult result = operation.Value;
```

- [ ] **A)** prebuilt-receipt
- [ ] **B)** prebuilt-invoice
- [ ] **C)** prebuilt-id
- [ ] **D)** prebuilt-layout

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The code passes the identifier prebuilt-invoice to AnalyzeDocument, so the invoice prebuilt model is selected.
 
 
</details>

### 18. What is the minimum number of labeled documents required to train a custom extraction model in Azure AI Document Intelligence?

- [ ] **A)** 1
- [ ] **B)** 5
- [ ] **C)** 10
- [ ] **D)** 50

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Custom extraction models require at least five labeled documents; adding more labeled samples generally improves accuracy.
 
 
</details>


---

### **Implement text analysis solutions**

### 19. Which Azure AI Language feature identifies and redacts sensitive personal data such as credit card numbers?

- [ ] **A)** PII detection
- [ ] **B)** Named entity recognition
- [ ] **C)** Key phrase extraction
- [ ] **D)** Entity linking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> PII detection is designed to find and redact sensitive personal data for compliance scenarios.
 
 
</details>

### 20. Which two pieces of information are returned by the language detection API when analyzing text? Select all that apply.

- [ ] **A)** ISO 639-1 language code
- [ ] **B)** Confidence score
- [ ] **C)** Translated text
- [ ] **D)** Sentiment label

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Language detection returns an ISO 639-1 code and a confidence score; it does not translate text or return sentiment.
 
 
</details>

### 21. The Python code snippet contains a TODO comment for the method that returns the main talking points of a document. Which method should replace the TODO?

```python
documents = [{"id": "1", "text": "The support agent resolved my login issue quickly", "language": "en"}]
result = client.TODO(documents=documents)
```

- [ ] **A)** extract_key_phrases
- [ ] **B)** analyze_sentiment
- [ ] **C)** recognize_entities
- [ ] **D)** detect_language

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Key phrase extraction uses extract_key_phrases to identify the main talking points in a document.
 
 
</details>

### 22. Which type of Azure AI Language summarization returns only original sentences selected from the source document?

- [ ] **A)** Extractive summarization
- [ ] **B)** Abstractive summarization
- [ ] **C)** Custom NER
- [ ] **D)** PII detection

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Extractive summarization selects the most important original sentences, while abstractive summarization generates new text.
 
 
</details>


---

### **Plan and manage an Azure AI solution**

### 23. Which Azure AI service is primarily used for open-ended conversational and generative tasks?

- [ ] **A)** Azure OpenAI
- [ ] **B)** Azure AI Search
- [ ] **C)** Azure AI Document Intelligence
- [ ] **D)** Azure AI Content Safety

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure OpenAI provides GPT and o-series models for generative conversational tasks. Search is retrieval, Document Intelligence extracts forms, and Content Safety filters harmful content.
 
 
</details>

### 24. Which two Azure AI services are prebuilt, task-specific APIs for text and image analysis?

- [ ] **A)** Azure AI Language
- [ ] **B)** Azure AI Vision
- [ ] **C)** Azure OpenAI
- [ ] **D)** Azure AI Search

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Azure AI Language and Azure AI Vision are prebuilt APIs for specific text and image tasks. Azure OpenAI is generative, and Azure AI Search is an information retrieval service.
 
 
</details>

### 25. Review the code block. Which Azure AI service is being called to summarize text?

```python
from openai import AzureOpenAI
client = AzureOpenAI(azure_endpoint=endpoint, api_version='2024-10-21', api_key=key)
response = client.chat.completions.create(
    model='gpt-4o',
    messages=[{'role': 'user', 'content': 'Summarize this text.'}]
)
```

- [ ] **A)** Azure OpenAI
- [ ] **B)** Azure AI Language
- [ ] **C)** Azure AI Search
- [ ] **D)** Azure AI Content Safety

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code creates an AzureOpenAI client and sends a chat completion request to a GPT model, which is a generative Azure OpenAI workload.
 
 
</details>

### 26. What is the main purpose of Azure AI Search in a retrieval augmented generation solution?

- [ ] **A)** Grounding the model with relevant documents
- [ ] **B)** Generating natural language answers
- [ ] **C)** Moderating harmful content
- [ ] **D)** Transcribing audio input

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Azure AI Search indexes documents and supports keyword, vector, and hybrid retrieval, providing the grounding data that reduces hallucination in generative AI.
 
 
</details>

### 27. Which protections are included in Azure AI Content Safety? Choose all that apply.

- [ ] **A)** Hate speech detection
- [ ] **B)** Self-harm detection
- [ ] **C)** Jailbreak risk detection
- [ ] **D)** Personally identifiable information removal

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Azure AI Content Safety detects hate, self-harm, sexual content, violence, jailbreak risks, and prompt injection. PII removal is not a Content Safety capability.
 
 
</details>

### 28. The code block obtains an Azure token without using a stored secret. Which identity type is being used?

```python
from azure.identity import ManagedIdentityCredential
credential = ManagedIdentityCredential()
token = credential.get_token('https://cognitiveservices.azure.com/.default')
print(token.token)
```

- [ ] **A)** Managed identity
- [ ] **B)** API key
- [ ] **C)** Shared access signature
- [ ] **D)** Connection string

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The code uses ManagedIdentityCredential from the Azure Identity SDK, which obtains a token without storing any secret in application code.
 
 
</details>

### 29. In Azure AI Foundry, which component is the top-level administrative container that owns shared infrastructure?

- [ ] **A)** Hub
- [ ] **B)** Project
- [ ] **C)** Deployment
- [ ] **D)** Model

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The hub is the top-level administrative container in Azure AI Foundry. It owns shared infrastructure, and all projects under it inherit those settings.
 
 
</details>

### 30. Which resources are owned at the hub level and shared by projects in Azure AI Foundry? Choose all that apply.

- [ ] **A)** Key Vault
- [ ] **B)** Storage account
- [ ] **C)** Compute instances
- [ ] **D)** Project-specific evaluation datasets

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Key Vault, Storage account, and compute instances are hub-owned shared resources. Evaluation datasets are typically scoped to a project.
 
 
</details>
