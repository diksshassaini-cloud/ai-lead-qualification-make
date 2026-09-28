# AI Lead Qualification Workflow (Make.com)

A no-code automation that scores every new marketing lead with AI and sends a personalized reply. Built as a demo for a fictional marketing agency and tested with sample lead data.

## The problem
Sales teams lose time reading every inquiry to decide which leads deserve a fast response.

## The solution
When a lead submits the form, the workflow scores it with Google Gemini, sorts it as Hot, Warm or Cold, logs the result, and emails the lead a message that fits their category.

## How it works
1. **Google Form** collects the lead's name, email, job title, company size, service needed, budget and goals
2. **Google Sheets** stores the response and triggers the scenario
3. **Google Gemini AI** scores the lead from 1 to 100, assigns Hot/Warm/Cold, and writes a reason and a personalized opening line
4. **Parse JSON** splits the AI answer into separate fields
5. **Google Sheets** logs the lead and AI results in a "Scored Leads" tab
6. **Router + Gmail** sends a different email for Hot, Warm and Cold leads

## Tools
Make.com, Google Forms, Google Sheets, Google Gemini API, Gmail, prompt engineering, JSON parsing

## Results
- Scores and categorizes a lead in 60 seconds, compared with about 5 minutes manually
- Tested on 2 sample leads across all three categories
- [Add anything else you measured]

## Files
- `blueprint.json`: import into Make to reproduce the scenario
- `prompt.txt`: the AI scoring prompt
- `screenshots/`: the scenario, the form and the results sheet

## Note
This is a demo project. All lead data is fictional and no real customer information is used.
