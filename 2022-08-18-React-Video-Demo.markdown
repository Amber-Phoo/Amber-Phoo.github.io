---
layout: post
title:  "AD project React Code Video Demo"
date:   2022-08-18 18:28:34 +0800
categories: video demo
---

## React App features


### General
1. Register for new account
2. Login to app

### Study Groups / Chats

1. Study groups with chatting.
2. Able to send images/videos/files.
3. Able to view images/play videos in full screen by tapping on them from the chat screen.
4. Able to download files sent
5. Search for users to chat 1 to 1
6. Both light mode and dark mode available
7. Mobile responsive for small device
8. Autoscroll to last message when click on each chat list.
9. Display message send time based on current timestamp.

### Events
1. View all available events with Calendar View
2. Join events or View Discussion (already member of group) by clicking each event
3. Create new events based on Date and Time
4. Have Agenda View.

### Books
1. View books recommended based on interests & groups joined
2. Search for books with autocomplete feature
3. View books

### Profile
1. View current profile
2. Change profile photo by clicking upload photo (Drag and Drop supported)
3. Edit interests, email, display name
4. Change password
5. Logout


### Technical Challenges

#### React Hook
1. React hook is a bit tricky. If you don't handle api request properly using hook effect, you will get memory heat problem.
2. React hook is newly introduced feature, it takes a bit of time to understand and use it.

#### Client Site Routing
1. react-router-dom V6 is used for client site routing. take a bit of time to know how to use the library.

#### CORS issue
1. This issue always happen when server and client site are not in the same domain. So, server reject every request from client because of cors issue.
2. Able to solve by setting up Cors compitablity setting in backend code.

#### Styling issue
1. In order to support multi mode in chat style, style was created using sass instead of css. By using sass, eliminateed lots of duplicate code.

#### HTTPS issue
1. In order to send data over the internet, browser compains unless it is being sent over a HTTPS tunnel. So react is running behind a Nginx reverse proxy providing HTTPS support.
2. If react is running with HTTPS, it cant send data to JAVA backend as it was running without HTTPS. So now all the servers are behind Nginx reverse proxies.

<p>&nbsp;</p>

<p>&nbsp;</p>
