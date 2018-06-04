# DigiBP-Eiger
# Introduction

In the following document, the documentation of the artefacts used for automising our recruiting process will be provided. 

_Authors:_ 

Charuta Pande, charuta.pande@students.fhnw.ch

Thomas Felder, thomas.felder@students.fhnw.ch

Yannick Godat, yannick.godat@students.fhnw.ch 

Pleurat Komani, pleurat.komani@students.fhnw.ch

# Company Background

We are mid-sized enterprise operating in the pharma industry in Basel/Switzerland. We cooperate with an external recruiting agency called yellow-shark to ensure that we have a constant supply of potential candidates for staffing our open positions. For our current open position we are looking for a programmer to help us develop our company App that will be supported in both Android and macOS operating systems.

## Design approach

We used a iterative design approach for digitalising our process:

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-03%20at%2000.16.35.png)

Immediately after each lecture we worked ourselves on the process. Afterwards during the coaching sessions we received and implemented the feedback we got from our coaches in a cyclic manner throughout the duration of the course. The more complex service integration tasks required extensive iteration until they were running in a seamless manner.  

## Project Plan & Milestones 

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2021.16.06.png)

## Collaboration

Given that this was a team-based assignment, it required considerable collaboration between the team-members. For this purpose, the GitHub repository for version control was used, which proved out to be very helpful for storing and documenting the input by all team-members

## Services, APIs & more 

For the automation of our process we have used:

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2016.23.03.png)

## Testing 

In order to identify bugs, and potential malfunctions in our process we have extensively undertaken tests. Individual (unit) testing was performed on local environments, whereas  integration testing on Heroku.

## Disclaimer

The documentation of the artefacts excludes the explanation of the process logic as it is expected that the readers of this documented have knowledge of BPMN 2.0 Notation and can navigate through the process by looking at the process models below. 

---------------------

# Process Models

## As-Is Process

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Recruitment_Process.png)

As it can be noted from the screenshot above, the As-Is process consisted of three pools:

* Internal Recruitment Process 

* YellowShark

* Applicant 

### As-Is Customer Journey

Our As-Is process was very complex, and required the involvement and coordination of many participants. Moreover, it was human-task centric and did not entail any automation. The recruitment process lacked a central system, and as consequence we received many complaints from our applicants, from which we were able to derive the following customer journey:

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.53.40.png)

## To-Be Process

A snapshot of the to-be process can be found below. It becomes apparent that the process has changed considerably. These changes are part of a larger digitalisation initiative inside the company which strives to make use of digitalisation in order to achieve cost-cutting and introduce digitally enhanced business processes in its environment. 

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/RecruitmentProcess_mail_dynamic_content_13.png)

Our To-Be recruiting process is made of the following Swimlanes and corresponding Pools/Participants:

_**Internal Recruiting process**_ - This swimlane represents our in-house recruiting process. There are the following participants:

* **Business Unit** - This pool represents the relevant business unit of our enterprise that has identified an staffing need and their corresponding activities.

* **HR Department** - This pool represents our Human Resource department and their corresponding activities.

* **Evaluation Team** - This pool represents the evaluation team, which is made up of upper management and the hiring manager.

_**YellowShark recruiting agency**_ - This swimlane represents the external company we cooperate with for our recruitment needs and their subsequent activities. The rationale behind modeling an external pool is to avoid deadlocks in our process.

### To-Be Customer Journey

After the successful automation of our recruitment process, our internal  KPI's showed that  we were able to handle more applications at a faster pace. Moreover we distributed surveys to our applicants which showed that they were very satisfied with the punctuality and response time of our process. Please view the figure below, to have a better understanding about the impact of the automation on the customer journey:

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.56.48.png)
---------------------

# Artefact Documentation 

## Camunda

### Embeded forms in camunda

### 1. Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.19.45.png)

### 1.1 Embedded Form:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2014.14.56.png)

### 2 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.23.11.png)

### 2.1 Embedded Form:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.30.15.png)

### 3 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.31.49.png)

### 3.1 Embedded Form:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.33.37.png)

### 4 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.36.20.png)

### 4.1 Embedded Form:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.38.20.png)

### 5 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.44.05.png)

### 5.1 Embedded Form:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.43.46.png)

### 6 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.48.07.png)

### 6.1 Embedded Form:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.47.50.png)

### 7 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.50.40.png)

### 7.1 Embedded Form:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.50.21.png)

### 8 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.54.15.png)

### 8.1 Embedded Form:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2019.53.50.png)

### 9 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.01.35.png)

### 9.1 Embedded Form:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.01.18.png)

----------------------------------------------------------------------------------------------

### Automatic E-mails.

### 1 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.10.56.png)

### 1.1 Automatic E-mail:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2015.06.50.png)

### 2 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.14.22.png)

### 2.1 Automatic E-mail:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2015.26.38.png)

### 3 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.17.49.png)

### 3.1 Automatic E-mail:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2015.20.07.png)

### 4 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.20.44.png)

### 4.1 Automatic E-mail:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2015.31.22.png)

### 5 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.23.10.png)

### 5.1 Automatic E-mail:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2016.54.38.png)

### 6 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.25.33.png)

### 6.1 Automatic E-mail:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2016.36.10.png)

### 7 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.28.06.png)

### 7.1 Automatic E-mail:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2017.15.10.png)

### 8 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.30.07.png)

### 8.1 Automatic E-mail:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2017.09.01.png)

### 9 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.32.55.png)

### 9.1 Automatic E-mail:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2016.58.35.png)

---------------------------------------------------------
### Embedded Decision Tables

### 1 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.37.55.png)

### 1.1 Embedded decision table:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2014.18.54.png)

### 2 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-02%20at%2020.40.03.png)

### 2.1 Embedded decision table:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-05-30%20at%2011.31.23.png)

---------------------------------------------------------

# Service Integration

## Integromat

### 1 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-03%20at%2022.37.03.png)

### 1.1 Service Integration:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-03%20at%2022.38.39.png)

In this check service, a webhook listens to a GET method. Once received, the service checks the google file Applicant Information’s second sheet, where the number of received applications is stored. The number is required to control the process flow, i.e. whether to extend the time frame (value equals 0) or processing the applications (value is above 0).

### 2 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-03%20at%2022.41.54.png)

### 2.1 Service Integration:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-03%20at%2022.51.06.png)

This service is mapped to the task “Get applicant information” and is responsible for getting the candidate information for the application processing. It reads from a Google Sheet the information for the different candidates that have applied so that it can be dynamically used for processing the application and sending either an e-mail containing the personal interview link or the rejection e-mail.

### 3 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2015.33.03.png)

### 3.1 Service Integration:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2015.34.49.png)

This service is mapped to the task “Get selected candidate details” and is responsible for getting the amount of candidates that have been invited for a personal interview so that multiple instantiations of the sub-process Candidate Evaluation for the candidate interview can be created.

### 4 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2015.36.22.png)

### 4.1 Service Integration:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2015.36.49.png)

This service is mapped to the task “Get legal approval data” and is responsible for getting two variables required by the following decision table. It reads from the Google Sheet HRModule - a file that mimics the decision logic of the company HR system. The output values are injected into the decision table “Determine vacancy approval” which controls the process flow. 

### 5 Save personal interview data

### 5.1 Service Integration:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2015.39.21.png)

This service is not mapped to a task, but to the digital assistant. Once an interview with the digital assistant is finished, the received data is stored intoa Google Sheet.

### 6 Store applicant Files

### 5.1 Service Integration:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2015.41.37.png)

This service is not mapped to a task, but constantly (interval of 15 minutes) listens whether an e-mail with attachments and a subject containing the word “Application” has been received. Once such an e-mail was registered, a Google Drive folder with the applicant’s name is created and the e-mail content as well as the folder id is store into a Google Sheet. The folder id will be required for an iFrame showing the applicant’s provided material. Afterwards, the attachments are stored into the applicant’s folder. 

--------------------------

### DocuSign 

### 1 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2022.17.14.png)

### 1.1 E-signature integration:
DocuSign helps HR organizations make key functions like hiring, onboarding, and benefits enrollment paper-free, so you can save time, reduce errors, increase compliance, and improve employee and candidates’ experience. With more than 40 signing languages and ease of integration with HRIS solutions, DocuSign helps meet the HR needs of global enterprises.
In our process there are two signing parties – the HR head and the employee. The contract is sent to the HR Head for signing. Once signed, the employee receives his/her copy for signing. After both parties sign, the document is available for download.

**Signer 1 - Email**

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2022.19.45.png)

**DocuSign signing – Signer 1**

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2022.21.31.png)

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2022.22.32.png)

**DocuSign signing – Signer 2**

![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2022.24.05.png)

-------------------------

### Dialogflow

### 1 Task:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2022.29.54.png)

### 1.1 Chatbot Integration:
![](https://github.com/DigiBP/digibp-eiger/blob/master/Documents/images/Screen%20Shot%202018-06-04%20at%2022.29.24.png)

-------------------------

### MS-Flow

TBD
