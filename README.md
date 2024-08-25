# PWC-POWER-BI-INTERNSHIP






Task 1 Call Centre KPI

Create a dashboard in Power BI for visualizing relevant KPIs and metrics in the dataset provided.
Utilize the resources provided, including podcasts and articles, to enhance your understanding of data visualization and upskilling.
Respond to the client's request by providing a well-designed Power BI dashboard reflecting the requested KPIs.

PROBLM STATEMENT
Overall customer satisfaction
Overall calls answered/abandoned
Calls by time
Average speed of answer
Agent’s performance quadrant -> average handle time (talk duration) vs calls answered

Measures used
Answered calls= Calculate(Count(Sheet1 [Callid]),Filter(Sheet1,Sheet1(Answered(Y/N)="Y"))
Calls Not Answered = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Answered (Y/N)]="N"))
Not Resolved = CALCULATE(COUNT(Sheet1[Topic]),FILTER(Sheet1,Sheet1[Resolved]="N"))
Resolved Calls = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Resolved]="Y"))
Total = COUNT(Sheet1[Call Id])
![Screenshot (12)](https://github.com/user-attachments/assets/ce88574c-b95f-4386-a40a-dbe07bf96132)
