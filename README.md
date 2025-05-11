# Host Your Own Help Desk!
Many of us often serve as the go-to tech support for our friends and family. But when they need help from a true IT professional, it's time to formalize the process with a proper ticket. In this lab, I'll show how to self-host your own help desk using ticketing software that ensures all support requests are submitted through an official system.
### Why is it important to practice a ticketing system as an inspiring IT professional?
Practicing a ticketing system is essential for an aspiring IT professional because it helps you develop key skills that are critical in nearly all real-world IT environments:
  - Organizational skills: You learn how to track, prioritize, and manage multiple issues efficiently.
  - Communication: It teaches you how to document problems clearly and professionally for both technical teams and non-technical users.
  - Accountability and transparency: Every action is logged, which builds a habit of thoroughness and responsibility.
  - Collaboration: Ticketing systems make it easier to work with other IT staff, escalate issues, and share updates.
  - Industry readiness: Most IT departments use some form of ticketing software (like ServiceNow, Jira, or Zendesk), so hands-on practice gives you a major advantage when entering the workforce.
### What is Linode?
Linode is a cloud computing platform that offers Linux virtual machines, a Cloud Manager for managing infrastructure, and various tools for building and deploying applications. It's known for its simple, affordable, and accessible approach to cloud computing, making it appealing for developers and businesses of all sizes. Linode is now owned by Akamai. We will be using Linode to host our ticketing system. 
## Lab Walkthrough:
1. Go to [Linode.com](https://login.linode.com/login) to create an account
2. After creating an account, click on "Create Linode"

![Image](https://github.com/user-attachments/assets/81eb9c8c-7e59-40bc-8a4c-eff79e7882b2)

3. Click on "Marketplace" and type in the search bar, "Peppermint." This is the program we are going to use to host our ticketing system.

![Image](https://github.com/user-attachments/assets/81abb59c-86ff-44e1-bedb-4e9c6a104f43)

4. Pick a plan for the Linode. To get the cheapest option, click on "Shared CPU" and select the first option. As you can see, it is only $5 a month to host this ticketing system.

![Image](https://github.com/user-attachments/assets/55f7ba32-2ec0-4233-aa3e-69b714cf1ae2)

5. Next, label or name the Linode. I have named it "doyouhaveaticket."

![Image](https://github.com/user-attachments/assets/30beb242-bec8-45d1-822b-ead22d753167)

6. Create a Root password. Make sure you do not forget this!
7. After selecting a plan, making a password, and naming the Linode, ignore everything else, scroll down, and select "Create Linode."

![Image](https://github.com/user-attachments/assets/fbf1125e-5547-4a23-8795-08a279307851)

7. The Linode will start running. Click on "Launch LISH console" on the top right corner of the screen.

![Image](https://github.com/user-attachments/assets/bbec539f-c20b-4669-b669-ac8230696efd)

8. Wait till the download is complete. You will know when the download is complete when you are prompted for your Login and Password.
9. Once you are prompted, next to **Login** type in *root*
10. You will be prompted to type a password. Type in the root password you just created a couple of minutes ago.
11. After logging in, type in the console *docker ps*. This will tell you which tcp port is being used.

![Image](https://github.com/user-attachments/assets/fb2eae60-cd88-4024-adab-7f5c1fa92d77)

The TCP port that I am using is 3000. Everyone is different so please make sure which one is yours and write it down. 

![Image](https://github.com/user-attachments/assets/f319a15d-b904-4d48-ae7a-3317b2e11008)

12. We no longer need the LISH console so you can close it out.
13. Click on the *Network* tab and find the column that says *Reverse DNS*.
14. Copy the Reverse DNS address.

![Image](https://github.com/user-attachments/assets/d3550522-a43c-4b53-8d37-1248762d27e3)

15. Paste the *Reverse DNS* address into another tab in your web browser.
16. Do not press Enter yet, paste the address, type the colon punctuation mark (:) after the address, and then press Enter.
17. After doing that, you should see the Peppermint login page.

![Image](https://github.com/user-attachments/assets/56c9bc81-f767-474a-9bc3-b51c6b595f74)

18. The email address is *admin@admin.com* and the password is *1234*. <br>

And that is it! You have now successfully created your own ticketing system.

![Image](https://github.com/user-attachments/assets/a94e6f85-1316-4d4b-bdcb-75a24b1efbc8)
