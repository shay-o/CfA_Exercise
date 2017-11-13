# CfA_Exercise

 From https://gist.github.com/bensheldon/267137a74f759e746a768c579decc9b1
 
 This part of the application consists of an exercise that should take you up to 2 hours to complete. Please read all the way through the instructions before beginning - you should time yourself once you start.

## Background

When applying for SNAP (food stamps), an applicant must complete an application that includes information about everyone in their household, submit verification documents (e.g. copies of pay-stubs and drivers license), and be interviewed by an eligibility worker. Typically applicants have 30 days to complete this process after which they receive an approval or denial.

## The Exercise

Using the tools of your choosing we would like you to analyze the provided data and produce a brief report and recommendation. This report should include:

1. An analysis of the data in two respects:
   - What application attributes/qualities correlate with approved SNAP applications? 
   - What demographics patterns (if any) exist within the data?
2. Given the previous analysis, what is your recommendation(s) for where a service delivery team should focus their efforts for maximum impact. For example:
   - Where to focus marketing and outreach
   - Where to focus product development that guides clients through the SNAP application process
3. A brief summary of how you performed the analysis (tools/approach). Given the time constraints, you might also note any compromises or describe an ideal analysis.

### The Data

**applications.csv**: information about a SNAP application
  - id: the identifier of the application, used across sheets
  - uploaded_documents: the number of verification documents that are included with the application
  - interview_preference: whether the applicant prefers to be interviewed in-person or by telephone
  - subscribed_to_reminders: whether the applicant opted-in to receive automated reminders about process and deadlines

**members.csv**: members of the applicant's household
  - application_id: reference to the application 
  - is_submitter: whether this data represents the person submitting the application
  - sex: binary sex of the member (Male/Female)
  - age: age of the member in years

**outcomes.csv**: whether the application was approved or denied 
  - application_id: reference to the application 
  - status: whether the application was approved/denied
