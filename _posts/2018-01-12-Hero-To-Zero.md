---
title:  "From Hero to Zero: My Path to OSCP"
date:   2019-01-12
categories: posts
tags: [posts]
excerpt: "How I went from a naive college kid who did not know there was more than one distribution of Linux, to an OSCP in less than a year- and debunking the stigma of OSCP."
---
Introduction:
---
"Wait, Kali Linux is the same thing as Linux?" I can still recall the sheer embarrassment hitting my face. This was me, a 20 year old novice in August of 2017, at one of my school's Cyber Defense Club meetings. In the world of information security, where there are ground breaking developments everyday- I had just came to the realization there in fact is more than one distribution of Linux. In this moment I realized I was being left in the dust by my peers, and a change was needed. This is the first of many events that propelled me to the elation I felt when I read the words "...allow us to be the first to congratulate you on your OSCP certification" in an email from Offensive Security. How did that befuddled young man obtain one of the industry's most elite certifications? In this blog post, I am going to elaborate a little on my background at the time I passed my OSCP in September. Provided also: My pathway to the cert, various resources I found useful, and I want to debunk a few myths I encountered on my journey that almost deterred me from the challenge.

Pre-PWK/OSCP Background
--
Let me preface this portion of the blog with this message- PWK is an acronym for Penetration Testing with Kali Linux. This is the accompanying course to the OSCP certification and it only after its completion can an attempt at OSCP can be made. My journey to OSCP begins in November 2017, during my Thanksgiving break at school. I was three years deep into a BS in cybersecurity. Schooling was the scope of my knowledge at this point. In school, I only was ever marginally interested in network functionality and implementation. I had never made any efforts outside of class at this point. The notion that I was going to be left behind by my peers led me to [Code Academy](https://www.codecademy.com/learn/learn-the-command-line), where I embarked on a journey to learn the Linux command line in. The culmination of the course and the drive to learn only increased my feelings of fervor. This course would later provide me the bedrock needed to get where I was going. Subsequently after this course I found myself conversing with some peers about my new-found Linux knowledge. At the conclusion of this engagement, I found that maybe penetration testing was the road I was going to tread down next. And by tread, I mean walk blind folded, with both of my legs broken. I ***REALLY*** had no idea what I was doing at this point in my development. A friend informed me that [Vuln Hub](https://www.vulnhub.com/) should be the next stone cast for me. I was advised to learn and "practice" some exploitation methods on these machines. Looking back, what I am about to say is so overtly absurd. The extent of my "exploitation" knowledge was that I knew about this divine tool called "Metasploit." To me, Metasploit was this mythical extension of Christ Himself. It could audit any application in the world. It either meant I was going to get this magical, unauthorized remote shell stemming from another device ***OR*** I was going to receive a somber message of "Exploit completed, but no session was created." I also knew that if I queried for an exploit in Metasploit and it contained "Buffer Overflow" in the title, it was going to give me probably a 20 percent better chance of exploitation (in my mind, anyway). I hadn't a clue in the slightest about what a buffer overflow was or why it worked, but that's what was going through my head. What is more comical, is my friend gave me a list of machines to try out from Vuln Hub. If I secured a shell, I revered in triumph. If I did not receive a shell, I deemed the computer to be locked down and secure! After some explanation, coaching, deep breaths, late nights, and Mountain Dew Baja Blasts, I was semi-okay at Vuln Hub. I had managed to PWN about 4 machines at this point. Still an ambitious, hungry, and hopeful lad- I still was actively researching on how to hone some of my new-found skills. I found a humble abode that would change my life forever in January of 2018 called [Hack The Box](https://www.hackthebox.eu/). Hack The Box is the single most important tool I came across in my development. From January into March all I did was Hack The Box. Every. Single. Day. It is very much akin to Vuln Hub, but you do not download the vulnerable machines. You VPN directly into their hostile and uncertain network- attacking machines remotely. The storage on my SSD admittedly thanked me for finding this place. I was engaging in Hack The Box unceasingly. I will attest, it was integral in regards to my OSCP certification. I will give a more in-depth decree on Hack The Box in the Resources portion of this blog.

Enrollment
--
When March arrived, my confidence was really flourishing and evolving. I was refraining from the Metasploit when possible and I was using what I consider to be more proper methodologies. I was scanning for open ports on potential victim machines and then properly enumerating each port. If HTTP was open, I was utilizing Burp Suite to see how data flowed through the application. Tools like Nikto, Gobuster, and the Nmap scripting engine were all marvelous when it came to auditing web applications for vulnerabilities. I was banner grabbing other ports for vulnerable versions of applications. I also found myself being more complacent with privilege escalation. I was understanding progressively how kernel exploits functioned- and compilation of the exploits were happening more auspiciously. I was becoming keen on distinguishing weak services on Windows and Linux that could lead to a privileged shell. I was also cultivating my **root.txt** dance (all of my Hack The Box readers will understand). I still was not where I am at today, nor where I needed to be. Although I was deterred from my lack of technical ability, one fantastic thing did come to fruition at this point. I knew at this point I ***HAD*** to be a penetration tester. It is what I love. But how could I, a college student with no penetration testing experience, accomplish such a daunting feat? I researched what credentials I needed- and I came across a slew of information security certifications. I came across CEH (I do not recommend this certificate, although it may be good for some), GPEN (expensive. Very, very expensive), CISSP, Security +, GCIH, and some others. But then I came across this BEAST called OSCP. OSCP, after reading about it, was almost impossible to pass for someone in my shoes. People with years of experience fail. This made me want it more! I knew this would be my way out! After about a month of reflection, prayer, and advice from others around me- I decided it was showtime.

Times up, let's do this
--
April 26th, 2018. "Thank you for your interest in Penetration Testing with Kali Linux, Please read this entire email carefully as it contains very important information." I had just submitted my application to PWK! I was ready to ride the NOP sled to OSCP (Exploit Development joke)! 
Let me fill you in on how overloaded I was at this time:
  1. I was working 40 hours a week as an intern
  2. I was driving 4 hours round trip, 3 days a week for a face to face course. This forced me to get in at 6 a.m. to work to 
     compensate the hours.
  3. I was also taking 3 other online courses.
  
I consider myself very assiduous. Even this was daunting for me. I was now about to add embarking on a long and winding road to that list! Crazy, I know. I also do not share this message to come off as a martyr. I want it to be known- there is no excuse for not taking the plunge if you truly want it. If you talk about it, be about it! Copious amounts of people ask me, "Connor how much time did you spend on PWK?" There are 3 paces you can select with PWK. 30, 60, or 90 days. I opted for 60 days. I spent 3 hours Monday through Friday jamming in coursework and labs. I then spent every waking moment on Saturday and Sunday doing the same. Having said that, I am human. There were some days I spent time watching movies, doing homework, playing sports, or playing video games. This is the amount of dedication I found myself putting in. You must recall this though- this is a blog on someone who had no experience obtaining OSCP. A more seasoned veteran may be able to get away with less- but I would advise dedicating whatever time and resources you have towards it.


May 26th, 2018. PWK D-DAY.
--
A date that forever altered the course of my life- for the better. This was my start date for PWK. There are a mass of blogs out there for the technical content of PWK. I want to try to establish an OSCP blog that is unique to my situation. This blog is going to talk about the following: what to expect, how to document, and some resources. This is not a "how to pass OSCP" blog, and I refuse to become a part of that machine. Documentation is the single most important commodity for red teamers. To pass the OSCP exam, you must submit a report. The OSCP exam consists of an undisclosed number of vulnerable machines in a network you have no prior knowledge of. Your grade will be determined by a committee of individuals from OffSec. They will read your report AND ONLY your report. Later in this blog, you will get more specifics about the exam and report- here I am stressing the importance of documentation. 
Here is what you can expect from PWK:
  1. **Exploit Development**- You will grasp the basics of exploit development. You will reverse engineer an 
     application and probe it for Buffer Overflow vulnerabilities. This include attaching an application to a debugger and 
     understanding what you are looking at. (If this seems daunting do not worry, it was to me at first.) But remember that this      is a ***LEARNING COURSE TAUGHT BY PROFESSIONALS***. You are here to learn, and they will teach you.
  2. **Enumeration**- This is a term that is used all. of. the. time. Enumeration is the process of probing, 
     discovering, and using what you know to come up with an attack vector. Enumeration includes things like scanning    
     machines with Nmap and various tools. Enumerating could also mean you play around with the functionality of a web
     application and seeing what you can do to abuse its functionality. When someone tells you to "enumerate" more it may            seem like a sarcastic answer that does not help. It is actually the best answer! It means that you are close, you just need      to look with a stronger magnifying glass and try harder! Someone encouraging you to enumerate means that they only want          you to learn for yourself. If you get told to enumerate, do not fret. Take a break and come back to it! You eventually          will find the attack vector with enough effort. PWK gives you the tools to find the vulnerabilities!
   3. **Web Application Exploitation**- This topic encompasses a vast portion of the PWK course. EVERYTHING uses a web app these 
      days from banks, schools, and governmental services. Many companies only pay for web application assessments. You will 
      learn fundamentals  of Cross-Site Scripting, Cross-Site Reverse Forgery, PHP exploitation, reviewing poor source code,
      SQL injections, File Inclusion Vulnerabilities, and my favorite- default credentials! Always check those firstly :).
   4. **Privilege Escalation**- This will encompass only 2 attack vectors primarily. These include misconfigurations and kernel
      exploitation. You will learn what services are weak and where you should look when you have a low privileged shell. 
      From a kernel exploit perspective, you will need to understand why a kernel exploit works and how to successfully
      compile one.
   5. **Using Exploit-DB and Metasploit**- This is where the fun comes in. These attack vectors take advantage of publicly
      known exploits. These generally will be exploits that take advantage of vulnerabilities in memory. These will inject 
      shellcode most likely into memory. You will also, at times, be tasked with modifying publicly available exploits to fit 
      your needs. Do not worry- it is not as daunting as one may think! Again, Offensive Security are world class instructors. 
      You will get the information you need!
      
      
Exam Day
--
I am not going to get in specifics here, I will just briefly touch on my experience. If you were comfortable with the PWK course and labs, you will be fine! Just enumerate properly and leave no stone unturned. I passed my exam on the first try. I do not mean to sound pretentious with that last sentiment, I just want to provide what transparency I can. I also opted in for the proctored exam, so the integrity of my exam is intact. If you enumerate, use google, and put forth maximum effort- there is no reason you should not pass! The OSCP exam was an ample amount of fun for me! Let's talk specifics. It is a 24-hour exam and you are presented with a number of hosts to compromise. The goal is ALWAYS to obtain a shell as a privileged user. As you are taking the exam, you need to be capturing screenshots (you will know what to screenshot when the time comes- trust me) and documenting the exploitation process. You will need to provide an enthralling written document with all of your findings and submit it for a grade. I will provide links to helpful websites at the end with all of this information. Make sure you follow ALL of Offensive Security's instructions. Passing OSCP has been one of the greatest pleasures on my young life- and I am proud to be apart of the community that have all "Tried Harder."


How Did I Document My PWK/OSCP machines?
--
Most blogs talk about the technical skills required- but I believe documentation is far superior in notoriety. OneNote is going to be your best friend. I recommend OneNote 2016.I also recommend 3 computer monitors for this whole journey! 1 for your Kali machine, 1 for OneNote, and 1 for the videos/PDF. I created an example template on how I documented my findings below. I found this method to be the most effective (these are fake IP addresses, so don't even try it):

<img src="{{ site.url }}{{ site.baseurl }}/images/Screenshot.png" alt="">

I realize this picture is small, but I will break it down so you can see it more easily.

First thing I do is create a new tab with the IP address of the machine I am going after with the hostname (here it is 10.10.10.10 TEST and 10.10.10.20 TEST_DEV along with 10.10.10.30 PROD_1):

<img src="{{ site.url }}{{ site.baseurl }}/images/Screentshot4.png" alt="">

Secondly, I run a port scan and I list all of the open ports with their services in numerical order:

<img src="{{ site.url }}{{ site.baseurl }}/images/Screenshot2.png" alt="">

Third, I enumerate the port and I document my steps with screenshots:

<img src="{{ site.url }}{{ site.baseurl }}/images/Screenshot 3.png" alt="">

This is the best approach I could come up with. I believe documentation plays the most pivotal and integral role in this whole process. A client does not buy a penetration test! They buy your documentation, so you can begin the remediation process. 


Resources
---
Here are a list of resources I used to take me from a zero to a hero!:

1. [Learning the Terminal](https://www.codecademy.com/learn/learn-the-command-line)- this is vital. You have to understand these basics before you can pursue anything more advanced.
2. [Vuln Hub](https://www.vulnhub.com/)- I am not a proponent of blogs saying which boxes you should attempt. It is about the methodologies. Any of them will do! Try them all. BUT DO ATTEMPT BRAINPAIN 1!!!!! Hint, it utilizes exploit development.
3. [Hack The Box](https://www.hackthebox.eu/)- start with the easier machines. Get your methodologies down, and document!!  I left some screenshots above on how to document. Get OneNote, make a HTB notebook, and go at it! All of those boxes will help prepare you. Again, not a fan of people giving specific boxes.
4. [Spawning TTY lines](https://netsec.ws/?p=337)
5. [Reverse Shell Cheat Sheet](http://pentestmonkey.net/cheat-sheet/shells/reverse-shell-cheat-sheet)
6. [Penetration Testing Cheat Sheet](https://ired.team/offensive-security-experiments/offensive-security-cheetsheets)
7. [Understanding Reverse and Bind Shells](https://www.hackingtutorials.org/networking/hacking-netcat-part-2-bind-reverse-shells/)
8. [Signing Up for OSCP](https://www.offensive-security.com/preregistration.php?cid=21)
9. [PWK Syllabus](https://www.offensive-security.com/documentation/penetration-testing-with-kali.pdf)
10. [OSCP/PWK Example Documentation](https://www.offensive-security.com/pwk-online/PWK-Example-Report-v1.pdf)
11. [OSCP Exam Guide](https://support.offensive-security.com/oscp-exam-guide/#oscp-certification-exam-guide)

Ending
--
There is not one tride and true method for obtaining OSCP. The goal of this blog was to show anyone can obtain OSCP. If you dedicate yourself enough, you will find yourself jumping up and down doing the root.txt dance when you receive your passing email from Offensive Security. Please feel free to reach out with any questions! If you just stay dedicated, go through the coursework before you hit the labs. Have an awesome rest of your day! :)
