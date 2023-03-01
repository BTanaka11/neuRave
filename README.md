# neuRave
This was an 8 person team project to build a music social media and event planning web app with a rave theme. The 4 pages of this app are Login/Home, Groups, Discover, and Profile. After an initial group planning phase, pairs of team members were assigned to each page. I (Ben Tanaka) and Christopher Leblanc were assigned to the **_Discover Page_**, which  For a more detailed README covering the other 3 pages and the entire team, please see repo this was forked from.

## Code I (Ben Tanaka) Wrote
* [/server/routes/sg.js](/server/routes/sg.js)
* [/server/database/schema.sql](/server/database/schema.sql)
* [/server/database/postgresDB.js](/server/database/postgresDB.js)
* [/server/database/controllers/getGroupOrCreateNew.js](/server/database/controllers/getGroupOrCreateNew.js)

## Code I Significantly Contributed To
* [/client/src/pages/DiscoverPage.jsx](/client/src/pages/DiscoverPage.jsx)
* [/client/src/pages/EventCard.jsx](/client/src/pages/EventCard.jsx)
* [/client/src/pages/SearchForm.jsx](/client/src/pages/SearchForm.jsx)
* [/client/webpack.config.js](/client/webpack.config.js)
* [/server/index.js](/server/index.js)

## Discover Page
Allows users to search for upcoming music events from an external Seatgeek API and create groups for events or join existing groups. This page is the main route by which external data enters the app's database. The only other one is Login/Home page which brings in Spotify account details. Search results are limited to 50 events at a time and sorted by the soonest upcoming event date. Each card can be clicked to redirect the user to seat geek’s website for that concert in order to purchase tickets. Each card also has the ability to join the events group or create a group if one has not been made. If both of those choices are not applicable due to the user being in that group already the button will dynamically change to show that status.

<img src="walkThroughGifs/Discover_Page.gif"/>

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
