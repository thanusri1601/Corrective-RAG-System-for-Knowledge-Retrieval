# CRAG: Corrective Retrieval-Augmented Generation System

## Setup

### 1. Clone the Repository
git clone https://github.com/your-username/CRAG-System.git  
cd CRAG-System

---

### 2. Create Virtual Environment
python3 -m venv venv  
source venv/bin/activate  

Python 3.10+ recommended.

---

### 3. Install Dependencies
pip install --upgrade pip  
pip install -r requirements.txt  

---

## Running the Application

### Local Execution
streamlit run app.py  

Access the application at:  
http://localhost:8501

---

## AWS EC2 Deployment

This project is deployed on an AWS EC2 Ubuntu instance.

### Deployment Steps
1. Launch an Ubuntu EC2 instance  
2. Open port 8501 in the EC2 security group  
3. Clone this repository on the EC2 instance  
4. Create and activate a Python virtual environment  
5. Install required dependencies  
6. Run the Streamlit application  

Run the application on EC2 using:
streamlit run app.py --server.port 8501 --server.address 0.0.0.0  

### Live Deployment
http://ec2-54-237-214-22.compute-1.amazonaws.com:8501

---

## Output

- Interactive Streamlit-based user interface  
- Corrective Retrieval-Augmented Generation workflow  
- Reduced hallucinations through validation and corrective retrieval  
- Publicly accessible AWS EC2 deployment  

---

## Project Structure

CRAG-System/  
├── app.py  
├── agents/  
│   ├── retriever.py  
│   ├── generator.py  
│   └── validator.py  
├── assets/  
│   ├── workflow_graph.png  
│   ├── ui_output.png  
│   └── aws_deployment.png  
├── requirements.txt  
└── README.md  

---

## Workflow Graph

![CRAG Workflow](assets/workflow_graph.png)

---

## Application Output

![Streamlit Output](assets/ui_output.png)

---

## AWS Deployment Screenshot

![AWS EC2 Deployment](assets/aws_deployment.png)

---

## Technologies Used

- Python  
- LangChain  
- LangGraph  
- FAISS Vector Store  
- OpenAI API  
- Streamlit  
- AWS EC2  

---

## Key Contributions

- Implemented Corrective Retrieval-Augmented Generation (CRAG) to improve factual grounding  
- Designed an agent-based workflow using LangGraph  
- Introduced validation and corrective retrieval to mitigate hallucinations  
- Deployed an end-to-end LLM system on AWS EC2  

---

## Notes

- Internet connectivity is required for API calls  
- Mermaid graph rendering may fail if external APIs are unavailable  
- Tested on Ubuntu 22.04 (AWS EC2)  

---

## Author

Thanusri A  
Aspiring Data Science Intern | LLM Systems | Agentic AI  

---

If you find this project useful, please consider giving it a star ⭐
