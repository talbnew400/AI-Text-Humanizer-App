# 1. Clone the project to your computer
git clone https://github.com/DadaNanjesha/AI-content-detector-Humanizer.git

# 2. Go inside the project folder
cd AI-content-detector-Humanizer

# 3. Create a clean virtual environment
python -m venv venv

# 4. Activate the virtual environment
# (If you are on Windows, use: .\venv\Scripts\Activate.ps1 instead)
source venv/bin/activate

# 5. Upgrade pip and install all required packages
pip install --upgrade pip
pip install -r requirements.txt

# 6. Download the required AI and language models
python -m spacy download en_core_web_sm
python -c "import nltk; nltk.download('punkt'); nltk.download('wordnet'); nltk.download('averaged_perceptron_tagger');"

# 7. Start your Streamlit app!
streamlit run app.py
