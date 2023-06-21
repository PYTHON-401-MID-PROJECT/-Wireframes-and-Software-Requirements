# Wireframes-and-Software-Requirements
# Wireframes
the wireframe is simply will be the whatsapp chat which will look like this:


![](./assests/Wireframe.png)

# User Stories
### Title : Story one

- User Story sentence:
As a user, I want to reach the instructions for renewal my Passport so that I can quickly navigate to my account and do it .
- Feature Tasks : to scrape the Civil affairs at https://eservices.cspd.gov.jo/index-rtl.html
- Acceptance Tests : to return the correct information

### Title : Story two

- User Story sentence:
As a user, I want to reach the instructions for Renewal of Driver's License so that I can quickly navigate to my account and do it .
- Feature Tasks : to scrape this web site (https://www.ammancity.gov.jo/ar/eservices/login.aspx)
- Acceptance Tests : to return the correct information

### Title : Story Three

- User Story sentence:
As a user, I want to reach the E-Services that Civil Status and passports Department provided using voice Record so that I can quickly have the reponse.
- Feature Tasks : to reach the bot on the whatssaap platform 
- Acceptance Tests : to return the correct instructions

### Title : Story Four

- User Story sentence:
As a user, I want to reach the instructions to create a new Id  using voice Record so I can prepare them before  .
- Feature Tasks : send a voice note to the whatsaap, the function will convert the voive to text and do what the user wants 
- Acceptance Tests :  to return the correct instructions

### Title : Story Five

- User Story sentence:
As a user, I want to ..... using voice Record .
- Feature Tasks : send a voice note to the whatsaap, the function will convert the voive to text and do what the user wants 
- Acceptance Tests :  to return the correct instructions

### Estimate your User Stories

- extra small : 0-2 hours
- extra large : day or two

| story #       | estimation time |
|:-------------:|:---------------:|
|1|extra large|
|2|extra large|
|3|extra large|
|4|extra large|
|5|extra small|

# Software Requirements
### Vision
What is the vision of this product?


The vision of JoEasyGov is to revolutionize the way people interact with government transactions in Jordan by leveraging AI technology. The product aims to streamline and simplify the often complex and time-consuming process of dealing with governmental procedures. By providing a user-friendly and efficient platform, JoEasyGov envisions enhancing citizen experience, reducing bureaucracy, and promoting efficiency in government services. Ultimately, the goal is to empower individuals by offering accessible and personalized assistance, making government transactions more convenient and hassle-free.


What pain point does this project solve?


This project addresses the pain points associated with complex government procedures, lack of information, limited accessibility, and time-consuming processes in Jordan. JoEasyGov streamlines government transactions, simplifying the steps and providing clear guidance to users, thereby reducing confusion and frustration. It serves as a reliable source of accurate and up-to-date information, ensuring individuals have the necessary knowledge to make informed decisions. Additionally, JoEasyGov's 24/7 availability and electronic document submission feature eliminate the constraints of fixed working hours and physical visits, saving users time and effort.


Why should we care about your product?


You should care about JoEasyGov because it addresses the challenges and complexities individuals face when dealing with government transactions in Jordan. By streamlining processes, providing accessible information, and offering a user-friendly interface, JoEasyGov simplifies the entire experience. It saves time, reduces bureaucracy, and promotes efficiency, ultimately enhancing citizen satisfaction. With its 24/7 availability and round-the-clock access, JoEasyGov offers convenience to individuals, making government services more accessible to all.





# Domain Modeling

### Entities:

1. PdfReader: Represents a PDF reader object.
2. RecursiveCharacterTextSplitter: Represents a text splitter object that divides the text into chunks.
3. VectorStore: Represents a vector store for embeddings.
4. OpenAIEmbeddings: Represents embeddings generated using OpenAI.
5. FAISS: Represents a vector store implementation using FAISS.
6. llm: Represents an instance of the OpenAI language model.
7. Chain: Represents a question-answering chain.

### Relationships:

- PdfReader is associated with the uploaded PDF file.
- RecursiveCharacterTextSplitter splits the text extracted from the PDF into chunks.
- VectorStore is created from the chunks of text.
- OpenAIEmbeddings generates embeddings for the chunks of text.
- FAISS utilizes the embeddings to create the VectorStore.
- llm is an instance of the OpenAI language model used for question-answering.
- Chain is created using the llm instance for question-answering.

### Domain Model Diagram

![domain model diagram](./assests/Screenshot_146.png)

1. Request: Represents a user's request for a particular government service. It may have properties like request ID, user ID, and service ID.
2. Service: Represents a government service
3. Instruction: Represents the instructions provided to the user for completing a task related to a government service. like instruction ID, service ID, step description, and additional resources.
4. Feedback: Represents the user follow up information

finally we dont need to Use a Database.
