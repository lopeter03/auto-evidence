
Auto Evidence QA Demo – Specification

Purpose  
Provide a self‑contained QA/UAT demo project that:  
- Automates login test cases  
- Captures evidence (screenshots, logs)  
- Generates a professional Word report  

Components  
- demo_site.html → simple login page with valid/invalid accounts  
- login_test_data.csv → 12 test cases (7 valid, 3 invalid, 2 mismatches)  
- browser_test.py → Selenium automation script  
- Fail_Report.docx → generated report with summary + fail case details  

Workflow  
1. setup_project.py expands folders and demo files.  
2. browser_test.py runs test cases against demo_site.html.  
3. Evidence is captured:  
   - CSV log  
   - Screenshots  
   - Word report  
4. User can review outputs in reports/.  

Test Case Design  
- Valid accounts: test, alice, bob, charlie, david, eva, frank  
- Invalid accounts: george, wrong, hacker  
- Mismatch cases: ghost, intruder  

Evidence Capture  
- Each test case logs Pass/Fail result.  
- Fail cases are highlighted in the Word report.  
- Screenshots are embedded for fail cases.  

Deliverables  
- README.me → overview + quick start  
- spec.md → technical specification  
- src/setup_project.py → expands project structure  
- Test Result.docx → consolidated evidence file with screenshots and summarized results  

