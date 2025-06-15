# **An Approach to Enterprise Integration of Generative-AI Models Using OpenWebUI and Ollama on Docker**

In enterprise settings, costs associated with using generative AI (GenAI) models can scale up with the number of people and processes that are using the models across the enterprise. Some of the cost associated with using GenAI models in enterprise settings include: 

### Data Acquisition and Processing Costs: 
High-quality data is essential as inputs to the model if methods of model's performance improvement (such as exposing the model to enterprise dataset through Retrieval Augmentation Generation (RAG)) are considered. 

Cost of obtaining high quality data could be prohibitive. Data restrictions in certain sectors like healthcare, non-civil technologies and finance can further increase costs. 
### Hardware Requirements: 
If models are acquired to be used on-prem, and if methods of model's performance improvement methods (such as exposing the model to enterprise dataset through RAG) are used, then, the cost of the hardware needed must be considered.

Most enterprise AI applications often needs specialized, expensive hardware like GPUs, which can cost tens of thousands of dollars per unit, and multiple units are often required for enterprise-scale deployments.
### Labor Costs: 
Skilled AI professionals command high salaries, and the limited supply of such talent drives up wages.
### Integration and Testing: 
Reliably integrating GenAI models into existing workflows and testing/optimizing systems could be complex and resource-intensive, potentially taking months and adding costs.
### Operating Costs: 
If models are acquired and intgerated with cloud-based or on-prem workflows, then, operational expenses must be considered. AI systems require significant computing power, leading to high ongoing operational expenses.
### Using Remote Vendor based APIs: 
If the enterprise approaches using GenAI models via the bulk purchase of access tokens; and the use of vendor based APIs such as remotely accessing OpenAI's ChatGPT, then the cost of the access tokens may scale up exponetially with daily usage of different APIs or models across the enterprise. An idea of the GenAI models' usage cost implication (in USD) is given on the graph below.

---
![Image](https://github.com/user-attachments/assets/afad8906-5c29-4945-863f-a0fab73a9a6a)

_Source: https://tomtunguz.com/gm-saas/?utm_source=tldrai_
---

### Model Selection and Licensing: 
Costs may vary based on the model selection approach; with commercial APIs having usage-based fees and open-source models having lower licensing but may have higher deployment costs.
### Vendor Lock-in: 
Heavy investment in a particular vendor's models can lead to being locked-in, making switching vendor/model difficult and potentially resulting in higher costs if the vendor increases price.
   

---
> 
## Cost Effective Consideration for Enterprise Generative AI Models' Integration 
### To reduce cost of GenAI model integration and to promote wider GenAI adoption and models' diversity in enterprise settings, we suggest: 
##### (i)    The use of models with minimal intgeration footprints such as using models with minimal memory or GPU requirements. 
##### (ii)   For common, non-specialized applications, We suggest using verified open-source models with very low or near-zero enterprise licensing fees.
##### (iii)  For effective securance of enterprise data and GenAI workflow, we suggest the use of well-known and proven GenAI models for on-prem deployments. The same consideration can be given to  cloud-based deployments and integration.
##### (iv) To prevent vendor lock-in and to reduce enterprise integration cost, we argue that it is better to consider enterprise adoption of diverse open-source models from different vendors. If enterprise model usage must necessarily entail the payment of licensing fees, then the enterprise should consider only robust, tested, highly reliable, and possibly multi-functional models that have lower licensing fees. 

---
> [!IMPORTANT]
> ### In this discourse, we have showm a method by which some GenAI models (such as: llama3.2, deepseek-r1 and gemma3 etc) can be installed <ins>on-prem</ins> using Docker. The same approach could be adopted for <ins>cloud-based</ins> workflow deployments such as when using Linux on an EC2 instance on AWS.
> ### In our approach, the user may use the docker-installed GenAI models online or offline without the Internet.
> ### Also, users or the enterprise do not need to pay token or API access charges since the method shown here does not use remote vendor-based API access points such as using OpenAIs ChatGPT UI.
> ### In our example shown here, Ollama models' suite UI is used along with Docker to illustrate our method.  OpenWebUI is used to provide a user-friendly UI for the installed GenAI models.
> ### In our approach here, widely known models with low memory footprint and low GPU (or none-GPU) usage are considered.
> ### We show how the installed models performed with generic queries and coding tasks. Outputs of the models under basic querying could be obtained as attachments from this repository.
> ### Outputs of the models' coding tasks can also be obtained from some of the inforgraphs below.
> ### We did not advocate for the usage of one model over the other in this discourse since usage requirements and/or needs could vary with different enterprise settings or requirements.
---
> [!CAUTION]
> ### Before any model or workflow is deployed in an enterprise setting, it is mandatory that the model or workflow should be thoroughly vetted by enterprise security personnel and tools.
> ### It is often better to initially deploy a model or workflow in an enterprise sandbox in order to observe its behaviour vis-à-vis any security flaw(s).
> ### The enterprise $${\color{red}Red \space Team}$$ should thoroughly test the model or workflow for any cybersecurity flaw before final deployment.
> ### Only GenAI models that have been thoroughly vetted security-wise should be whitelisted and deployed in an enterprise setting.
---

Step 1: Navigate to Ollama homepage: 
---
Ollama is a tool that allows users to run large language models (LLMs) directly on their local machine, without relying on cloud services. This makes it useful for developers, researchers, and businesses who want to maintain control over data and privacy, reduce cost, improve performance by deploying different models, and to customize experiments along with model deployments)

![Image](https://github.com/user-attachments/assets/861f3af3-e7a9-4c2a-add3-f8ff36dd09fe)

On Ollama's model page, users can obtain details regarding currently available and Ollama-supported GenAI models. Some examples are shown on the figures below. More are available on Ollama's homepage (https://ollama.com/).

Step 2: Check available models on Ollama homepage
---
![Image](https://github.com/user-attachments/assets/893d66fb-0078-4b99-8295-08958a4030b3)
---

![Image](https://github.com/user-attachments/assets/7b7436e9-6a57-4432-8713-12a77288ba23)

---
Step 3: On Ollama's homepage, select the installation method for your target OS. 
---

For Linux, use the command:


```ruby
curl -fsSL https://ollama.com/install.sh | sh
```

to install Ollama from the command line. Example is shown below

![Image](https://github.com/user-attachments/assets/54374cf7-3e6d-4a3b-951c-40f9f5b6113a)

---
Note that Ollama can work with the target device's CPU if GPU is not detected on the device
---

![Image](https://github.com/user-attachments/assets/f572f483-9536-4506-ab48-9b0a6ee67593)
---
Step 4: Use the installed ollama to download and install your desired model. For example, to install llama3.2, use the command:
---
```ruby
ollama run llama3.2:latest
```
---
![Image](https://github.com/user-attachments/assets/5993eece-7179-4e55-b214-67a5c5d8d310)
---
Step 5: Test-run the installed llama3.2 model
---

The query used to test the installed llama3.2 model is: "What are some interesting facts about the Benin empire?"

![Image](https://github.com/user-attachments/assets/9b99ba31-71cf-41b0-a106-de30b07bea5c)
---
Step 6: Install other model, e.g deepseek. To install deepseek, use the code:
---
```ruby
ollama run deepseek-r1:latest
```
---
Test-run the installed deepseek model
---
You can decide to use the same query as the one used to test the llama3.2 model: "What are some intersting facts about the Benin empire?"

![Image](https://github.com/user-attachments/assets/b8f839f9-0fdd-4695-b356-a76eeb1aba84)
---
![Image](https://github.com/user-attachments/assets/2fe77a36-828f-4d9f-bcc0-6a1fa46b3b61)
---
![Image](https://github.com/user-attachments/assets/90057750-bc84-4b93-975d-253acfee307c)
---
Step 7: Install another model if you wish. To install gemma3. Use the code: 
---
```ruby
ollama run gemma3:latest
```
---
![Image](https://github.com/user-attachments/assets/a5648c09-cf19-48d8-b01b-9a6f37825816)
---
Test-run the installed model
---
![Image](https://github.com/user-attachments/assets/72b96526-048d-42a1-b15a-fc797548ef3b)

Responses of each installed model to the query: "What are some interesting facts about the Benin Kingdom" can be found as attachments on this Github repository. Interested reader can notice that each model responses are quite different. Some model ask follow-up questions, which makes them fully conversational. Some other model's response are very brief while some other ones are quite extensive. 

---
To see a list of all available models on Ollama, use:
---
```ruby
ollama list
```
---
![Image](https://github.com/user-attachments/assets/ad7024ef-5627-48ce-b410-382220bac79c)
---
Step 8: Install OpenWebUI on Docker
---
OpenWebUI is an extensible, feature-rich, and user-friendly self-hosted AI platform designed to operate entirely offline. It supports various LLM runners like Ollama and OpenAI-compatible APIs, with built-in inference engine for RAG, making it a powerful AI deployment solution

---
Navigate to the OpenWebUI Github page and copy the code that can be used to install OpenWebUI on Docker. Ensure that Docker is already runing on your Linux system. 
---
![Image](https://github.com/user-attachments/assets/4c76ceea-965a-4644-a3c0-be881e813088)
---
Step 9: Read the instructions and install OpenWebUI on your Linux Docker. For Windows and Mac OS, the instructions for installation are also available on OpenWebUI Github page. 
---
![Image](https://github.com/user-attachments/assets/1dc6655b-f8b9-4efe-9f45-e54f773452cf)
---
Use
```ruby
docker ps -a
```

to see the list of all containers available on your Docker

---

![Image](https://github.com/user-attachments/assets/abc7526f-73cc-415a-89d7-9b040f58d950)
---
Step 10: Navigate to the page at which OpenWebUI is runing on your device. Configure the Admin details and login to OpenWebUI
---
![Image](https://github.com/user-attachments/assets/7b3d6198-2901-4a88-afb0-e13eb9b5fa62)
---
Use gemma3 to write some (Python) code. It can write codes in other langages as well. 
---

Code Query: Write a Python program that will list all the numbers that are a multiple of 5 and 7 in the range 700 to 2100

---
![Image](https://github.com/user-attachments/assets/66c60695-5610-4bef-9241-a71396248793)
---
![Image](https://github.com/user-attachments/assets/c21c9e3d-d558-4f76-b154-b87581829a58)
---
Users can decide to compare the codes generated by two different models using OpenWebUI. For example, the code outputs of both gemma3 and llama3.2 could be compared. 
---
![Image](https://github.com/user-attachments/assets/e268fba1-ca7c-4215-84bb-043752206171)
---

OpenWebUI also support multimodal inputs. Users can decide to use their device microphone to dictate the query
![Image](https://github.com/user-attachments/assets/4e8c5cd6-5907-4876-ae2c-ddd194658e1b)
---











### **AUTHOR'S BACKGROUND**

```

Author's Name:  Emmanuel Oyekanlu
Skillset:   I have experience spanning several years in developing scalable enterprise data pipelines, architecting enterprise data, software and AI solutions,
data engineering, high performance computing (GPU, CUDA), machine learning, NLP and LLM applications as well as deploying scalable solutions (apps) on-prem and in the cloud.
I can be reached through: manuelbomi@yahoo.com
Website:  http://emmanueloyekanlu.com/
Publications:  https://scholar.google.com/citations?user=S-jTMfkAAAAJ&hl=en
LinkedIn:  https://www.linkedin.com/in/emmanuel-oyekanlu-6ba98616
Github:  https://github.com/manuelbomi

```
[![Icons](https://skillicons.dev/icons?i=aws,azure,gcp,scala,mongodb,redis,cassandra,kafka,anaconda,matlab,nodejs,django,py,c,anaconda,git,github,mysql,docker,kubernetes&theme=dark)](https://skillicons.dev)



