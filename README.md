# <Circular clock >


## Problem
RBI keeps replacing and amending its Master Directions, and old PDFs stay on staff laptops. Compliance officers waste hours checking whether a paragraph they remember is still valid, and branch staff sometimes follow withdrawn rules.

##  Who it is for

1. **Compliance officers at NBFCs and banks:** For example, a compliance officer at a mid-sized gold-loan NBFC in Coimbatore who needs to monitor RBI updates and ensure branches follow the latest applicable regulations.

2. **Common people and bank customers:** People who want to verify RBI rules related to gold loans, home loans, and education loans, understand applicable interest-rate requirements, and check whether their bank's terms and conditions comply with the relevant RBI directions.

**Example:** A customer taking a gold loan can ask CircularClock what RBI rules apply to gold valuation, loan-to-value (LTV) limits, and interest disclosures, then compare those requirements with the terms offered by their lender.


## Signature feature
Time-travel' date picker: ask any question as of a past date and see the answer that was legally correct then.

## Hardest problem (my interview story)

 	
Versioning: latest valid version. Each paragraph is stored with valid-from and valid-to dates, so a question 'as on 1 April 2025' and 'as on today' can give different, correctly cited answers. A side-by-side diff shows exactly which lines changed between two versions.

| Source                                     | Link                                                                                                           | Documents           | Pages         | Licence / terms                                   |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------- | ------------------- | ------------- | ------------------------------------------------- |
| RBI Master Directions                      | [Official website](https://www.rbi.org.in/Scripts/BS_ViewMasterDirections.aspx?utm_source=chatgpt.com)         | 60+ target          | 1,500+ target | RBI website terms; verify reuse conditions        |
| RBI Notifications and Circulars            | [Official notifications](https://www.rbi.org.in/Scripts/NotificationUser.aspx?utm_source=chatgpt.com)          | 100+ target         | To be counted | RBI website terms; retain source and date         |
| RBI Gold and Silver Collateral Directions  | [Official RBI website](https://www.rbi.org.in/Scripts/NotificationUser.aspx?utm_source=chatgpt.com)            | 1+ initial document | To be counted | Official RBI document; verify reuse conditions    |
| RBI NBFC Scale-Based Regulation Directions | [Official document](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=12550\&utm_source=chatgpt.com) | 1+ initial document | To be counted | Official RBI document; preserve amendment history |
## 10 real questions
# CircularClock — 10 Real Questions

1. What is the current RBI loan-to-value (LTV) limit for NBFC gold loans?
2. What gold-loan rules were applicable on 1 April 2023?
3. How must lenders determine the value of gold pledged as collateral?
4. What must an NBFC disclose about gold-loan interest rates and charges?
5. What RBI rules govern interest-rate changes on floating-rate home loans?
6. What RBI requirements apply to banks offering education loans?
7. Which RBI paragraph covers the conduct of loan recovery agents?
8. What changed in the RBI Scale-Based Regulation framework in a specified amendment?
9. Which version of an RBI Master Direction was valid on 1 April 2025?
10. What new RBI directions or amendments have affected NBFC gold loans, and when did they become effective?

## Expected chatbot behaviour

- Cite the official RBI document and relevant paragraph.
- Identify the applicable version and effective date.
- Support historical and current-date questions.
- Explain changes between versions.
- Say when reliable evidence is unavailable rather than inventing an answer.

## Run it
```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements-dev.txt
cp .env.example .env                                 # Windows: copy .env.example .env
uvicorn app.main:app --reload
curl localhost:8000/health
```

## Live link

