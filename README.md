## NYUSHer

![Swift Planner](https://img.shields.io/badge/iOS-Built-40aa00.svg?style=flat-square)
![Swift Planner](https://img.shields.io/badge/Android-Built-40aa00.svg?style=flat-square)
![NYUAPI](https://img.shields.io/badge/With-NYU%20API-ff6400.svg?style=flat-square)
![Code](https://img.shields.io/badge/Code%20With-<3-ff0000.svg?style=flat-square)

## What is NYUSHer

A HTML5 based cross-platform app which gathers every students / professors / stuff of one school into a centralized platform through .edu emails. NYU people repeat similar task everyday across multiple platforms such as weather app, wechat, facebook, calendar, OrgSync, and etc. We brings these scattered platform into one centralized app, including functionalities such as chatting, momenting, todo-dashboard, and calendar.

## Detailed infomation

Students can create sub-forms in categories and chat freely. Every message is kept for new come-ins, so students are exposed to every information in the campus. Also, the app supports multiple forms of message. Users can send not only bare text messages, but also voice, pictures, videos, stickers, voting poll, docs, .etc, publicly or privately, parallely getting statistics about how many people have read and how popular your messages are.
	Furthermore, users can decorate their own dashboard to get information instantly. They can put bus schedule, room vacancy, todo list onto the dashboard to make the day arranged.

## Motivation

It has alway been frustrating for me to switch between many website everyday to complete daily school tasks. I have observed and asked some of my friends and they are also experiencing the same problem, so this is a school-wide pain point. Also, our school does not have an online platform where everyone can post information. A campus craigslist-like website can help students spread their words faster.

## Comparison

Some of our app’s core functions may have an overlap with other apps that are dedicated to them. For example, chatting vs WeChat & Facebook; forum vs WeChat Moments & Facebook group posts; classroom assistance vs NYU Classes; personal information vs Albert. But as each of them is dedicated to certain functions, by combining them and focusing on life at NYU Shanghai, our app can organically co-exist with those apps and further help improve user experience at NYU Shanghai.

## Widgets

### Inspiration

As course registration is approaching, NYU students across all campuses are struggling to find what courses to take. Albert course search is slow and the students have to either find information about the professor on other website or ask their friends. Another issue is that all the mid-term review and final-review students submit are viewed by professors but not disclosed to other students. As a result, students cannot get fair information about a professor when registering.

### What it does
We are a course/instructor search platform for NYU students to find out the reputation of professors.
Better UI for seamless course search experience
Allow students to rate and comment their professors anonymously
We believe with more student review about professors, NYU students will benefit by enrolling in a class that actually suits them.

### How we built it
We utilized the NYU API (specifically Course Catalog API, Class Roster API, and Faculty API) to match professor names and NetID with classes they are teaching.
We used Python Flask and bmob.cn NoSQL for back-end development.
Deployed with Docker and Kubernetes engine for better control of server usage.
We bought NYU.wiki domain and our service is already deployed on Google App Engine and served by Global Server Load Balancing engine.

### Challenges we ran into
Since we cannot directly use the NYU API to select professors by course filter, we built up a python backend to do aggregation search. Students can either search professors by courses or search professors by their name. Also, we use python backend to gather related professors or courses for a better reference of course selection.
Mobile devices resolution fragmentation is a big problem for mobile web app designing. In order for better user experience, we use Semantic UI and flex layout to ensure the suitable display for every device. We chose Semantic UI from a number of VUE libraries such as Materialize and iView because of its rich components and elegant aesthetics.
Accomplishments that we're proud of
Our query speed is much faster than NYU Albert, which is the official course search engine. We implement NYU API to give students a better experience of understanding of professors, course selection, and career decision.
Both students and professors can use this platform to evaluate both courses and the teaching style of faculties. Although the rating is anonymous, the comment is not, so that it can be ensured that the comments on the Swift Planner are responsible for public use.

### What we learned
Use NoSQL to store simple nonrelational data
Use mature libraries such as iView, Materialize and Semantic UI to develop frontend systemically.
We use serverless backend service provided by Bmob (which is the same as Google Firebase or stdlib.com). So that we can just write python code on Cloud Functions rather than deploy it on a server. It is more stable so that we do not need to concern about the maintenance and stability of the server. We can leave more time on API / User Interface designing.

### What's next for Swift Planner
We plan to add more course information such as class time and location onto the search.
Then we can integrate a new course planner feature where students can easily just click a course and it will be mapped on a weekly calendar. Also, we need to add user system to prevent abusive use of rating and comment system.
Use natural language processing to filter out offensive slandering comments

## Programming Languages

- Front-end: HTML, CSS, JS
- Back-end: Python (Flask Library)
- Database: MySQL
- API: OrgSync, Google Calendar, Cryptowat.ch
- iOS Adaptation: Swift + HTML
- Android Adaptation: Kotlin (or Java) + HTML
- Internet Transmission Protocol: TCP with SSL Encrypted

## Meeting Schedule

Tuesdays: 18:30 - 22:30 (4hrs)
Thursday: 16:00 - 18:00 (2hrs)

## Team
Jack, Jerry, Masaki, Max
