### **LogBook** 

This logbook is part of Cyber ​​Security and Data Protection (IT00AK39-3002) course.

02.11.2024 2 hours Listened the first lecture. GitHub repo done and logbook link send.

06.11.2024 3 hours Module 1: Introduction to Cybersecurity and Module 2: Attacks, Concepts and Techniques done.

07.11.2024 2 hours Module 3: Protecting the Organizarion done.

08.11.2024 2 hours Module 4: Protecting the Organization done.

09.11.2024 3 hours Module 5: Will Your Future Be in Cybersecurity? and Course Final Exam done. I created account and logged in PortSwigger.

13.11.2024 5 hours SQL injection 1/3 of the labs done.

14.11.2024 2 hours SQL injection 2/3 of the labs done.

16.11.2024 5 hours Couple of SQL injection labs and Authentication 1/3 of the labs done.

17.11.2024 8 hours All Access Control labs done. I tried the challenging labs one last time, but the intruder attacks took so long that I gave up and I returned PortSwigger assignment to ItsLearning.

19.11.2024 2 hours Downloaded Docker and I watched to a video (16 minutes) about it. I also watched 11.11 lecture Starting the project. I followed the teacher's guide and created booking_system_structure.sql.

20.11.2024 2 hours I rewatched 11.11 lecture and installed ZAP. I also created the necessary files in VS Code and added to this GitHub repo. I did my first security test with ZAP. The user registry worked in SQL but not in the browser.

23.11.2024 8 hours I read the material again and copied all the codes into VSCODE. I tested several times adding the user using SQL and http://localhost. Both ways worked. Also tested curl -x POST method on GitBash. Tested several times ZAP and Google Developer Tools that everything works, because the text Administrator and my own changes to the username to e-mail give a lot of errors. After all the changes, everything worked. First-register-test-23-11-24 and First-test-set were performed before adding CSS. After adding I performed second-register-test-23-11-24 and second-test-set.

24.11.2024 2 hours I was in a Teams meeting with a schoolmate who had asked for help several times on Itslearning and was having trouble with a Phase 1 task. I helped him to copy the codes from the teacher's GitHub and complete the task according to the instructions. I also helped him to use GitHub because he was not very familiar with coding and GitHub.

30.11.2024 4 hours I watched 18.11 lecture and made same the changes as in lecture. Everything worked. I did two attack in ZAP and I genereted "index-login-registreration-301124-Test-1.md report". I watched to a video about Alerts (15 minutes), made the same changes as shown in the video related to middleware functions for setting security headers globally, and conducted several attacks in ZAP. After changes and attacks I genereted "Fixed-Alerts-1.12.2024.md" report. I watched to a video about Adding a logging (16 minutes). I created login_log TABLE and made same changes as teacher in the video but I got error "Invalid email or password". I returned the link to my github repository to Itslearning.

1.12.2024 2 hours I helped my school mate with Phase 2 task. I also tried to understand why I was getting error "Invalid email or password" and why the logs didn't save to the table.

2.12.2024 2 hours I continued to work on the code. I notice that const = [, storedUsername, storedPasswordHash, userUUID] = user; needs a comma in the first spot. After making that small change, everything worked well. I took the ZAP test afterward and I named that test "Added-A-Logging-2-12-2024.md". After that, I took the second test with .HAR and named that test "Second-test-after-adding-a-logging-2-12-2024.md". I noticed that there are difference between tests: The second test has line User Agent Fuzzer | Informational | 24 |.

3.12.2024 1 hour I helped the same schoolmate with Phase 2 in a Teams meeting to get his system up and running.

8.12.2024 2 hours I did task Phase 3 and returned it Itslearning. I added cookies and indexPage with new options (log out, add a new resource and add a new reservation). I also added new files from the teacher's git hub. Everything worked well when I tested add a new resource and a reservation as a admin or reserver. I tested it under 15 year old and over 15 year old user. I took 2 Zap report. Second with .Har-file and it got 2 alerts more than other report. It got alert about loosely scoped cookie and user agent fuzzer.

12.12.2024 2 hours I forgot to answer the previous task "The 5 most important points -> Tell in each point", so I did that. I named file SecurityCheck.md. The task wasn't easy and I had to use AI and Google searches with it. I learned more about vulnerabilities and security with booking systems like this. During the whole process, I had looked at the website and the code, that something was rotten here, but now the answer came that there were problems.

13.12.2024  2 hours I did Phase 4. I downloaded .zip and did all the addings with AI (terms.html, privacynotice.html and needed code parts to other codes). I answered the questions to consent_privacy.md file. I tested how well navigation between pages works and it was successful. The final phase has great screenshot of all pages. After changes, it is possible to check privacy policy before registering and logging in. After logging in, user can check her/his account page, terms of service and privacy policy. 

15.12.2024 2 hours I wrote the final phase.

I have worked 63 hours.

# The booking system
1. Create a database
    1. Install Docker: https://www.docker.com/
    2. Load the postgres image: docker pull postgres
    3. Create a container: docker run --name new_booking_system_database -e POSTGRES_PASSWORD=Secret1234! -d -p 5432:5432 postgres
    4. Connect to the database: docker exec -it new_booking_system_database psql -U postgres -d postgres
    5. Copy the file booking_system_structure.sql to the clipboard.
    6. Paste the file into the psql terminal
2. Run the command: deno run --allow-net --allow-env --allow-read --watch app.js

# Pages
0. http://localhost:8000 --> GET
1. http://localhost:8000/register --> GET and POST
2. http://localhost:8000/login --> GET and POST
3. http://localhost:8000/logout --> GET
4. http://localhost:8000/resources --> GET and POST
5. http://localhost:8000/reservation --> GET and POST
6. http://localhost:8000/resourcesList --> GET
7. http://localhost:8000/terms --> GET
8. http://localhost:8000/privacynotice --> GET
9. http://localhost:8000/account --> GET
10. http://localhost:8000/accountInfo --> GET

