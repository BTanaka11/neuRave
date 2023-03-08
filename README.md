# neuRave
This was an 8 person team project to build a music social media and event planning web app with a rave theme. The 4 pages of this app are Login/Home, Groups, Discover, and Profile. After an initial group planning phase, we split into pairs and each was assigned to 1 page. Myself (Ben Tanaka) and Christopher Leblanc were assigned to the **_Discover Page_**. I did the backend and contributed to the frontend. For a more detailed README covering the other 3 pages and the entire team, please see repo this was forked from.

## Tech Stack
<p align="left"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a><a href="https://www.postgresql.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a><a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a><a href="https://nodejs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a><a href="https://aws.amazon.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/> </a><a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a><a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a><a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a><a href="https://expressjs.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original-wordmark.svg" alt="express" width="40" height="40"/> </a><a href="https://axios-http.com/docs/intro" target="_blank" rel="noreferrer"> <img src="https://user-images.githubusercontent.com/37204126/222049084-4f80d4a6-17fe-42fd-857d-56d720372f3b.svg" alt="axios" width="40" height="40"/> </a><a href="https://jestjs.io" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/jestjsio/jestjsio-icon.svg" alt="jest" width="40" height="40"/> </a><a href="https://webpack.js.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/d00d0969292a6569d45b06d3f350f463a0107b0d/icons/webpack/webpack-original-wordmark.svg" alt="webpack" width="40" height="40"/> </a><a href="https://babeljs.io/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/babeljs/babeljs-icon.svg" alt="babel" width="40" height="40"/> </a></p>

## Code I Wrote Includes:
* [/server/routes/sg.js](/server/routes/sg.js)
* [/server/database/schema.sql](/server/database/schema.sql)
* [/server/database/postgresDB.js](/server/database/postgresDB.js)
* [/server/database/controllers/getGroupOrCreateNew.js](/server/database/controllers/getGroupOrCreateNew.js)

## Code I Contributed To Includes:
* [/client/src/pages/DiscoverPage.jsx](/client/src/pages/DiscoverPage.jsx)
* [/client/src/pages/EventCard.jsx](/client/src/pages/EventCard.jsx)
* [/client/src/pages/SearchForm.jsx](/client/src/pages/SearchForm.jsx)
* [/client/webpack.config.js](/client/webpack.config.js)
* [/server/index.js](/server/index.js)

## Discover Page
Allows users to search for upcoming music events from an external Seatgeek API and create groups for events or join existing groups. This page is the main route by which external data enters the app's database. The only other one is Login/Home page which brings in Spotify account details. Search results are limited to 50 events at a time and sorted by the soonest upcoming event date. Each card can be clicked to redirect the user to seat geek’s website for that concert in order to purchase tickets. Each card also has the ability to join the events group or create a group if one has not been made. If both of those choices are not applicable due to the user being in that group already the button will dynamically change to show that status.

<!--- <img src="walkThroughGifs/Discover_Page.gif"/> --->
https://user-images.githubusercontent.com/37204126/223301349-ab214f01-0ab3-4035-a603-3533283207f0.mp4

## Database
The PostgreSQL database was deployed as an EC2 micro instance remotely accessible by the team. Here is the schema and what some of the data looked like.

https://user-images.githubusercontent.com/37204126/223301520-f6724939-62ce-4276-a7bf-8cd617232f27.mp4

<!--- 
## Tech Stack I Used
### Front End
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Styled Components](https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=white)
![Zustand](https://img.shields.io/badge/-Zustand-red)

### Back End
![Postgres](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Express](https://img.shields.io/badge/-Express-DCDCDC?logo=express&logoColor=black&style=for-the-badge)
![Node](https://img.shields.io/badge/-Node-9ACD32?logo=node.js&logoColor=white&style=for-the-badge)
![Axios](https://img.shields.io/badge/-Axios-671ddf?logo=axios&logoColor=black&style=for-the-badge)
![Socket.io](https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&badgeColor=010101)
--->
