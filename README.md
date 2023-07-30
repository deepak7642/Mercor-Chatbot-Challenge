# ***Mercor Chatbot Challenge***

This challenge revolves around building innovative chatbots with low codes and layman understandable. 

for more details click here : [Mercor Chatbot Challenge](https://unstop.com/hackathons/mercor-chatbot-challenge-mercor-715192)

**Below is my one of the submission for it**

---

## **Mini JD Generator App (Documentation) : -**

### **App Creator:**
The Mini JD Generator App is created by Deepak Kaura, an enthusiastic Data Scientist. The app utilizes the Open Assistant language model, which is an open-source GPT model, to provide accurate and detailed job responsibilities based on the user's inputs.

### **Overview:**

The Mini JD Generator App is a user-friendly web application built to automatically generate job descriptions. It utilizes advanced natural language processing technology to produce detailed job responsibilities based on user-provided information. This app is designed to save time for HR professionals by automating the process of writing job descriptions.

----------------------------------------

### **Input Fields:**

* **Job Title:** Enter the title of the job you want to create a description for.

* **Work Experience Required:** Specify the number of years of experience required for the job.

* **Company Name:** Provide the name of the hiring company.

* **About Company:** Enter a brief description of the company.

* **Company's Number of Employees:** Input the number of employees in the company.

* **Job Location:** Specify the location of the job.

* **Date Posted:** Select the date of posting the job.

### **Next step is Generating Job Description**

- Fill in all the required input fields.

- Click on the "Generate Job Description" button.

- The app will use the input provided to generate relevant job responsibilities.

- The generated job responsibilities will be displayed below the input fields.

***Please note that the app uses a GPT-based language model, and the quality of the generated job description may vary based on the input provided.***


---------------------------


### **Advantages:**

1. **Automated Job Description Generation**: The app automates the process of generating job descriptions. This can save time and effort for HR professionals who often need to write multiple job descriptions for different roles.

2. **Customizable Input**: The app allows users to input specific details such as job title, work experience required, company name, and job location. This ensures that the generated job description is tailored to the specific requirements of the role and the company.

3. **User-Friendly Interface**: Streamlit provides a simple and interactive web interface for the app, making it easy for users to input information and generate the job description with just a click of a button.

4. **Integration with GPT Model**: The app leverages a pre-trained GPT text generation model to create the job responsibilities. Using a powerful language model ensures that the generated text is coherent and contextually relevant.

5. **Expandable and Maintainable**: The code is organized into functions and follows best practices for modularization. This makes it easy to add more features or make changes to the app in the future.

6. **Open Source and Community Support**: The app is built using open-source tools, including Streamlit and the Open Assistant GPT model. This allows developers to contribute, collaborate, and benefit from the advancements in the community.

7. **Easy Deployment**: Streamlit apps are relatively easy to deploy, making it convenient to share the job description generator with other users or within an organization.

8. **Data Privacy**: Since the job description generation is done on the client-side (in the user's browser), sensitive information about the job details remains on the user's device and is not sent to a server, enhancing data privacy.

-------------------------------


### **Limitations:**

1. **User Input Validation**: The code does not validate the user inputs thoroughly. For example, it should check if the date entered is in the correct format or if the experience years are numerical. Proper validation will prevent unexpected errors during job description generation.


2. **Text Formatting**: The code concatenates strings to create the job details and the final job responsibilities, but there might be issues with proper text formatting (e.g., extra spaces, etc.). Using a templating library or dedicated formatting functions can make the code more robust and maintainable.

3. **User Interface**: The current user interface is minimal and straightforward. Depending on the target users, it may require further improvements to enhance user experience and usability.

----------------


### **Tools and Languages Used:**

- **Python:** The programming language used to write the entire application.

- **Streamlit:** An open-source Python library used for creating web applications for data science and machine learning projects. It allows for easy integration and visualization of data and model outputs.

- **Open-Source GPT Model:** The language model used for generating job responsibilities based on the provided inputs. The model is hosted on the Open Assistant and accessed through the text_generation library.

--------

### **Architecture Overview:**
 The main components of the architecture are as follows:

1. **Streamlit Integration:**
   - Install Streamlit: Install the Streamlit library using pip or conda in the development environment.
   - Create Streamlit App: Set up a new Python file to create the Streamlit web application.
   - Import Dependencies: Import the necessary libraries, including Streamlit and other required packages.
   - Load Model: Load the OpenAssistant GPT model into memory, allowing it to generate text based on input prompts.
   - Set Up UI: Create a user-friendly interface using Streamlit widgets like text inputs, buttons, and dropdown menus to gather relevant job details from the user.
   - Define Callbacks: Define callback functions for event handling, such as when the user clicks the "Generate Job Description" button.

2. **OpenAssistant GPT Model:**
   - Choose Model: Select and download an appropriate pre-trained GPT model like OpenAssistant, which is fine-tuned for text generation tasks.
   - Model Loading: Implement a function to load the GPT model into memory, using a deep learning library like Hugging Face's transformers or TensorFlow.
   - Text Generation: Utilize the loaded model to generate job descriptions based on the provided job details.

3. **User Interface (UI):**
   - Design UI: Create a layout for the user interface, keeping it intuitive and easy to understand.
   - Input Fields: Add input fields for job title, work experience, company name, company description, number of employees, job location, and date posted.
   - User Input Validation: Implement validation to ensure that all required fields are filled correctly before generating the job description.

4. **Job Description Generation:**
   - Input Processing: Prepare the user-provided job details as input for the GPT model.
   - Text Generation: Pass the processed input to the GPT model to generate the job responsibilities.
   - Post-processing: Refine the generated text if necessary, to make it more coherent and accurate.

5. **Job Responsibilities Display:**
   - Output Layout: Design a visually appealing layout to display the job details and generated job responsibilities.
   - Output Rendering: Populate the output fields with the relevant information retrieved from the GPT model.
   - Clear Output: Provide an option to clear the output and allow the user to input new details for another job description generation.

6. **Deployment:**
      - Deploy App: Deploy the Streamlit app to the chosen platform, ensuring that the GPT model and all dependencies are correctly set up.
   - Testing: Thoroughly test the deployed app to identify and fix any issues that may arise during real-world usage.



7. **Feedback:**
   
   - Collect User Feedback: Gather feedback from users to understand their experience and any additional features they might find useful.

-----

### **Data Flow Diagram:**


                   +-----------------+
                   | User Input Form |
                   +-----------------+
                             |
                             | (job_title, work_experience_required, company_name, about_company, no_of_employees, job_location, date_posted)
                             v
                  +---------------------------+
                  | Main Function - main()    |
                  +---------------------------+
                             |
                             | (job_title, work_experience_required, company_name, about_company, no_of_employees, job_location, date_posted)
                             v
         +-----------------------------------------------+
         |          generate_job_responsibilities()    |
         +-----------------------------------------------+
                             |
                             | (job_title, work_experience_required, company_name, job_location)
                             v
                  +---------------------------------+
                  |  GPT-3.5 Text Generation Model  |
                  +---------------------------------+
                             |
                             |  Generated Job Responsibilities
                             v
                   +------------------------+
                   | Display Job Responsibilities |
                   +------------------------+



#### **Conclusion:**
The Mini JD Generator App is a powerful tool for HR professionals to streamline the job description creation process. With its user-friendly interface and automated job responsibilities generation, it significantly enhances efficiency and accuracy in the hiring process. Utilize the app to generate comprehensive job descriptions tailored to your company's specific requirements.
