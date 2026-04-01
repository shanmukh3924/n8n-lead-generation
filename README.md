# n8n Lead Generation Workflow

## About this project

I built this project to automate a simple problem — collecting leads and storing them without doing everything manually.

Earlier, I had to copy data one by one, which was slow and boring. So I created this workflow using n8n to handle everything automatically.

---

## What this workflow does

* Takes data from an API (Apify)
* Processes the response
* Handles multiple results properly (looping)
* Stores the final data into Google Sheets

---

## How it works (my approach)

I designed the workflow step by step:

1. Start with a trigger (manual for testing)
2. Use HTTP Request node to get data
3. Clean and format the data using Set node
4. Fix the issue of only one item by adding proper looping
5. Send each item to Google Sheets

Initially, I had a problem where only one record was getting stored.
I fixed it by understanding how n8n handles items and loops.

---

## Files included

* `lead-gen-workflow.json` → main workflow
* `README.md` → this file

---

## How to run it

1. Import the JSON file into n8n
2. Add your credentials:

   * Google Sheets
   * Apify API
3. Execute the workflow

---

## Output

The workflow stores structured lead data in Google Sheets.
Each row represents one lead.

---

## Challenges I faced

* JSON format errors while sending requests
* Only one item getting stored in Google Sheets
* Understanding how looping works in n8n

---

## What I learned

* How n8n workflows actually process data
* How APIs return data and how to handle it
* Importance of looping when dealing with multiple items
* Debugging workflow errors step by step

---

## Future improvements

* Add scheduling (automatic runs)
* Improve data filtering
* Add more sources for lead generation

---

## About me

I am currently learning automation and building projects using n8n.
This is one of my practice projects to improve my skills.

