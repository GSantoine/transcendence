# transcendence - Web app with chat, channel groups, and real-time multiplayer game

## 15th project of my 42 cursus (final project of the common core)

The project involves creating a single page web application featuring an interactive Pong game and a matchmaking system. Client users can create accounts, log in to chat and play.


|    Project Name    |                                                                       ft_transcendence                                                                      |
| :----------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------: |
|    Description     |       A website that runs an online multiplayer pong, a real-time chat and a user management system                                       |
|    Technologies    |  <img alt="React" src="https://img.shields.io/badge/React-20232a.svg?logo=react&logoColor=%2361DAFB"> <img alt="Nest" src="https://img.shields.io/badge/nestjs-%23E0234E.svg?logo=nestjs&logoColor=white"> <img alt="Docker" src="https://img.shields.io/badge/docker-%230db7ed.svg?logo=docker&logoColor=white"> <img alt="PostgreSQL" src ="https://img.shields.io/badge/PostgreSQL-316192.svg?logo=postgresql&logoColor=white"> <img alt="Prisma" src="https://img.shields.io/badge/Prisma-3982CE?logo=Prisma&logoColor=white"> |

## Features 
- User's features include profile data, settings, friend lists, private chats, custom avatars, game stats, and match history.
- Authentication management is handled using the 42 API (OAuth2) and Google Authenticator for 2FA.
- Database management employs the Prisma ORM, connecting the server to a PostgreSQL database, ensuring password security and protection against injections via POST forms.
- The frontend built using React, on port __3333__.
- The Backend development utilizes NestJS, providing a project architecture and tools for creating a REST API to enable coherent and structured communication between systems via HTTP. On port __3000__.
- Group discussion channels management involves websockets programming, supporting both public and private channels (and channels protected by password).
- The website is responsive.
- The whole app is deployable using Docker.
- At least chrome and firefox are supported.


## Prerequisite

To run the project, you have to install __docker-compose and docker__. You need to rename "example.env" to ".env" and setup the file __.env with your credentials__ and __42 API credentials__.
```bash
  git clone https://github.com/GSantoine/transcendence.git
  cd transcendence
  mv example.env .env
```

Here you need to modify the .env file to configure it with your credentials :<br>
You have to put a password for the jwt secret and for the refresh jwt secret. You need also to put your __42 API credentials__, if you don't it won't work.
```bash
...
JWT_SECRET=""
JWT_REFRESH_SECRET=""
API_42_UID=""
API_42_PWD=""
...
```

## Usage
```bash
  make
```
When the containers are done building up and are running, you can access the application in your browser on the url "localhost:3000"

## Some visuals of the final project
The figma wireframe made by Tullia (thank you !)
![](https://github.com/trobert42/transcendence/blob/main/transcendence_figma.png)

Annnnnd the final look :
![](https://github.com/trobert42/transcendence/blob/main/transcendence_clip.gif)
