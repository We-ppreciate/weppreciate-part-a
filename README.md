# T3A2-A Katie Lock and Nate Picone

## You work hard. We'ppreciate you. 

### A full stack MERN application

## R1 Purpose

A leader in the Fast Moving Consumer Goods industry approached us with a problem.

They have a monthly employee reward and recognition program for a key business unit, Business Services. Anyone in the business can nominate anyone in Business Services. They want to expand the program so that anyone from the wider business can be nominated, but have some issues they want to overcome first.

### The problem

After a requirements discussion with the client, and some analysis of the existing system, we aligned with the client that:

- Completing a nomination through a Microsoft Form is not easy, it lacks an engaging experience, and that a custom web interface is preferable;
- Finding the location of the Microsoft Forms is difficult, and a linkable domain name would be helpful;
- The monthly process of extracting the nominations from Microsoft Excel, preparing the list for review, then manually building PowerPoint slides for presentation and sharing the data with relevant parties could use some improvement;
- The business has a complicated structure of employees and vendor partner workers, who are also eligible for awards, and providing the nomination and award winners' data to the vendor partners has been manual and prone to human error. A method of giving the vendor partners access to the data would be helpful;
- Nomination and award recipients have no persistent record of the nomination or award, which creates a feeling that the celebration is fleeting, and a method for recipients to be able to keep the details of the award would be helpful for the employee's satisfaction, and for their development and performance review discussions;
- Likewise, those who submit nominations have no record of having done so, creating unease around whether their nomination was successful and leaving no way of nominators checking who they have nominated in the past;
- There is no formalised way of expressing and sharing thanks to an individual for actions that are appreciated but not substantial enough for an award nomination;

> [!NOTE]
> Viewable on [We'ppreciate's Notion site - Product Requirements Document](https://weppreciate.notion.site/Product-Requirements-Document-1a4fc83d4ca94759987db15e73e52171?pvs=4)

### The reason

Celebrating the success of people within business is important for engagement, which can translate to higher employee retention, and renewed efforts of those who have been recognised, as well as within their peers.

According to a 2019 [Deloitte study](https://www2.deloitte.com/content/dam/Deloitte/us/Documents/about-deloitte/us-about-deloitte-the-practical-magic-of-thank-you-june-2019.pdf):

- 68% of respondent prefer a non-financial reward, such as recognition;
- 40% of respondents like their success to be the reason they are recognised (46% of male respondents; 34% of female respondents).

> ...… one study found employees receiving small rewards and thanks were eight times more engaged than those receiving compensation and bonus increases once a year.

[Deloitte](https://www2.deloitte.com/content/dam/Deloitte/us/Documents/about-deloitte/us-about-deloitte-the-practical-magic-of-thank-you-june-2019.pdf), p23

> “I want the recognition to match the level of work. Small things don’t need to be shared with the broader team. Big things should be recognized to higher levels.“

[Deloitte](https://www2.deloitte.com/content/dam/Deloitte/us/Documents/about-deloitte/us-about-deloitte-the-practical-magic-of-thank-you-june-2019.pdf), p21

> [!NOTE]
> Viewable on [We'ppreciate's Notion site - Product Requirements Document](https://weppreciate.notion.site/Product-Requirements-Document-1a4fc83d4ca94759987db15e73e52171?pvs=4)

### The proposal

We will build a full stack MERN web application, as a pilot, allowing for the current award system structure (anyone from the business can nominate anyone in Business Services), with the ability for the client to easily upscale for future, full-business expansion.

The web app will offer services to cater to the user stories, identified below. In summary, the main groups of users are:

1. Anyone with an email address with one of the business' domains can access the site, to view Business Services people’s profiles, to nominate, or to send a form of instant thanks.
1. Anyone within Business Services can be nominated or receive a form of instant thanks. This group will:
	- have a customisable profile,
	- have a feed of others' nominations, awards and instant thanks to view and interact with,
	- have a persistent record of nominations, awards and instant thanks received,
	- also be able to nominate others within Business Services.
1. Senior Managers will be able to review, group, reject, or progress nominations to awards.
1. Line Managers will have a rolled-up view of cards, nominations and awards received by thier team members.
1. Administrators will be able to have wide data viewing, updating, deleting, and creation abilities, including to change user details, add and remove profiles, add and remove nominations, and and remove authorisation.

Were this project to be implemented, the client would be encouraged to run promotional activity for implementation and staff engagement. We suggest identifying stakeholders, and a group of people for User Acceptance Testing and user experience feedback.

> [!NOTE]
> Viewable on [We'ppreciate's Notion site - Product Requirements Document](https://weppreciate.notion.site/Product-Requirements-Document-1a4fc83d4ca94759987db15e73e52171?pvs=4)

## R4 User Stories

### The user story format

We used [Atlassian's](https://www.atlassian.com/agile/project-management/user-stories) format of: **As a \[persona\], I \[want to\], \[so that\].**

Breaking this down:

- **"As a \[persona\]":** Who are we building this for? We’re not just after a job title, we’re after the persona of the person. Max. Our team should have a shared understanding of who Max is. We’ve hopefully interviewed plenty of Max’s. We understand how that person works, how they think and what they feel. We have empathy for Max.
- **“Want to”:** Here we’re describing their intent — not the features they use. What is it they’re actually trying to achieve? This statement should be implementation free — if you’re describing any part of the UI and not what the user goal is you're missing the point.
- **“So that”:** how does their immediate desire to do something this fit into their bigger picture? What’s the overall benefit they’re trying to achieve? What is the big problem that needs solving?

> [!NOTE]
> Viewable on [We'ppreciate's Notion site - User Stories](https://weppreciate.notion.site/User-Stories-b41b48c301e34f498625f1c724df3976)

### The personas

To give our user stories the true “persona” effect, here are some defined personas that represent a variety of users/stakeholders within the organisation:

| **Name**   | **Role within organisation**                       | **User role in application** |
| ------ | ---------------------------------------------- | ------------------------ |
| Nate   | Individual contributor, Business Services team | Employee (Full access)   |
| Ed     | Line manager, Business Services team           | Line Manager             |
| Katie  | HR Business Partner, Business Services team    | Administrator            |
| Naomi  | Individual contributor, Sales team             | Employee (Basic access)  |
| Hannah | Senior manager, Business Services team         | Senior Manager           |

Some user stories will apply to multiple or all personas.

> [!NOTE]
> Viewable on [We'ppreciate's Notion site - User Stories](https://weppreciate.notion.site/User-Stories-b41b48c301e34f498625f1c724df3976)

### The user stories

The core functionality of the application form the *acceptable criteria* in the user stories

![Screenshot of User Stories from Notion collaborative space](./resources/user-stories.jpg)

> [!NOTE]
> Viewable on [We'ppreciate's Notion site - User Stories](https://weppreciate.notion.site/User-Stories-b41b48c301e34f498625f1c724df3976)

### The Stack

We intend to solve these issues with a full stack MERN web application, harnessing:

#### Front end

[ReactJS](https://react.dev/)

[Javascript](https://www.javascript.com/)

[HTML5](https://developer.mozilla.org/en-US/docs/Glossary/HTML5)

[SCSS](https://sass-lang.com/)

[CSS3](https://developer.mozilla.org/en-US/docs/Web/CSS)

==any styling framework?==

#### Database

[MongoDB (Atlas platform)](https://www.mongodb.com/)

#### Object Document Mapping

[Mongoose](https://mongoosejs.com/docs/)

#### Back end

[Node.js](https://nodejs.org/en/)

[ExpressJS](https://expressjs.com/)

#### Package Management

[npm](https://www.npmjs.com/)

#### Testing

Currently evaluating between:

[Jest](https://jestjs.io/)

[msjws](https://mswjs.io/)

[Cypress](https://www.cypress.io/)

#### Diagramming

[draw.io](http://draw.io/)

#### Project Management

[Notion](http://notion.so)

#### DevOps

[Visual Studio Code](https://code.visualstudio.com/)

[Git](https://git-scm.com/doc)

[GitHub](https://github.com/)

#### Hosting

[Netlify](https://www.netlify.com/) - Front end hosting

[Heroku](https://dashboard.heroku.com/) - Back end hosting

#### Resource File Storage

[Google Drive](https://www.google.com/intl/en_au/drive/)

#### Design applications and services

[Figma](https://www.figma.com/)

[Affinity Designer](https://affinity.serif.com/en-gb/designer/)

> [!NOTE]
> Viewable on [We'ppreciate's Notion site - Product Requirements Document](https://weppreciate.notion.site/Product-Requirements-Document-1a4fc83d4ca94759987db15e73e52171?pvs=4)

## R2 - Dataflow

### Context Diagram (Overview of the system)

![Dataflow Context Diagram, showing a high level view of the system](./resources/dfd-context-v2.png)

### Dataflow Diagram

![Dataflow detailed Diagram, showing processes within the system](./resources/data-flow-diagram-v5.png)

> [!NOTE]
> Viewable on [We'ppreciate's Notion site - Dataflow Diagram](https://weppreciate.notion.site/Data-Flow-Diagram-47398d8544d94a65a338526915426a19?pvs=4)


## R3 - Application Architecture Diagram

![Image of the We'ppreciate Application Architecture Diagram, showing high level front end layer, back end layer, data layer, and database layer](./resources/application-architecture-document-v1.png)

> [!NOTE]
> Viewable on [We'ppreciate's Notion site - Application Architecture Diagram](https://weppreciate.notion.site/Application-Architecture-Diagram-51b1afe2e0a4482192db82302ac318b4?pvs=4)

## R5 - Wireframes


## R6 - Project Management

We split our project into 6x 1-week sprints, starting from 0th week.

> [!NOTE]
> Project Management documents are viewable on the below links. Note that as they are working documents, the live view may differ from the images below
>
>[We'ppreciate's Notion site - Sprints](https://weppreciate.notion.site/096aac0b89cd4d4ba7fcd0b02ce6187a?v=b9b2dde3fc2e4b53b59e3509f8c3d2b2&pvs=4)
>
>[We'ppreciate's Notion site - Tasks](https://weppreciate.notion.site/75b89fa68e894f5f954787c5eeef489f?v=989fd6fd0ad146e4af4e6ada44b70641&pvs=4)
>
>[We'ppreciate's Notion site - Projects](https://weppreciate.notion.site/fd3c53db9a1f4e27b59dcc063b46864a?v=41b6032216174cf59edfa04a8e317941&pvs=4)
>
>[We'ppreciate's Notion site - Meetings](https://weppreciate.notion.site/33e465ae7b2c4bdf9a261acbbf5167e0?v=00a1f910091e4b5c98a984ca396519f6&pvs=4)
>
>[We'ppreciate's Notion site - Documents](https://weppreciate.notion.site/59318e1ab6b840efbb38de4eb82117ec?v=c5f3f0c8a680426482b9cb31b7ec58ce&pvs=4)
>
>[We'ppreciate's Notion site - Wireframes](https://weppreciate.notion.site/Wireframes-85bba971e91a4a6380b062e88355c931?pvs=4)

## Project boards at end Sprint 0

### Sprint board wk0

![image of the sprint board, end week 0](./resources/notion-screenshots/end-wk-0/sprint-board-end-sprint-0.jpg)

### Project Board wk0

![image of the project board, end week 0](./resources/notion-screenshots/end-wk-0/projects-end-sprint-0.jpg)


### Task board, by project wk0

![image of the task board by project, end week 0](./resources/notion-screenshots/end-wk-0/task-by-project-end-sprint-0.jpg)

### Task Timeline wk0

![image of the task board timeline, end week 0](./resources/notion-screenshots/end-wk-0/task-timeline-end-sprint-0-a.jpg)

### Documents list wk0

![image of the documents board, end week 0](./resources/notion-screenshots/end-wk-0/docs-end-sprint-0.jpg)

### Meetings wk0

![image of the weekly meeting minutes, end week 0](./resources/notion-screenshots/end-wk-0/team-weekly-sprint-0.jpg)

![image of the standup meeting minutes, end week 0](./resources/notion-screenshots/end-wk-0/sunday-standup-wk-0.jpg)

## Project boards at end Sprint 1

### Sprint board wk1

![image of the sprint board, end week 1](./resources/notion-screenshots/end-wk-1/sprint-kanban-end-of-sprint-1.jpg)

### Project Board wk1

![image of the project board, end week 1](./resources/notion-screenshots/end-wk-1/project-end-sprint-1.jpg)


### Task board, by project wk1

![image of the task board by project, end week 1](./resources/notion-screenshots/end-wk-1/task-by-project-end-wk-1.jpg)

### Task Timeline wk1

![image of the task board timeline, end week 1](./resources/notion-screenshots/end-wk-1/task-timeline-end-sprint-1.jpg)

### Documents list wk1

![image of the documents board, end week 1](./resources/notion-screenshots/end-wk-1/docs-end-sprint-1.jpg)

### Meetings wk1

![image of the standup minutes 26th Nov, end week 1](./resources/notion-screenshots/end-wk-1/stand-up-sprint-1.jpg)

![image of the standup meeting minutes 21st Nov, end week 1](./resources/notion-screenshots/end-wk-1/standup-21-Nov-wk1.jpg)
