---
layout: post
title:  "Study Buddy (Capstone Project)"
date:   2023-02-13 18:28:34 +0800
categories: Projects
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

#### Auto Scroll  
1. Auto scroll chat history when there is new message especially image in React. When message is arrived, auto scroll will be triggered but image is still loading, and browser don't know exact height to be scrolled yet. 
2. So able to solve issue by adding auto scroll function inside onload event of image. 

#### Sate Management 
1. React UI state management. To maintain single source of truth between Parent and Child components. 

<p>&nbsp;</p>

<p>&nbsp;</p>

## Landing Page

![image](https://user-images.githubusercontent.com/100519215/218746449-7e55b59d-c8a7-4608-9fbe-798b978654eb.png)

## Event Page with Calendar View

![image](https://user-images.githubusercontent.com/100519215/218746702-1e313a00-cfab-401c-bb5f-bbcc92d24f58.png)

## Profile Page

![image](https://user-images.githubusercontent.com/100519215/218747268-d90703c9-7d23-4bdb-9bad-036e4b6cff49.png)

## Chat UI (Dark Mode)

![image](https://user-images.githubusercontent.com/100519215/218747612-5dc71645-76f8-4df6-931f-20e2fdb982f0.png)

## Chat UI (Light Mode)

![image](https://user-images.githubusercontent.com/100519215/218748000-ec2374dc-d822-491a-a228-59bc25265091.png)

## Gif Supported

![image](https://user-images.githubusercontent.com/100519215/218748124-04040b37-3236-48c5-abac-179c6b0940d1.png)

## Emonji Supported

![image](https://user-images.githubusercontent.com/100519215/218748370-68119d3e-6106-4e7c-9105-eb277f4298e0.png)

