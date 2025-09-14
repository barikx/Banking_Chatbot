Detecting Hazardous Space Objects Around Earth with Artificial Intelligence and Machine Learning

To run the FastAPI app using Anaconda Prompt, follow these steps:

✅ Step-by-Step Instructions
🔹 1. Open Anaconda Prompt
Launch Anaconda Prompt from your Start Menu (not Jupyter or Python console).

🔹 2. Navigate to the Project Folder
Unzip the file you downloaded (neo_fastapi_app.zip), then use cd to move into that folder:
cd path\to\neo_fastapi_app
Example (if you unzipped on Desktop):
cd C:\Users\YourName\Desktop\neo_fastapi_app

🔹 3. Create and Activate a New Conda Environment (optional but recommended)
conda create -n neoapp python=3.10 -y
conda activate neoapp

🔹 4. Install the Requirements
pip install -r requirements.txt
If you see any errors related to xgboost, you may run:
conda install -c conda-forge xgboost

🔹 5. Add Your Model File
Make sure your model.xgb file is copied into this directory:
neo_fastapi_app/
├── app.py
├── model.xgb  ← make sure this exists here
├── requirements.txt
└── static/

🔹 6. Run the FastAPI App
uvicorn app:app --reload
You should see output like:
    Uvicorn running on http://127.0.0.1:8000

🔹 7. Open in Browser
Visit:
http://127.0.0.1:8000
You’ll see your NEO prediction interface.


