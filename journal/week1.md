# Week 1 — App Containerization

Week 1 continued to build upon Week 0, specifically focusing on further navigation of the CDE, utilizing containers (Docker) and Docker Compose, and build out of the backend and frontend apps. 

Homework Challenge: **To Be Completed**

[Interest: Push and tag a image to DockerHub and/or Launch an EC2 instance that has docker installed, and pull a container to demonstrate you can run your own docker processes]

I encountered a few challenges during the completion of the assignments this week; even despite my constant rewinding and fast fowarding of material. I have found that a 30 minute video, often does not only take 30 minutes to complete (e.g. taking my time enables me to retain and understand the content in multiples). Even so, all issues encountered were able to be resolved with time. Utilizing the "Inspect" feature on the webpage (noted in the "Before You Ask for Help" video) became my lifesaver during my research.

1) Blank Home Page - this error was deceptively simple, when I inspected the page I found a CORS issue. Thinking back to the instructional video, I remember this can be caused by incorrect ports. I then found a typo in env.example (however, ultimately learned that this isn't the actual code that would solve the issue). Finally, I took a look at my ports to realize that I simply had not unlocked them. 

![Week1_BlankHomePageIssue](https://user-images.githubusercontent.com/125226013/221755124-c772f773-f611-4472-8688-f7ef7492e154.png)
![Week1_BHPResearch](https://user-images.githubusercontent.com/125226013/221755144-18670217-a386-4cc8-8e49-1aa18c3e0ce1.png)
![Week1_EnvBackEnd](https://user-images.githubusercontent.com/125226013/221755161-97309531-3d82-45ea-b376-39ba41912ace.png)
![Week1_BHPResolution](https://user-images.githubusercontent.com/125226013/221755195-cc08ff62-568b-4ddb-b270-3e1af1c10d58.png)

2) Indentation error - this error was the post clear cut error I have seen to date. It clearly called out line 71 in the backend python file that was the issue. One little space! Cleared space and proceeded. 

![Week1_IndendationError](https://user-images.githubusercontent.com/125226013/221755375-9968a1a0-1d63-48cf-b7b4-8b9d21f9357b.png)
![Week1_IndendationError2](https://user-images.githubusercontent.com/125226013/221755415-45f90782-ed06-4329-b778-e80b58fc26de.png)

3) Blank Page Full - I ran into another blank page after adjusting the Notifications CSS/JS. Immediately ran inspect on the page and began to research the first line " NotificationsFeedPage.css". I then looked into the front end pages and realized when I had copied the pages for Notifications, I inadvertently retained "copy". I updated, refreshed, and success!

![Week1_BlankPageFull](https://user-images.githubusercontent.com/125226013/221755529-295de598-2d28-4904-a638-2898e737fa26.png)
![Week1_BPFResolution](https://user-images.githubusercontent.com/125226013/221755567-84cec69c-4d41-4a1c-be47-0e07b0e37820.png)
![Week1_BPFResolution2](https://user-images.githubusercontent.com/125226013/221755581-996f3c9d-8eb7-40b5-9efd-781c0088da29.png)

4) Finally, a bit of an oddity. I notice that sometimes when I composed up, I would error out. I noted that there were some gaps between where volume/db was placed in the video vs the pasted notes, so initially I tried to change the location in the code, and surprisingly, it ran. At another point, I shut down my workspace and restarted, and the same  issue arose. What I believe may actually be occuring is the need to do a full compose down and a full compose up. Once I completed this ( full compose up/down) the second time around, even after changing the location again (sole compose up didn't work initially), I was able to run the full compose file with no errors). 

![Week1_VolumesDBLocationIssue](https://user-images.githubusercontent.com/125226013/221756638-43782361-61a3-4b24-a315-68247b1df772.png)

Great week! 
