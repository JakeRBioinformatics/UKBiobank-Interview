# Mock Health Data API & UI Automation

This is a small-scale demonstration project built to simulate Create/Read/Update/Delete operations on anonymised health data — with a focus on test automation, data persistence, and full-stack observability.

---

Project Features

- FastAPI-based RESTful API > for managing anonymised health data
- CSV-backed data persistence > to simulate real-world record storage
- Mock HTML UI > that interacts with the API (file-based, JS-powered)
- Playwright automation > to test Add, Edit, and Delete workflows
- Timestamped logging > for both API and UI actions

---

Sample Data Model (CSV)

csv
patient_id,age,sex,BMI,diagnosis_code,sample_taken,blood_pressure,cholesterol_level
PAT1000,67,Female,17,I75,FALSE,141/79,7.8

Setup Instructions: 

1) Install dependencies

pip install fastapi uvicorn httpx nest_asyncio pydantic playwright
playwright install

2) Run the FastAPI server

uvicorn main:app --reload

3) Open the UI

Open mock_ui.html in your browser

4) Run Playwright UI tests

await test_add_patient("TEST999")
await test_edit_patient("TEST999", "50", "26.5")
await test_delete_patient("TEST999")

Log files: 

api_requests.log — API activity (POST, PUT, DELETE)
ui_test_actions.log — Playwright test steps

Author

Jake (UK-based software tester) 
Interview-ready demonstration build in June 2025 
Python • FastAPI • Playwright • Jupyter


