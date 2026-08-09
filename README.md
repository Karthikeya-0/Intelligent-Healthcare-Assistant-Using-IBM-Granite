HealthAI: Intelligent Healthcare Assistant Using IBM Granite 🏥🤖HealthAI is an AI-driven, real-time healthcare assistant leveraging IBM Granite Large Language Models (LLMs) and Streamlit. Designed to bridge the gap between complex medical information and everyday users, HealthAI offers empathetic conversational support, symptom-based disease evaluation, personalized treatment recommendations, and vital signs health analytics.🌟 Key Features1. 💬 Patient Chat (chat_interface.py)Empathetic QA: Provides reliable health, wellness, and medical information in easy-to-understand language.Guardrailed Responses: Context-aware prompts powered by IBM Granite with built-in safety boundaries to ensure responsible, non-diagnostic guidance.2. 🦠 Disease Prediction (disease_predictor.py)Symptom Analysis: Analyzes user-reported symptoms (e.g., fever, persistent cough, fatigue, headache).Smart Matching: Combines rule-based clinical matrices and model reasoning to outline potential conditions for further investigation by a physician.3. 💊 Personalized Treatment Plans (treatment_generator.py)Tailored Care Advice: Generates custom treatment guidelines incorporating patient demographics (age, gender, pre-existing conditions).Actionable Recommendations: Details standard over-the-counter considerations, lifestyle/dietary modifications, home care routines, and suggested diagnostic tests.4. 📊 Health Analytics Dashboard (analytics_dashboard.py)Vitals Tracker: Log and monitor key health vitals including Blood Pressure (BP), Heart Rate, Blood Sugar, and Pulse.Visual Trend Analysis: Powered by pandas and matplotlib to render trend graphs and highlight abnormal metric spikes.AI Health Insights: Summarizes historical trends with actionable wellness tips.🛠️ Technology StackFrontend: StreamlitBackend: Python 3.8+AI Model: IBM Granite (ibm/granite-13b-instruct-v2 / ibm/granite-3.2b-instruct via IBM Watsonx.ai or Hugging Face)Data Processing & Visualization: Pandas, NumPy, MatplotlibEnvironment Configuration: python-dotenv📁 Repository StructureIntelligent-Healthcare-Assistant-Using-IBM-Granite/
├── app.py                      # Main Streamlit web application entry point
├── disease_predictor.py        # Disease prediction logic & interface
├── treatment_generator.py      # Personal treatment plan generator module
├── chat_interface.py           # Conversational patient assistant
├── analytics_dashboard.py      # Health vitals visualizer & dashboard
├── requirements.txt            # Python package dependencies
├── .env.example                # Sample environment configuration file
└── README.md                   # Project documentation
⚙️ Installation & SetupPrerequisitesPython 3.8+ installed on your system.An API Key for IBM Watsonx.ai or Hugging Face to query IBM Granite models.Step-by-Step InstructionsClone the Repositorygit clone https://github.com/Karthikeya-0/Intelligent-Healthcare-Assistant-Using-IBM-Granite.git
cd Intelligent-Healthcare-Assistant-Using-IBM-Granite
Create and Activate a Virtual Environment# Windows
python -m venv venv
venv\Scripts\activate

# macOS / Linux
python3 -m venv venv
source venv/bin/activate
Install Dependenciespip install -r requirements.txt
Configure Environment VariablesCreate a .env file in the project root directory (or copy .env.example):IBM_WATSONX_APIKEY=your_ibm_watsonx_api_key_here
WATSONX_PROJECT_ID=your_watsonx_project_id_here
# Alternative: Hugging Face Token (if accessing via HF Hub)
HF_TOKEN=your_huggingface_token_here
Launch the Applicationstreamlit run app.py
Access the web application in your browser at http://localhost:8501.🚀 Usage GuidePatient Chat: Navigate to the chat tab to ask general health and wellness questions.Disease Prediction: Select your symptoms from the options provided and click Analyze to review potential medical insights.Treatment Generator: Fill in medical context (age, gender, pre-existing conditions) and condition names to receive personalized care suggestions.Health Analytics: Input vital statistics (BP, heart rate, blood sugar) to view interactive charts and trend summaries.🛡️ DisclaimerIMPORTANT MEDICAL NOTICE:HealthAI is developed strictly for educational, demonstration, and research purposes. It is NOT a replacement for professional medical advice, diagnosis, or treatment. Always consult with a qualified healthcare professional regarding any medical conditions or health decisions.🤝 ContributingContributions are welcomed! Follow these steps to contribute:Fork this repository.Create a feature branch (git checkout -b feature/AmazingFeature).Commit your changes (git commit -m 'Add AmazingFeature').Push to the branch (git push origin feature/AmazingFeature).Open a Pull Request.📜 LicenseDistributed under the MIT License.
