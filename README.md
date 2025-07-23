# Smart Voice-Based Ticket Analytics System 🗣️🎫📊

## Table of Contents

  * [Project Overview](https://www.google.com/search?q=%23project-overview)
  * [Features](https://www.google.com/search?q=%23features)
  * [Technologies Used](https://www.google.com/search?q=%23technologies-used)
  * [Installation and Setup](https://www.google.com/search?q=%23installation--setup)
  * [Usage](https://www.google.com/search?q=%23usage)
  * [Contact](https://www.google.com/search?q=%23contact)

-----

## Project Overview

The Smart Voice-Based Ticket Analytics System is an advanced deep learning-based system designed to streamline customer support operations by leveraging voice-enabled interfaces and artificial intelligence. This system captures customer queries in real-time, converts speech to text, extracts user intent using advanced language models, and generates analytical insights from support tickets. Hosted in Azure cloud, the project utilizes Generative AI (Gemini API) and OpenAI's GPT API technologies to automate ticket categorization, prioritization, and response analysis, significantly improving efficiency and intelligence in customer support processes.

## Features

This system offers a comprehensive set of features to manage and analyze customer support tickets:

1.  **Dashboard:**
      * **Purpose:** Provides a centralized, visual overview of key metrics and insights related to ticket trends, system performance, and common customer issues.
      * **Method:** Displays interactive charts and graphs summarizing ticket volumes, priority distribution, and resolution times.
      * **Outcome:** Enables quick identification of bottlenecks and overall system health.
2.  **Voice-to-Text Converter:**
      * **Purpose:** To enable natural language input by converting spoken customer queries into text.
      * **Method:** Leverages robust speech recognition technology (integrated via OpenAI GPT API) to accurately transcribe real-time voice input.
      * **Outcome:** Facilitates hands-free interaction and quick capture of customer issues.
3.  **Keyword Storage:**
      * **Purpose:** To store important keywords and phrases extracted from customer queries for efficient search, categorization, and future analysis.
      * **Method:** Processes the converted text through NLP techniques to identify and save relevant keywords into a database.
      * **Outcome:** Improves data organization and retrievability for support agents.
4.  **AI-Powered Chatbot:**
      * **Purpose:** To intelligently understand customer problems, prioritize them, and provide automated responses.
      * **Method:** Utilizes OpenAI GPT API to extract intent, classify problem types, and assign priority levels (e.g., Low, Medium, High, Urgent), storing this information in a database.
      * **Outcome:** Automates initial triage, reducing manual workload and speeding up response times.
5.  **View List (Ticket Management):**
      * **Purpose:** To display a comprehensive list of all tickets raised by customers, providing a clear overview of support requests.
      * **Method:** Fetches ticket details (including problem description, extracted keywords, and priority level) from the database and presents them in a sortable and filterable list.
      * **Outcome:** Enables support teams to easily track and manage customer issues.
6.  **Mail Tab (Complaint Submission):**
      * **Purpose:** To allow users to submit complaints or queries directly via email, with automated processing of the email content.
      * **Method:** Redirects users to Gmail using **OAuth** for secure authentication. Upon sending, the system parses the email content, extracts keywords, and determines the problem's priority level, storing them in the database.
      * **Outcome:** Provides an alternative, familiar channel for submitting complaints while ensuring system integration.

## Technologies and Tools Used

  * **Cloud Platform:** Azure (for hosting and various cloud services)
  * **Generative AI:**
      * OpenAI GPT API (for voice-to-text conversion, intent extraction, and chatbot functionalities)
  * **Authentication:** OAuth (for secure mail integration)
  * **Programming Language:** python
  * **Database:** (Supabase)
  * **Front-end Technologies:** (Node.js, React.js and Tailwind CSS)

## Installation & Setup

To get a copy of the project up and running on your local machine for development and testing purposes, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [YOUR_REPOSITORY_URL_HERE]
    cd ticket-managment-system
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate # On Windows: `venv\Scripts\activate`
    ```
3.  **Install the required dependencies:**
  
4.  **Configure API Keys and Environment Variables:**
      * Obtain your **Google Gemini API Key** from the Google AI Studio.
      * Obtain your **OpenAI GPT API Key** from the OpenAI platform.
      * Set up your **OAuth 2.0 credentials** for Gmail API if you're using direct Gmail integration for sending/receiving.
      * Create a `.env` file in the root directory of your project and add the following:
        ```
        GEMINI_API_KEY="your_gemini_api_key_here"
        OPENAI_API_KEY="your_openai_api_key_here"
        DATABASE_URL="your_database_connection_string_here"
        # Add any other necessary environment variables, e.g., for OAuth client IDs/secrets
        OAUTH_CLIENT_ID="your_google_oauth_client_id"
        OAUTH_CLIENT_SECRET="your_google_oauth_client_secret"
        ```

## Usage

This project includes a web application for demonstrating the voice-based ticket creation, management, and analytics.

1.  **Ensure all dependencies are installed, and environment variables/API keys are configured.**
2.  **Run the Flask application (or your main application file):**
    ```bash
    python app.py
    ```
3.  **Access the web interface:**
    Open your web browser and navigate to `http://127.0.0.1:5000/` (or the address where your application is hosted).
4.  **Interact with the system:**
      * **Voice-based Ticket Creation:** Click on the designated button (e.g., "Speak your query") and speak clearly. The system will convert your speech to text, analyze it, and create a ticket.
      * **Chatbot Module:** Engage with the chatbot to get automated prioritization and insights on problems.
      * **View Tickets:** Browse the "View Tickets" section to see a list of all submitted tickets, their keywords, and priority levels.
      * **Email Complaints:** Use the "Mail Complaints" feature to be redirected to Gmail, where you can send an email that will be processed by the system.

## Contact

For any questions or collaborations regarding this project, please feel free to reach out to:

  * **Arun S:**
  * www.linkedin.com/in/arun2k04 *

-----
