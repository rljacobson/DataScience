# Data Set

Description from the [source website](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing).

## Bank Client Data

| **idx** | **Column** | **Type**    | **Values**                                                   | **Column Description** |
| ------- | ---------- | ----------- | ------------------------------------------------------------ | ---------------------- |
| 1       | age        | numeric     |                                                              |                        |
| 2       | job        | categorical | admin., blue-collar, entrepreneur, housemaid, management, retired, self-employed, services, student, technician, unemployed, unknown | type of job            |
| 3       | marital    | categorical | divorced, married, single, unknown; note: divorced means divorced or widowed | marital status         |
| 4       | education  | categorical | basic.4y, basic.6y, basic.9y, high.school, illiterate, professional.course, university.degree, unknown |                        |
| 5       | default    | categorical | no, yes, unknown                                             | has credit in default? |
| 6       | housing    | categorical | no, yes, unknown                                             | has housing loan?      |
| 7       | loan       | categorical | no, yes, unknown                                             | has personal loan?     |

## Data related with the last contact of the current campaign

| **idx** | **Column**  | **Type**    | **Values**                   | **Column Description**                                       |
| ------- | ----------- | ----------- | ---------------------------- | ------------------------------------------------------------ |
| 8       | contact     | categorical | cellular, telephone          | contact communication type                                   |
| 9       | month       | categorical | jan, feb, mar, ..., nov, dec | last contact month of year                                   |
| 10      | day_of_week | categorical | mon, tue, wed, thu, fri      | last contact day of the week                                 |
| 11      | duration    | numeric     |                              | last contact duration, in seconds. **Important note:** this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model. |

## "Other Attributes"

| **idx** | **Column** | **Type**    | **Values**                    | **Column Description**                                       |
| ------- | ---------- | ----------- | ----------------------------- | ------------------------------------------------------------ |
| 12      | campaign   | numeric     |                               | number of contacts performed during this campaign and for this client, includes last contact |
| 13      | pdays      | numeric     | 999                           | number of days that passed by after the client was last contacted from a previous campaign (999 means client was not previously contacted) |
| 14      | previous   | numeric     |                               | number of contacts performed before this campaign and for this client |
| 15      | poutcome   | categorical | failure, nonexistent, success | outcome of the previous marketing campaign                   |

## Social and Economic Context Attributes

| **idx** | **Column**     | **Type** | **Values** | **Column Description**                          |
| ------- | -------------- | -------- | ---------- | ----------------------------------------------- |
| 16      | emp.var.rate   | numeric  |            | employment variation rate - quarterly indicator |
| 17      | cons.price.idx | numeric  |            | consumer price index - monthly indicator        |
| 18      | cons.conf.idx  | numeric  |            | consumer confidence index - monthly indicator   |
| 19      | euribor3m      | numeric  |            | euribor 3 month rate - daily indicator          |
| 20      | nr.employed    | numeric  |            | number of employees - quarterly indicator       |

## "Output" (Outcome)

| **idx** | **Column** | **Type** | **Values** | **Column Description**                    |
| ------- | ---------- | -------- | ---------- | ----------------------------------------- |
| 21      | default    | binary   | yes, no    | has the client subscribed a term deposit? |