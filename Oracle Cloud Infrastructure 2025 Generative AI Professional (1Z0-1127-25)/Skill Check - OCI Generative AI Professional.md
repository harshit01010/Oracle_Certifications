# Skill Checks
## Fundamentals of Large Language Models


1. What does in-context learning in Large Language Models involve?
- [ ] Adding more layers to the model
- [x] Conditioning the model with task-specific instructions or demonstrations
- [ ] Training the model using reinforcement learning
- [ ] Pretraining the model on a specific domain

> In-context learning in Large Language Models (LLMs) involves updating or fine-tuning a pretrained language model with additional data or examples specific to a particular context or domain. This process enables the model to adapt its knowledge and capabilities to better suit the requirements of a specific task or application.


2. Which statement accurately reflects the differences between these approaches in terms of the number of parameters modified and type of data
used?
- [ ] Soft Prompting and Continuous Pretraining are both methods that require no modification to the original parameters of the model.
- [x] Fine-tuning modifies all parameters using labeled, task-specific data, while Parameter Efficient Fine-Tuning updates a few, new parameters
also with labeled, task-specific data.
- [ ] Parameter Efficient Fine-Tuning and Soft Prompting modify all parameters of the model using unlabeled data.
- [ ] Fine-tuning and Continuous Pretraining both modify all parameters and use labeled, task-specific data.

> Fine-tuning involves adjusting all parameters of the pretrained model using labeled, task-specific data. This means that the entire model architecture is modified based on the new task or domain-specific data. Parameter Efficient Fine-Tuning updates only a subset of parameters within the pretrained model, typically focusing on specific layers or components that are relevant to the new task. Despite this, both Fine-tuning and Parameter Efficient Fine-Tuning utilize labeled, task-specific data for training.


3. What is the role of temperature in the decoding process of an LLM?
- [ ] To decide which part of speech the next word should belong to
- [ ] To increase the accuracy of the most likely word in the vocabulary
- [x] To adjust the sharpness of the probability distribution over the vocabulary when selecting the next word
- [ ] To determine the number of words to generate in a single decoding step

> When decoding with an LLM, the model assigns probabilities to each word in the vocabulary for the next word in the sequence. Temperature controls the sharpness or smoothness of this probability distribution. A low temperature value results in a sharper distribution, meaning that the model is more confident in its predictions and tends to select the most likely word with higher probability. Conversely, a higher temperature value smooths out the distribution, making it more likely for lower probability words to be chosen, leading to more diverse and varied output.


4. What is prompt engineering in the context of Large Language Models (LLMs)?
- [x] iteratively refining the ask to elicit a desired response
- [ ] Adjusting the hyperparameters of the model
- [ ] Adding more layers to the neural network
- [ ] Training the model on a large dataset

> Prompt engineering in the context of Large Language Models (LLMs) refers to the practice of designing and refining prompts or input instructions to elicit desired responses from the model. It involves crafting specific textual cues or queries that guide the model towards generating outputs that align with the user's intentions or requirements.


5. What does the term "hallucination" refer to in the context of Large Language Models (LLMs)?
- [ ] The process by which the model visualizes and describes images in detail
- [x] The phenomenon where the model generates factually incorrect information or unrelated content as if it were true
- [ ] A technique used to enhance the model's performance on specific tasks
- [ ] The model's ability to generate imaginative and creative content

> Hallucination occurs when the model generates text that seems plausible or coherent but is not grounded in factual reality or relevant to the task at hand. Hallucination can be problematic, especially in applications where generating accurate and reliable information is crucial, such as question answering, summarization, or content generation for decision-making.


## Generative AI Service

1. What happens if a period (.) is used as a stop sequence in text generation?
- [ ] The model stops generating text after it reaches the end of the current paragraph.
- [ ] The model ignores periods and continues generating text until it reaches the token limit.
- [ ] The model generates additional sentences to complete the paragraph.
- [x] The model stops generating text once it reaches the end of the first sentence, even if the token limit is much higher.

> Stop sequences, in the context of text generation, are special tokens or symbols used to signal the end of the generated text. These sequences serve as markers for the model to halt its generation process. Common stop sequences include punctuation marks such as periods (.), question marks (?), and exclamation marks (!), as they typically denote the end of sentences in natural language.


2. What is a distinctive feature of GPUs in Dedicated Al Clusters used for generative Al tasks?
- [ ] Each customer's GPUs are connected via a public internet network for ease of access.
- [x] GPUs allocated for a customer's generative Al tasks are isolated from other GPUs.
- [ ] GPUs are shared with other customers to maximize resource utilization.
- [ ] GPUs are used exclusively for storing large datasets, not for computation.

> The GPUs allocated for a customer’s generative AI tasks are isolated from other GPUs to maintain the security and privacy of customer data and workloads.


3. What is the purpose of frequency penalties in language model outputs?
- [ ] To randomly penalize some tokens to increase the diversity of the text
- [x] To penalize tokens that have already appeared, based on the number of times they've been used
- [ ] To reward the tokens that have never appeared in the text
- [ ] To ensure tokens that appear frequently are used more often

> Frequency penalties in language model outputs aim to discourage the repetition of tokens that have already appeared in the generated text. When generating text, language models may tend to produce repetitive phrases or words, which can lead to less diverse and less interesting outputs. By applying frequency penalties, tokens that have been used multiple times are penalized, reducing the likelihood of their repetition in subsequent generations.


4. What is the main advantage of using few-shot model prompting to customize a Large Language Model (LLM)?
- [ ] It allows the LLM to access a larger dataset.
- [ ] It significantly reduces the latency for each model request.
- [x] It provides examples in the prompt to guide the LLM to better performance with no training cost.
- [ ] It eliminates the need for any training or computational resources.

> The main advantage of using few-shot model prompting to customize a Large Language Model (LLM) is its ability to adapt the model quickly and effectively to new tasks or domains with only a small amount of training data. Instead of retraining the entire model from scratch, which can be time-consuming and resource-intensive, few-shot prompting leverages the model's pre-existing knowledge.


5. What is the purpose of embeddings in natural language processing?
- [ ] To increase the complexity and size of text data
- [ ] To compress text data into smaller files for storage
- [ ] To translate text into a different language
- [x] To create numerical representations of text that capture the meaning and relationships between words or phrases

> Embeddings map words or text on to a continuous vector space where similar words are located close to each other. This allows NLP models to capture semantic relationships between words, such as synonyms or related concepts. For example, in a well-trained embedding space, the vectors for "king" and "queen" would be closer to each other than to unrelated words like "car" or "tree." Embeddings also provide a dense, low-dimensional representation of words compared to traditional one-hot encodings. This makes them more efficient and effective as input features for machine learning models, reducing the dimensionality of the input space, and improving computational efficiency.


##  RAG Using Generative AI Service and Oracle 23ai Vector Search

1. What is a key characteristic of Large Language Models (LLMs) without Retrieval Augmented Generation (RAG)?
- [ ] They always use an external database for generating responses.
- [ ] They cannot generate responses without Fine-Tuning.
- [x] They rely on internal knowledge learned during pretraining on a large text corpus.
- [ ] They use vector databases exclusively to produce answers.

> Large Language Models (LLMs) without Retrieval Augmented Generation (RAG) primarily rely on internal knowledge learned during pretraining on a large text corpus. These models are trained on vast amounts of text data, which enables them to learn complex patterns, structures, and relationships within language.


2. What is the purpose of memory in the LangChain framework?
- [ ] To retrieve user input and provide real-time output only
- [ ] To act as a static database for storing permanent records
- [ ] To perform complex calculations unrelated to user interaction
- [x] To store various types of data and provide algorithms for summarizing past interactions

> In the LangChain framework, memory serves as a dynamic repository for retaining and managing information throughout the system's operation. It allows the framework to maintain state and context, enabling chains to access, reference, and utilize past interactions and information in their decision-making processes.


3. How are prompt templates typically designed for language models?
- [x] As predefined recipes that guide the generation of language model prompts
- [ ] To only work with numerical data instead of textual content
- [ ] As complex algorithms that require manual compilation
- [ ] To be used without any modification or customization

> Prompt templates for language models are typically designed as predefined recipes that guide the generation of prompts. By using predefined templates, developers can ensure consistency and coherence in the prompts generated for the language model. These templates may include placeholders or variables representing different components of the prompt, such as user queries, context, or response options.


4. What differentiates semantic search from traditional keyword search?
- [ ] it depends on the number of times keywords appear in the content.
- [x] It involves understanding the intent and context of the search.
- [ ] It is based on the date and author of the content.
- [ ] It relies solely on matching exact keywords in the content.

> Semantic search differs from traditional keyword search in that it involves understanding the intent and context of the search query, rather than relying solely on matching exact keywords in the content.


5. What is the LCEL in the context of LangChain chains?
- [ ] A programming language used to write documentation for LangChain
- [ ] An older Python library for building Large Language Models
- [ ] A legacy method for creating chains in LangChain
- [x] A declarative way to compose chains together using LangChain Expression Language

> LECL, or LangChain Expression Language, is a declarative way to compose chains together within the LangChain framework. It provides a structured and expressive syntax for defining the composition of chains, specifying the sequence of components and their interactions in a clear and concise manner.


## Chatbot Using Generative AI Agent Service


1. What happens when you restart a previously run ingestion job in OCI Generative Al Agents?
- [ ] The entire process stops if a single file fails.
- [x] Only files that failed in the earlier attempt and have since been updated are ingested.
- [ ] Only new files added to the bucket are ingested.
- [ ] All files are re-ingested, regardless of previous success.

> When you restart a previously run ingestion job, the pipeline detects files that were successfully ingested earlier and skips them. It only ingests files that failed previously and have since been updated.


2. In the context of OCI Generative Al Agents, what does "Groundedness" mean?
- [ ] The model's reliance on human feedback to improve its training
- [ ] The model's ability to maintain a continuous conversation context
- [x] The model's ability to generate responses that can be traced back to data sources
- [ ] The model's focus on generating creative responses grounded in imagination

> In the context of OCI Generative AI Agents, "groundedness" refers to the model's capability to produce responses that are accurate, reliable, and verifiable by being based on specific and identifiable data sources. 


3. How should you handle a data source in OCI Generative Al Agents if your data is not ready yet?
- [ ] Upload placeholder files larger than 100 MB as a temporary solution.
- [x] Create an empty folder for the data source and populate it later.
- [ ] Leave the data source configuration incomplete until the data is ready.
- [ ] Use multiple buckets to store the incomplete data.

> If your data isn't available yet, create an empty folder for the data source and populate it later. This way, you can ingest data into the source after the folder is populated.


4. What is the maximum number of endpoints you can create per agent by default in OCI Generative Al Agents?
- [ ] 5
- [ ] 1
- [x] 3
- [ ] 2

> Number of endpoints that you can create for each agent is 3.


5. Which field is optional when setting up the Oracle Database 23ai table for Generative Al Agents?
- [ ] DOCID
- [ ] VECTOR
- [x] TITLE
- [ ] BODY

> DOCID, BODY, and VECTOR are required fields while TITLE is an optional field for creating an Oracle Database 23ai table.

<br />


***