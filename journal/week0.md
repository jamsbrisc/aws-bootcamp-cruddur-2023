# Week 0 — Billing and Architecture

This week encompassed multiple topics including architecture, cloud services, the Well-Architected Framework, budgets and billing, utilizing the CLI/scripting, and IAM. I ran into a few issues with this week's required assignments; however, the homework challenge went smoothly.
For the challenge I added MFA and created an IAM user. I also created the conceptual and logical diagram - these were both recreations to become acquiainted with Lucid Charts and do not significantly differ from the provided examples. Please see links:

**Conceptual**:

https://lucid.app/lucidchart/6406ecd5-d5b8-4294-b47a-0f74ec0fe2fa/edit?viewport_loc=-984%2C-828%2C2900%2C1265%2C0_0&invitationId=inv_2ac056d6-7ff2-4bdc-9fcf-6dab8f5746c9

**Logical**

https://lucid.app/lucidchart/7ec768cf-50fd-4ae2-a7d4-75094719e834/edit?viewport_loc=-38%2C-336%2C1933%2C844%2C0_0&invitationId=inv_8ef8c293-d9a1-4309-92cc-b95da1f7b252


**MFA**

![Week0_MFA_IAM](https://user-images.githubusercontent.com/125226013/220427590-569d30da-7a7f-4813-be8c-2c2d76d9f141.png)

Regarding issues that I encountered: 

1) I initially couldn't see Budget in my IAM user to confirm the CLI budget. I had to enable IAM billing in the root account and then attach a billing policy to the IAM user. Following the root user adjustments, budgets populated in the IAM.  
2) When following along in the CLI video - I kept running into an error with the budget json -- I cleared and ran, cleared and ran and checked formulas to no avail. I took a break, and then returned to check formulas once again and behold! I was missing a "/" on the path for notifications-with-subscribers.


![Week0_IssueGitPod](https://user-images.githubusercontent.com/125226013/220479657-4a4b4766-5940-4167-b5a2-23e562dc11fc.png)

3) Within the pricing video instructions, I found that my AWS account currently did not list "Billing" as a metric. I ended up going directly to the billing section under alerts. Once clicked, the subsequent screen was similar to the example provided by Chirag (i.e. displaying a similar "Specify metric and conditions" and Namespace "AWS/Billing"). I was also able to specify the dollar amount threshold of $10 and create the noted alerts that shows in "All Alerts".

![Week0_Metrics Issue ](https://user-images.githubusercontent.com/125226013/220480201-2898d4ff-ee81-4fcd-994f-4f4e4b88450e.png)


![Week0_Billing Alert](https://user-images.githubusercontent.com/125226013/220480663-f93fb19a-1c21-4833-a566-f8a05b11147d.png)

4) Finally - not as much of an issue, but a curiousity. I didn't have VSC so I ended up downloading the toold so I could edit and save the svg. I also wanted to to see if the xml was indeed the trigger to get the Momento image to work in Lucid charts. I ended up editing the code purely adding the xml (w/ no other adjustments) and was unable to generate the image (still received the checkerboard). I then proceeded to edit the code and save according to the suggestions (1 at a time) to find that the culprit was Fill="currentColor". In my momento.svg version I retained all the original code with the exception of fill-current color and the image populated successfully. It did appear a bit pixelated - not sure if removing the other code (width/height) would correct, but that will be an item to investiagte at a later time when I am more familiar. 

![Week0_Lucidsvg](https://user-images.githubusercontent.com/125226013/220481719-7bad7708-4d12-4e68-b5b0-8519b0d97909.png)

Overall - a successful week. Eager for Week 1!
