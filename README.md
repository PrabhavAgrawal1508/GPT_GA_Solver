# GPT_GA_Solver

This repository has the second project for the Course _Tools in Data Science_ in IIT Madras B.S in Data Science and Programming Degree

# Setup
* Clone this repository
* Create a virtual environment: 
  ```bash
  python -m venv venv
  ```
* Activate the virtual environment:
  ```bash
  source venv/bin/activate  
  ```
* Install dependencies: pip install -r requirements.txt
  ```bash
  pip install -r requirements.txt
  ```
* Create a .env file with your AIPROXY_TOKEN
* Run the server:
 ```bash
  uvicorn app.main:app --reload
 ```


# How To Use
Send a POST request to the /api/ endpoint with:
```bash
curl -X POST "http://localhost:8000/api/" \
  -H "Content-Type: multipart/form-data" \
  -F "question=Your Question Here" \
  -F "file=@yourfile.abcd"
```