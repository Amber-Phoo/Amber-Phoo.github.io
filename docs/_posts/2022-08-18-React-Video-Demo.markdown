---
layout: post
title:  "AD project React Code Video Demo"
date:   2022-08-18 18:28:34 +0800
categories: video demo
---

<h2>Code Structure</h2>
<h3>This React application is created using create-react-app command.</h3>
<p>At the high level below is the structure of the React app.</p>

![image](https://user-images.githubusercontent.com/100519215/185398745-cc01f90e-f88c-4cc9-8efb-c07b68b068b0.png)


## api
<p>This directory will have all methods which make calls to an API.</p>

![image](https://user-images.githubusercontent.com/100519215/185402500-df7ce799-2b05-4eac-bb4f-af73299e3934.png)


## components
<p>This directory consists all react UI components.</p>

![image](https://user-images.githubusercontent.com/100519215/185402686-31484ee5-63ae-4eaf-8b4b-64d046248c29.png)


## providers
<p>This directory contains all context API providers for react app.</p>

![image](https://user-images.githubusercontent.com/100519215/185402784-60096885-675c-4165-8a4f-842d0b4c1fd8.png)


## - reducers
<p>This directory has all reducers which help manages state via actions.</p>

![image](https://user-images.githubusercontent.com/100519215/185402840-c479dc7f-c99a-4614-992f-0d5b175e1872.png)

## routers
<p>This directory contains client site routing configuration file.</p>

![image](https://user-images.githubusercontent.com/100519215/185403033-bb5bd00c-ef10-4cfa-8e5a-60c13dedb2ea.png)

## styles
<p>This directory has all styles components such as 'css' , 'scss' and 'css in js'.</p>

 ![image](https://user-images.githubusercontent.com/100519215/185402932-5077813c-f392-4abb-8666-16dc80dd5cd9.png)

## utils
 <p>This directory contains utility function such as store and retrieve session. Last but not least AppSetting to easily configure api endpoint.</p>

![image](https://user-images.githubusercontent.com/100519215/185403637-f6022141-b703-4c6d-a547-814707c6d244.png)


##  _mock
<p>This directory contains mock data structure of App Model to make app work before actual data is passing down from api.</p>


<p>&nbsp;</p>

<p>&nbsp;</p>


<h2>Code Overview</h2>


## Index.js
<p>This file is main entry point of React app and which has child component called AppRouter.js</p>

![image](https://user-images.githubusercontent.com/100519215/185407241-072af988-529f-4be7-904d-da8f550ee22a.png)

## AppRouter.js
<p>The route of the application is configure in this file.</p>

![image](https://user-images.githubusercontent.com/100519215/185408254-bc260fe8-46b3-4b00-95f4-603488f40ce2.png)

<p>Authentication logic is implemented in this code.</p>

![image](https://user-images.githubusercontent.com/100519215/185408355-be5416cd-68e0-440d-b606-33dce928654d.png)

## eventReducer.js  
<p>Each UI component has their own state. Those states are declare in the respective reducer file. eventReducer is one of them which is used to manage states of event component.</p>

![image](https://user-images.githubusercontent.com/100519215/185410590-46ffc357-79cd-47b6-87bf-49dfb1f91c31.png)

## EventHome.js (Parent Component)
<p>1. EventHome is UI component for event. States of this UI component are initialized using userReducer hook.</p>

![image](https://user-images.githubusercontent.com/100519215/185412197-7c6c346f-d23d-47e0-9a19-13e92a7bb1d4.png)

<p>2. <b>useEffect</b> hook will be triggered before component mounted and after component dismounted.</p>
<p>That is the reason we put restful api call in this method.</p>

![image](https://user-images.githubusercontent.com/100519215/185413535-7d86b1ae-e664-4fdf-8a5c-2d098eb11c0a.png)

<p>3. Then we use Provider to pass down parent state to child components. So that parent and child component can use same state.</p>

![image](https://user-images.githubusercontent.com/100519215/185413034-ea30df89-71a7-480d-aeec-79e9817578df.png)

## MyCalendar.js (Child Component)
<p>1. Child component retrieve parent's state by using <b>useContext</b> hook.</p> 

![image](https://user-images.githubusercontent.com/100519215/185418359-2893085b-1f84-4762-8100-e4e2a662e867.png)

<p>2. As long as eventContext has eventList state, then child component will render.</p> 

![image](https://user-images.githubusercontent.com/100519215/185419001-321b7312-486b-4b3a-b63e-0fb3fee1adf9.png)

##  event-actions.js (Event Restful Service handler)
<p>All the event related restful services are implemented in here using axios library.</p> 

![image](https://user-images.githubusercontent.com/100519215/185419978-1f47cb4b-046c-485c-b2f1-9851556ceaf5.png)


<p>&nbsp;</p>

<p>&nbsp;</p>

## Libary Used in this project 

<h2><a href="https://axios-http.com/docs/intro" target="_blank">axios</a></h2>
<p>This library is used to call restful api service.</p>

<h2><a href="https://reactrouter.com/docs/en/v6/getting-started/overview" target="_blank">react router</a></h2>
<p>This library is used to make client site routing possible.</p>

<h2><a href="https://mui.com/" target="_blank">MUI</a></h2>
<p>This library is used as based UI library. It helps a lot in creating nice looking UI.</p>

<h2><a href="https://github.com/jquense/react-big-calendar" target="_blank">React Big Calendar</a></h2>
<p>This library is used to creaet Calendar View with event.</p>

#### Special thanks to above libaries for making this react application happen.



