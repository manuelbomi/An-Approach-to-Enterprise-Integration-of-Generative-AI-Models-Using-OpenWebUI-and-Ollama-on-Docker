# An Approach to Enterprise Integration of Generative-AI Models Using OpenWebUI and Ollama on Docker

Some of the cost associated with using generative AI models in the enterprise settings include: 

1. Data Acquisition and Processing: 
High-quality data is essential for training effective AI models, and acquiring, cleaning, and labeling this data, especially for specialized industries, can be time-consuming and costly.
Data restrictions in certain sectors like healthcare or finance can further increase costs. 
2. Hardware Requirements: If models are acquired to be used on-prem, and if methods of models performance improvement such as exposing the model to enterprise dataset through Retrieval Augmentation Generation (RAG) are used, then the cost of the hardware needed must be considered.  AI needs specialized, expensive hardware like GPUs, which can cost tens of thousands of dollars per unit, and multiple units are often required.
3. Labor Costs: Skilled AI professionals command high salaries, and the limited supply of such talent drives up wages.
4. Integration and Testing: Reliably integrating Gen AI models into existing workflows and testing/optimizing systems is complex and resource-intensive, potentially taking months and adding costs.
5. Operating Costs: If models are acquired and intgerated with cloud-based or on-prem workflows, the operational expenses must be considered. AI systems require significant computing power, leading to high ongoing operational expenses, potentially hundreds of thousands of dollars monthly for server and energy costs.
6. Using Remote Vendor based APIs: If the enterprise approaches using Gen AI models by the bulk purchase of access tokens and the use of vendor based APIs such as using OpenAI's ChatGPT, then the cost of the access tokens may scale up exponetially with the daily usage of different APIs or models across the enterprise. Some

---
![Image](https://github.com/user-attachments/assets/afad8906-5c29-4945-863f-a0fab73a9a6a)

_Source: https://tomtunguz.com/gm-saas/?utm_source=tldrai_
---

7. Model Selection and Licensing: Costs vary based on the model approach, with commercial APIs having usage-based fees and open-source models having lower licensing but higher deployment costs.
8. Vendor Lock-in: Heavy investment in one vendor's models can lead to lock-in, making switching difficult and potentially resulting in higher costs if the vendor increases prices.
   

---
> 
## Cost Effective Consideration for Enterprise Generative AI Models' Integration 
For enterprise integration, based on enterprise applications or needs, to reduce Gen AI models usage cost we suggest: 
(i) The use of models with minimal intgeration footprints such as using models with minimal memory or GPU requirements. 
(ii) For common, non-specialized applications, We suggest using verified open-source models with very low or near-zero enterprise licensing fees
(iii) For effective securance of enterprise data, we suggest the use of verified and highly secured method of integration if on-prem integration is considered. The same consideration can be given to  

---



---
![Image](https://github.com/user-attachments/assets/afad8906-5c29-4945-863f-a0fab73a9a6a)

_Source: https://tomtunguz.com/gm-saas/?utm_source=tldrai_
---



### **OVERVIEW**
Reliably architecting databases is very crucial for designing efficient data analytics systems. After selecting the software and  

> [!NOTE]
> Ollama supports several state of the art Gen AI models. Interested readers can check the entire repertoire at the Ollama model homepage _(https://ollama.com/search)_.
Some eamples are shown in the two figures below:

---
![Image](https://github.com/user-attachments/assets/893d66fb-0078-4b99-8295-08958a4030b3)

---

![Image](https://github.com/user-attachments/assets/7b7436e9-6a57-4432-8713-12a77288ba23)

---

### **Benefits of Using Lucidchart for Entity Relationship Diagrams**
For very complex systems, due to system 

In addition, Lucidchart 

---

> [!IMPORTANT]
After using Lucidchart to 
>

---
In this discourse, we will show (using infographs) how to use Lucidchart to architect an e-commerce database comprising of four tables viz: customers, products, orders and order_details tables.

We shall then show how to use Lucidchart to translate the e-commerce ERD to a database by using Lucidchart to automatically generate SQL codes for MSSQL Server database. 

---
> [!IMPORTANT]
Here, we have shown the steps needed to efficiently architect an e-commerce database for MSSQL Server database.
>
---

Navigate to Ollama homepage: 
---
![Image](https://github.com/user-attachments/assets/861f3af3-e7a9-4c2a-add3-f8ff36dd09fe)

---
Select installation method for your target OS. 
---
For Linux, use:
---

```ruby
curl -fsSL https://ollama.com/install.sh | sh
```
to install Ollama from the command line
---
![Image](https://github.com/user-attachments/assets/54374cf7-3e6d-4a3b-951c-40f9f5b6113a)

---

![Image](https://github.com/user-attachments/assets/f572f483-9536-4506-ab48-9b0a6ee67593)
![Image](https://github.com/user-attachments/assets/5993eece-7179-4e55-b214-67a5c5d8d310)
![Image](https://github.com/user-attachments/assets/9b99ba31-71cf-41b0-a106-de30b07bea5c)
![Image](https://github.com/user-attachments/assets/670a53f6-e467-40ef-8263-200ce8191121)
![Image](https://github.com/user-attachments/assets/b8f839f9-0fdd-4695-b356-a76eeb1aba84)
![Image](https://github.com/user-attachments/assets/2fe77a36-828f-4d9f-bcc0-6a1fa46b3b61)
![Image](https://github.com/user-attachments/assets/90057750-bc84-4b93-975d-253acfee307c)
![Image](https://github.com/user-attachments/assets/a5648c09-cf19-48d8-b01b-9a6f37825816)
![Image](https://github.com/user-attachments/assets/72b96526-048d-42a1-b15a-fc797548ef3b)
![Image](https://github.com/user-attachments/assets/ad7024ef-5627-48ce-b410-382220bac79c)
![Image](https://github.com/user-attachments/assets/4c76ceea-965a-4644-a3c0-be881e813088)
![Image](https://github.com/user-attachments/assets/1dc6655b-f8b9-4efe-9f45-e54f773452cf)
![Image](https://github.com/user-attachments/assets/abc7526f-73cc-415a-89d7-9b040f58d950)
![Image](https://github.com/user-attachments/assets/7b3d6198-2901-4a88-afb0-e13eb9b5fa62)
![Image](https://github.com/user-attachments/assets/66c60695-5610-4bef-9241-a71396248793)
![Image](https://github.com/user-attachments/assets/c21c9e3d-d558-4f76-b154-b87581829a58)
![Image](https://github.com/user-attachments/assets/e268fba1-ca7c-4215-84bb-043752206171)
![Image](https://github.com/user-attachments/assets/cd020526-aeb7-4773-8e2d-60b2927d831d)








> [!TIP]
> Here, we have shown the e-commerce use case SQL code generated by Lucidchart for MSSQL Server database.
 

> MSSQL Server database Implementation

```ruby
'CREATE TABLE [customers] (
  [customer_id] INT ,
  [last_name] VARCHAR(255),
  [first_name] VARCHAR(255),
  [phone_nos] VARCHAR(20),
  [email] VARCHAR(255),
  [street] VARCHAR(255),
  [city] VARCHAR(255),
  [zip] VARCHAR(255),
  [is_active] BOOLEAN,
  PRIMARY KEY ([customer_id])
);

CREATE TABLE [product] (
  [product_id] INT,
  [product_name] VARCHAR(255),
  [price] DECIMAL,
  PRIMARY KEY ([product_id])
);

CREATE TABLE [orders] (
  [id] INT,
  [customer_id] INT,
  [date] DATE,
  PRIMARY KEY ([id]),
  CONSTRAINT [FK_orders.customer_id]
    FOREIGN KEY ([customer_id])
      REFERENCES [customers]([customer_id])
);

CREATE TABLE [order_details] (
  [id] INT,
  [order_id] INT,
  [product_id] INT,
  [quantity] INT,
  [price] DECIMAL(12, 2),
  [to_street] VARCHAR(255),
  [to_city] VARCHAR(255),
  [to_zip] VARCHAR(255),
  [ship_date] varchar,
  PRIMARY KEY ([id]),
  CONSTRAINT [FK_order_details.product_id]
    FOREIGN KEY ([product_id])
      REFERENCES [product]([product_id]),
  CONSTRAINT [FK_order_details.order_id]
    FOREIGN KEY ([order_id])
      REFERENCES [orders]([id])
);


```

---
Step 9: Log onto your MSSQL Server database
---
![Image](https://github.com/user-attachments/assets/254ee87b-15d3-4e2e-afa3-1dbce2b1375a)
---
Step 10: Create a new named database.






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



