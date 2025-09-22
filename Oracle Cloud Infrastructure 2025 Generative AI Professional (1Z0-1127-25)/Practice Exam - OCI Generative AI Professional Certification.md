# OCI Generative AI Professional Certification
## Practice Exam


1. In the simplified workflow for managing and querying vector data, what is the role of indexing?
- [ ] Converting vectors into a non-indexed format for easier retrieval
- [x] Mapping vectors to a data structure for faster searching, enabling efficient retrieval
- [ ] Compressing vector data for minimized storage usage
- [ ] Categorizing vectors based on their originating data type (text, images, audio)

> Indexing in vector databases is crucial for optimizing search efficiency by organizing vectors in a way that allows fast and approximate nearest neighbor (ANN) searches. It maps vectors into data structures like HNSW (Hierarchical Navigable Small World), FAISS, or IVF (Inverted File Index), significantly reducing search time compared to brute-force comparisons. This is essential for scaling semantic search and retrieval-augmented generation (RAG) applications.


2. A marketing team is using Oracle's Generative AI service to create promotional content. They want to generate consistent responses for the same prompt across multiple runs to ensure uniformity in their messaging. They notice that the responses vary each time they run the model, despite keeping the prompt and other parameters the same.\
chat_request.seed = None \
chat_request.temperature = 0 \
chat_request.frequency_penalty = 1 \
chat_request.top_p = 0.75 \
Which parameter should they modify to ensure identical outputs for the same input?
- [ ] temperature
- [ ] top_p
- [x] seed
- [ ] frequency_penalty

> The seed parameter ensures that the model generates deterministic outputs. By setting a fixed seed value (e.g., 123), the model will consistently produce the same response for the same input prompt and parameters. Leaving it as None allows the model to generate varied responses each time. temperature, frequency_penalty, and top_p control aspects of the text generation process, but they do not enforce consistency across multiple runs.


3. When activating content moderation in OCI Generative AI Agents, which of these can you specify?
- [ ] The threshold for language complexity in responses
- [x] Whether moderation applies to user prompts, generated responses, or both
- [ ] The maximum file size for input data
- [ ] The type of vector search used for retrieval

> Moderation is applied to: User prompt (input) Generated response (output) Both input and output


4. endpoint = *"https://inference.generativeai.eu-frankfurt-1.oci.oraclecloud.com"* \
What is the purpose of this _endpoint_ variable in the code?
- [ ] It stores the OCI API key required for authentication.
- [ ] It sets the retry strategy for the inference client.
- [x] It defines the URL of the OCI Generative AI inference service.
- [ ] It specifies the availability domain where the OCI Generative AI model is hosted, ensuring inference happens in the correct region.

> The endpoint variable stores the URL where requests to Oracle's Generative AI inference service are sent. This endpoint acts as the gateway to communicate with the AI model hosted in the specified region.


5. What is the role of the _OnDemandServingMode_ in the following code snippet? \
`chat_detail.serving_mode = oci.generative_ai_inference.models.OnDemandServingMode(model_id="ocid1.generativeaimodel.oc1.eu-frankfurt-1.xxxxxxxxxxxxxxxxxxxxxx")`
- [x] It specifies that the Generative AI model should serve requests only on demand, rather than continuously.
- [ ] It configures the model to use batch processing for requests.
- [ ] It defines the retry strategy for handling failures during model inference.
- [ ] It initializes the model with the default configuration profile for inference.

> The OnDemandServingMode is used to configure the Generative AI model to handle requests on-demand, which is suitable for use cases where requests are sporadic or less frequent.

6. Which fine-tuning methods are supported by the *cohere.command-r-08-2024* model in OCI Generative AI?
- [ ] LoRA and Vanilla
- [ ] T-Few and Vanilla
- [ ] T-Few, LoRA, and Vanilla
- [x] T-Few and LoRA

> The cohere.command-r-08-2024 model supports the T-Few and LoRA fine-tuning methods.

7. What does a cosine distance of 0 indicate about the relationship between two embeddings?
- [ ] They have the same magnitude.
- [ ] They are unrelated.
- [x] They are similar in direction.
- [ ] They are completely dissimilar.

> Cosine distance (or cosine similarity) measures the angle between two vectors in a high-dimensional space. A cosine distance of 0 (which corresponds to a cosine similarity of 1) means that the vectors are identical in direction, indicating strong semantic similarity between the two embeddings. This is crucial in vector search and retrieval systems, where similar meanings are identified based on direction rather than magnitude.


8. What must be done before you can delete a knowledge base in Generative AI Agents?
- [ ] Disconnect the database tool connection.
- [x] Delete the data sources and agents using that knowledge base.
- [ ] Reassign the knowledge base to a different agent.
- [ ] Archive the knowledge base for future use.

> You can only delete knowledge bases that aren't used by agents. Before you delete a knowledge base, you must delete the data sources in that knowledge base and delete the agents using that data source. The delete action permanently deletes the knowledge base. This action can't be undone.

9. Accuracy in vector databases contributes to the effectiveness of LLMs by preserving a specific type of relationship. What is the nature of these relationships, and why are they crucial for language models?
- [x] Semantic relationships, and they are crucial for understanding context and generating precise language
- [ ] Hierarchical relationships, and they are important for structuring database queries
- [ ] Linear relationships, and they simplify the modeling process
- [ ] Temporal relationships, and they are necessary for predicting future linguistic trends

> Vector databases store and retrieve information based on semantic relationships, meaning they capture meaning and context rather than just exact matches. This is crucial for LLMs because it allows them to retrieve the most relevant documents, ensuring context-aware and accurate responses in applications like chatbots, search engines, and retrieval-augmented generation (RAG) systems.

10. You are hosting a dedicated Al cluster using the OCI Generative AI service. You need to employ maximum number of endpoints due to high workload. \
How many dedicated Al clusters will you require to host at least 60 endpoints?
- [ ] 5
- [ ] 1
- [ ] 3
- [x] 2

> A hosting dedicated AI cluster can have up to 50 endpoints.

11. You want to build an LLM application that can connect application components easily and allow for component replacement in a declarative manner. \
What approach would you take?
- [x] Use LangChain Expression Language (LCEL).
- [ ] Use Python classes like LLMChain.
- [ ] Use prompts.
- [ ] Use agents.


12. What does accuracy measure in the context of fine-tuning results for a generative model?
- [ ] The number of predictions a model makes, regardless of whether they are correct or incorrect
- [ ] The proportion of incorrect predictions made by the model during an evaluation
- [ ] The depth of the neural network layers used in the model
- [x] How many predictions the model made correctly out of all the predictions in an evaluation

> Accuracy in the context of fine-tuning results for a generative model measures the proportion of correct predictions made by the model out of all predictions made during an evaluation. In other words, it quantifies the model's ability to generate outputs that match the desired or target outputs according to some evaluation metric or criteria. It represents the percentage of generated outputs that are considered accurate or correct based on the evaluation criteria used.


13. What is a key effect of deleting a data source used by an agent in Generative AI Agents?
- [ ] The agent starts generating responses based on pretrained data.
- [x] The agent no longer answers questions related to the deleted source.
- [ ] The agent automatically ingests data from a different source.
- [ ] The agent stops running completely.

> You can always delete data sources that are used by agents. While the agent continues to run, it no longer answers questions related to the sources that you deleted. The delete action permanently deletes the data source. This action can't be undone.

14. What advantage does fine-tuning offer in terms of improving model efficiency?
- [x] It reduces the number of tokens needed for model performance.
- [ ] It improves the model's understanding of human preferences.
- [ ] It eliminates the need for annotated data during training.
- [ ] It increases the model's context window size.

> Fine-tuning helps improve model efficiency by adapting a pre-trained model to a specific task or domain, allowing it to generate more relevant responses with fewer input tokens. This reduces computational costs and inference time while maintaining or improving accuracy. By refining the model's knowledge, fine-tuning enhances performance without requiring excessive amounts of new training data.

15. A researcher is exploring generative models for various tasks. While diffusion models have shown excellent results in generating high-quality images, they encounter significant challenges in adapting these models for text. \
What is the primary reason why diffusion models are difficult to apply to text generation tasks?
- [ ] Because diffusion models can only produce images
- [x] Because text representation is categorical, unlike images
- [ ] Because text is not categorical
- [ ] Because text generation does not require complex models

> Diffusion models are naturally suited for continuous data like images, where noise can be incrementally added and removed. However, text is categorical, meaning each token belongs to a discrete vocabulary, making it challenging to apply the same gradual noise-based transformations. Unlike images, where pixel values exist in a continuous space, text tokens do not have a smooth interpolation, making diffusion-based text generation more complex.

16. Which phase of the RAG pipeline includes loading, splitting, and embedding of documents?
- [ ] Generation
- [ ] Retrieval
- [x] Ingestion
- [ ] Evaluation

> In Retrieval-Augmented Generation (RAG), the ingestion phase involves loading documents, splitting them into smaller chunks, and embedding them into a vector database for efficient retrieval. This step is crucial because properly formatted and indexed data enables accurate and relevant retrieval during the generation phase. 


17. In which phase of the RAG pipeline are additional context and user query used by LLMs to respond to the user?
- [ ] Ingestion
- [ ] Retrieval
- [ ] Evaluation
- [x] Generation

> In the Retrieval-Augmented Generation (RAG) pipeline, the Generation phase is when the LLM uses both the user query and the retrieved additional context to produce a response. This is where the model synthesizes information and formulates an answer based on the retrieved knowledge.


18. You are developing an application that displays a house image along with its related details. Assume that you are using Oracle Database 23ai. \
Which data type should be used to store the embeddings of the images in a database column?
- [ ] INT
- [ ] Float32
- [x] VECTOR
- [ ] Double


19. When specifying a data source, what does enabling multi-modal parsing do?
- [x] Parses and includes information from charts and graphs in the documents
- [ ] Merges multiple data sources into a single knowledge base after parsing the files
- [ ] Automatically tags files and folders in the bucket
- [ ] Parses and converts non-supported file formats into supported ones


20. You are debugging and testing an OCI Generative AI chat model.
What is the model behavior if you don't provide a value for the seed parameter?
- [ ] The model generates responses deterministically.
- [ ] The model assigns a default seed value of 9999.
- [x] The model gives diverse responses.
- [ ] The model restricts the maximum number of tokens that can be generated

> If a seed value is provided, the model generates deterministic responses (same input leads to the same output). However, if no seed is specified, the model behaves non-deterministically, producing diverse responses each time it processes the same input.


21. How can you affect the probability distribution over the vocabulary of a Large Language Model (LLM)?
- [ ] By modifying the model's training data
- [ ] By adjusting the token size during the training phase
- [x] By using techniques like prompting and training
- [ ] By restricting the vocabulary used in the model


22. How is the _totalTrainingSteps_ parameter calculated during fine-tuning in OCI Generative AI?
- [ ] totalTrainingSteps = (size (trainingDataset) * trainingBatchSize) / totalTrainingEpochs
- [ ] totalTrainingSteps = (totalTrainingEpochs * trainingBatchSize) / size (trainingDataset)
- [x] totalTrainingSteps = (totalTrainingEpochs * size (trainingDataset)) / trainingBatchSize
- [ ] totalTrainingSteps = (totalTrainingEpochs + size (trainingDataset)) * trainingBatchSize


23. What is the destination port range that must be specified in the subnet's ingress rule for an Oracle Database in OCI Generative AI Agents?
- [ ] 8080-8081
- [ ] 3306-3307
- [ ] 1433-1434
- [x] 1521-1522

> Oracle Database typically uses port 1521 for SQL*Net (also known as Oracle Net) connections, which facilitate communication between clients and the database server. Some configurations may also use port 1522 for additional services or failover. When setting up ingress rules in an OCI subnet security list, allowing traffic over ports 1521-1522 ensures that Oracle Database can be accessed properly within the Generative AI Agents environment.

24. What happens to chat data and retrieved context after the session ends in OCI Generative AI Agents?
- [x] They are permanently deleted and not retained.
- [ ] They are stored for training the Large Language Models (LLMs).
- [ ] They are stored in isolation for future customer usage, ensuring maximum security but not used for training.
- [ ] They are archived for audit purposes.

> The OCI Generative AI Agents service retains customer-provided queries and retrieved context used for chatting with Large Language Models (LLMs) during the user's session. However, this data isn't stored beyond the session. Also, the service doesn't use customer chat data or knowledge base data for model training.


25. Which component of Retrieval-Augmented Generation (RAG) evaluates and prioritizes the information retrieved by the retrieval system?
- [ ] Encoder-decoder
- [ ] Retriever
- [ ] Generator
- [x] Ranker

> In Retrieval-Augmented Generation (RAG), the ranker evaluates and prioritizes the retrieved information to ensure that the most relevant and high-quality data is passed to the generator. It refines the initial retrieval results by scoring and reordering them based on relevance, improving the accuracy and contextual appropriateness of the generated response. This step is crucial for minimizing irrelevant or misleading outputs.


26. How many numerical values are generated for each input phrase when using the cohere.embed-english-light-v3.0 embedding model?
- [ ] 256
- [ ] 512
- [x] 384
- [ ] 1024


27. How does the temperature setting in a decoding algorithm influence the probability distribution over the vocabulary?
- [ ] Decreasing temperature broadens the distribution, making less likely words more probable.
- [ ] Increasing temperature removes the impact of the most likely word.
- [x] Increasing temperature flattens the distribution, allowing for more varied word choices.
- [ ] Temperature has no effect on the probability distribution; it only changes the speed of decoding.

> The temperature setting in a decoding algorithm scales the logits before applying the softmax function, which affects the probability distribution over the vocabulary. A higher temperature (e.g., >1) makes the distribution more uniform, increasing randomness and diversity in word choices. Conversely, a lower temperature (e.g., <1) sharpens the distribution, making the model favor the most probable words, leading to more deterministic outputs.


28. When is fine-tuning an appropriate method for customizing an LLM?
- [ ] When the LLM requires access to the latest data for generating outputs
- [ ] When you want to optimize the model without any instructions
- [ ] When the LLM already understands the topics necessary for text generation
- [x] When the LLM does not perform well on a particular task and the data required to adapt the LLM is too large for prompt engineering

> If the LLM's performance is suboptimal for a particular task, fine-tuning allows for the model to be further trained on task-specific data, enabling it to learn task-specific patterns and improve its performance. Fine-tuning is particularly suitable when prompt engineering is not feasible due to the size or complexity of the data required. In such cases, fine-tuning allows for direct adaptation of the model to the task without the need for extensive manual intervention.

29. A company is using a model in the OCI Generative AI service for text summarization. They receive a notification stating that the model has been deprecated. \
What action should the company take to ensure continuity in their application?
- [ ] The company can request an extension to continue using the model after it is retired.
- [x] The company can continue using the model but should start planning to migrate to another model before it is retired.
- [ ] The company should ignore the notification as deprecated models remain available indefinitely.
- [ ] The company must immediately stop using the model because it is no longer available and start using the newer model.


30. How does a presence penalty function when using OCI Generative AI chat models?
- [ ] It applies a penalty only if the token has appeared more than twice.
- [ ] It only penalizes tokens that have never appeared in the text before.
- [x] It penalizes a token each time it appears after the first occurrence.
- [ ] It penalizes all tokens equally, regardless of how often they have appeared.

> A presence penalty in language model generation functions by penalizing tokens each time they appear after their initial occurrence in the generated text. It serves the same purpose as Frequency penalty. Frequency penalty works on total number of occurrence vs step occurrence in Presence Penalty.


31. Which of these does NOT apply when preparing PDF files for OCI Generative AI Agents?
- [ ] Reference tables must be formatted with rows and columns.
- [x] Hyperlinks in PDFs are excluded from chat responses.
- [ ] PDF files can include images and charts.
- [ ] Charts must be two-dimensional with labeled axes.

> To prepare your data for Generative AI Agents data sources in OCI Generative AI Agents follow these guidelines: Data Sources: Data for Generative AI Agents must be uploaded as files to an Object Storage bucket. Number of Buckets: Only one bucket is allowed per data source. Supported File Types: Only PDF and txt files are supported. File Size Limit: Each file must be no larger than 100 MB. PDF Contents: PDF files can include images, charts, and reference tables but these must not exceed 8 MB. Chart Preparation: No special preparation is needed for charts, as long as they're two-dimensional with labeled axes. The model can answer questions about the charts without explicit explanations. Table Preparation: Use reference tables with several rows and columns. For example, the agent can read the table on the limits page. URLs: All the hyperlinks present in the PDF documents are extracted and displayed as hyperlinks in the chat response. Data Not Ready: If your data isn't yet available, create an empty folder for the data source and populate it later. This way, you can ingest data into the source after the folder is populated.

32. What happens to the status of an endpoint after initiating a move to a different compartment?
- [x] The status changes to Updating during the move and returns to Active after completion.
- [ ] The endpoint becomes Inactive permanently, and you need to create a new endpoint.
- [ ] The endpoint is deleted and recreated in the new compartment.
- [ ] The status remains Active throughout the move.

> A notification indicates that the endpoint resource is moved to the new compartment successfully. You might notice that the endpoint status changes to Updating. After the move is successful, the endpoint status changes back to Active.


33. A data scientist is training a machine learning model to predict customer purchase behavior. After each training epoch, they analyze the loss metric reported by the model to evaluate its performance. They notice that the loss value is decreasing steadily over time. \
What does the loss metric indicate about the model's predictions in this scenario?
- [ ] Loss reflects the quality of predictions and should increase as the model improves.
- [x] Loss quantifies how far the model's predictions deviate from the actual values, indicating how wrong the predictions are.
- [ ] Loss measures the total number of predictions made by the model during training.
- [ ] Loss only evaluates the accuracy of correct predictions, ignoring the impact of incorrect predictions.

> Loss, in the context of machine learning, is a measure of how incorrect or "wrong" the model's predictions are compared to the true or target values. It quantifies the discrepancy between the predicted outputs and the actual ground truth.


34. Which of these is NOT a supported knowledge base data type for OCI Generative AI Agents?
- [ ] Oracle Database 23ai vector search
- [x] Custom-built file systems
- [ ] OCI Object Storage files with text and PDFs
- [ ] OCI Search with OpenSearch

> Knowledge Base Data Types: 1) Service-Managed Option - OCI Object Storage files 2) Bring Your Own (BYO) Options - Oracle Database 23ai vector search & OCI Search with OpenSearch

35. A company is using a Generative AI model to assist customer support agents by answering product-related queries. \
Customer query: "What are the supported features of your new smart watch?"  \
Generative AI model response: "The smart watch includes ECG monitoring, blood sugar tracking, and solar charging." \
Upon review of this response, the company notes that blood sugar tracking and solar charging are not actual features of their smart watch. \
These details were not part of the company's product documentation or database. \
What is the most likely cause of this model behavior?
- [ ] The model is overfitting to specific details from unrelated training data, causing inaccuracies.
- [ ] The model encountered a prompt that was too ambiguous, leading to random outputs.
- [ ] The model was unable to access the company's database, so it defaulted to guessing feature sets based on similar products.
- [x] The model is hallucinating, confidently generating responses that are not grounded in factual or provided data.

> Hallucination occurs when the model generates content that is plausible-sounding but factually incorrect or fabricated. In this case, the model invented product features that were not in the company s documentation.


36. In which scenario is soft prompting more appropriate compared to other training styles?
- [ ] When there is a significant amount of labeled, task-specific data available
- [ ] When the model needs to be adapted to perform well in a domain it was not originally trained on
- [ ] When the model requires continued pretraining on unlabeled data
- [x] When there is a need to add learnable parameters to a LLM without task-specific training

> Soft prompting involves learning a small set of continuous embeddings that guide the model's behavior without modifying its original parameters. Unlike traditional fine-tuning, soft prompts require no task-specific training of the full model and are efficient in adapting LLMs to different tasks with minimal computational overhead. This makes it ideal for scenarios where full fine-tuning is impractical but some level of customization is needed.


37. Which statement regarding fine-tuning and Parameter-Efficient Fine-Tuning (PEFT) is correct?
- [ ] PEFT requires replacing the entire model architecture with a new one designed specifically for the new task, making it significantly more data-intensive than fine-tuning.
- [ ] Both fine-tuning and PEFT require the model to be trained from scratch on new data, making them equally data and computationally intensive.
- [x] Fine-tuning requires training the entire model on new data, often leading to substantial computational costs, whereas PEFT involves updating only a small subset of parameters, minimizing computational requirements and data needs.
- [ ] Fine-tuning and PEFT do not involve model modification; they differ only in the type of data used for training, with fine-tuning requiring labeled data and PEFT utilizing unlabeled data.

> Fine-tuning involves adjusting all model parameters, which can be computationally expensive and require large amounts of data. Parameter-Efficient Fine-Tuning (PEFT), on the other hand, updates only a small subset of parameters (e.g., LoRA, adapters) while keeping the majority of the pre-trained model unchanged. This approach significantly reduces computational cost and memory requirements while achieving strong performance on specialized tasks.


38. A data scientist is exploring Retrieval-Augmented Generation (RAG) for a natural language processing project. \
Which statement is true about RAG?
- [x] It is non-parametric and can theoretically answer questions about any corpus.
- [ ] It is primarily parametric and requires a different model for each corpus.
- [ ] It is not suitable for fact-checking because of high hallucination occurrences.
- [ ] It is solely used in QA-based scenarios.

> Retrieval-Augmented Generation (RAG) is a non-parametric approach because it retrieves relevant information from external data sources at inference time rather than relying solely on pre-trained parameters. This allows RAG to dynamically answer questions based on any corpus without requiring a separate fine-tuned model for each dataset.

39. In the context of generating text with a Large Language Model (LLM), what does the process of greedy decoding entail?
- [ ] Using a weighted random selection based on a modulated distribution
- [ ] Picking a word based on its position in a sentence structure
- [ ] Selecting a random word from the entire vocabulary at each step
- [x] Choosing the word with the highest probability at each step of decoding

> Greedy decoding is a simple decoding strategy where, at each step, the model selects the word with the highest probability. While this approach ensures deterministic outputs, it may lead to suboptimal results because it doesn't consider future word choices, often resulting in repetitive or less coherent text. 


40. What is the role of the inputs parameter in the given code snippet? <br />
_inputs = [ \
"Learn about the Employee Stock Purchase Plan", \
"Reassign timecard approvals during leave", \
"View my payslip online",\
]\
embed_text_detail.inputs = inputs_
- [ ] It sets the output format for the embeddings.
- [ ] It controls the maximum number of embeddings the model can generate.
- [x] It specifies the text data that will be converted into embeddings.
- [ ] It provides metadata about the embedding process.

> The inputs parameter is used to pass a list of text strings to the Generative AI model for embedding generation.


41. In an OCl Generative AI chat model, which of these parameter settings is most likely to induce hallucinations and factually incorrect information?
- [ ] temperature = 0.0, top_p = 0.7, and frequency_penalty = 1.0
- [x] temperature = 0.9, top_p = 0.8, and frequency_penalty = 0.1
- [ ] temperature = 0.5, top_p = 0.9, and frequency_penalty = 0.5
- [ ] temperature = 0.2, top_p = 0.6, and frequency_penalty = 0.8

> High Temperature (e.g., temperature = 0.9): A high temperature introduces randomness and creativity in the model's token selection, increasing the likelihood of hallucinations and generating factually incorrect information. Moderate top_p (e.g., top_p = 0.8): Lowering top_p constrains the model to focus on high-probability tokens but still allows some randomness when combined with high temperature. Low frequency_penalty (e.g., frequency_penalty = 0.1): A low frequency penalty allows the model to reuse tokens, which can exacerbate hallucination tendencies. A temperature of 0.0 results in deterministic outputs, which significantly reduces hallucination risks. A moderate temperature balances creativity and determinism, reducing the risk of hallucinations. A low temperature and constrained top_p create outputs that are factually grounded and less likely to hallucinate.


42. A startup is using Oracle Generative AI's on-demand inferencing for a chatbot. The chatbot processes user queries and generates responses dynamically. \
One user enters a 200-character prompt, and the model generates a 500-character response.\
How many transactions will be billed for this inference call?
- [ ] 500 transactions
- [ ] 1 transaction per API call, regardless of length
- [ ] 200 transactions
- [x] 700 transactions

> For on-demand inferencing, the total number of billable characters is the sum of the prompt and response length.


43. Which statement is true about the "Top p" parameter of OCI Generative AI chat models?
- [x] "Top p" limits token selection based on the sum of their probabilities.
- [ ] "Top p" selects tokens from the "top k" tokens sorted by probability.
- [ ] "Top p" assigns penalties to frequently occurring tokens.
- [ ] "Top p" determines the maximum number of tokens per response.

> Instead of selecting from a fixed k number of tokens, "Top p" dynamically selects tokens whose cumulative probability reaches a threshold.


44. What is the purpose of the VECTOR field in the Oracle Database 23ai table for Generative AI Agents?
- [x] To store the embeddings generated from the BODY content
- [ ] To assign a unique identifier DOCID to each document
- [ ] To store the URL references for the documents
- [ ] To store the document TITLE

> Required Fields for creating Oracle Database 23ai table with the following fields: DOCID: An id assigned to each record or document BODY: The actual content that you want the agent to search VECTOR: The vector generated from an embedding model based on the body content

45. A machine learning engineer is exploring T-Few fine-tuning to efficiently adapt a Large Language Model (LLM) for a specialized NLP task. They want to understand how T-Few fine-tuning modifies the model compared to standard fine-tuning techniques. \
Which of these best describes the characteristic of T-Few fine-tuning for LLMs?
- [ ] It does not update any weights but restructures the model architecture.
- [x] It selectively updates only a fraction of the model's weights.
- [ ] It updates all the weights of the model uniformly.
- [ ] It increases the training time as compared to Vanilla fine-tuning.

> T-Few fine-tuning, also known as Task-Focused Fine-Tuning, is a technique used with Large Language Models (LLMs) to adapt them to specific tasks or domains more efficiently. The characteristic of T-Few fine-tuning is that it selectively updates only a fraction of the model's weights rather than updating all weights uniformly. This selective updating process involves identifying and updating the parameters of the LLM that are most relevant to the target task or domain, while keeping most of the weights fixed. This also reduces the computational cost and time required for adaptation.


46. In the context of RAG, how might the concept of Groundedness differ from that of Answer Relevance?
- [ ] Groundedness focuses on data integrity, while Answer Relevance emphasizes lexical diversity.
- [ ] Groundedness measures relevance to the user query, while Answer Relevance evaluates data integrity.
- [x] Groundedness pertains to factual correctness, while Answer Relevance concerns query relevance.
- [ ] Groundedness refers to contextual alignment, while Answer Relevance deals with syntactic accuracy.

> In Retrieval-Augmented Generation (RAG), Groundedness ensures that the model s response is factually correct and traceable to retrieved sources, minimizing hallucinations. Answer Relevance, on the other hand, evaluates how well the response aligns with the user s query, ensuring that the retrieved and generated content is contextually appropriate rather than just factually correct. Both are essential for high-quality AI-generated responses.

47. A data science team is fine-tuning multiple models using the Oracle Generative AI service. They select the _cohere.command-r-08-2024_ base model and fine-tune it on three different datasets for three separate tasks. They plan to use the same fine-tuning Al cluster for all models. \
What is the total number of units provisioned for the cluster?
- [ ] 2
- [ ] 1
- [x] 8
- [ ] 6

> For fine-tuning clusters, the cohere.command-r-08-2024 base model automatically provisions 8 units, regardless of the number of models fine-tuned on the cluster. Multiple models can be fine-tuned using the same cluster without increasing the unit count.


48. When does a chain typically interact with memory in a run within the LangChain framework?
- [x] After user input but before chain execution, and again after core logic but before output
- [ ] Continuously throughout the entire chain execution process
- [ ] Only after the output has been generated
- [ ] Before user input and after chain execution

> In the LangChain framework, a chain typically interacts with memory at two specific points during a run. The first interaction occurs after user input but before chain execution begins. At this stage, the chain may access and retrieve relevant information or context stored in memory to inform its processing or decision-making process. The second interaction with memory occurs after the core logic of the chain has been executed but before generating the final output. At this stage, the chain may update or modify the memory based on the results of its processing, storing any relevant information or intermediate results for future reference or use.


49. What happens when this line of code is executed? \
`embed_text_response = generative_ai_inference_client.embed_text(embed_text_detail)`
- [x] It sends a request to the OCI Generative AI service to generate an embedding for the input text.
- [ ] It processes and configures the OCl profile settings for the inference session.
- [ ] It initiates a connection to OCI and authenticates using the user's credentials.
- [ ] it initializes a pretrained OCI Generative AI model for use in the session.


50. What does the OCI Generative AI service offer to users?
- [ ] A limited platform that supports chat-based LLMs without hosting capabilities
- [x] Fully managed LLMs along with the ability to create custom fine-tuned models
- [ ] A service requiring users to share GPUs for deploying LLMs
- [ ] Only pretrained LLMs with customization options

> Generative AI is a fully managed Oracle Cloud Infrastructure service that provides a set of state-of-the-art, customizable large language models (LLMs) that cover a wide range of use cases, including chat, text generation, summarization, and creating text embeddings. You can also use the playground to try out the ready-to-use pretrained models or create and host your own fine-tuned custom models based on your own data on dedicated AI clusters.


<br />

___
