# COMP424-Web-Engineering-II
User authentication web development using PHP, CSS, JavaScript and host in AWS

Developed a web server and website for a small business company. The company is a typical small business company with medium hit-rate site visits for their webpage and very interested in security while not significantly compromising usability.

**1. Preparing the web server**
Prepared LAMP (Linux, Apache, MySQL, PHP) stack web server in latest version of Ubuntu OS in AWS along with necessary security tools to protect it from popular attacks using most popular firewall (IPtables), intrusion detection system (snort).

Wrote two shell scripts to automate the installation and configuration of your system for disaster recovery purposes with comments for every single command:
      installation.sh: Includes all the commands regarding installation of all the necessary services and tools. Also, all configuration scripts for LAMP.
      implementation.sh: Includes all the commands regarding implementing policies for firewall, IDS, etc.


**2. The webpage**
            Web page paradigm: 
                  A login page, and upon successfully logging into the system, it will allow the user to download the company_confidential_file.txt. This page                         displays the successfully logged-in user: "Hi, (First-Name Last-Name)", "You have logged in X times" and "Last login date: Y". You will implement
                  using PHP, MySQL, HTML, JavaScript, and CSS.

      1) The login page
          An "https" webpage redirected from AWS web server would be a simple login page where the user can enter the username and password and a “Login” button.             Also, available on that page are two links: (i) New User? Sign Up and (ii) Forgot Username or Password?. 
          
      2) New user sign up
         New user sign up page has:
            - Typical information about the user: First Name, Last Name, Birth date, E-mail. - 
            - User's password: Password and re-enter password along with real-time proactive password metric feedback (i.e., is this password weak, strong) 
            - Challenge-response test to determine whether or not the user is human (used: CAPTCHA and reCAPTCHA)
            - Activation of account via e-mail.
            - A set of security questions for password retrieval. 

      3) Forgot username and passwordExtra Credit (Up to 15%)
     
**3. Two-Factor Authentication**
Implemented 2FA via Google Authenticator to log in to the website


**Security Testing:**
Suspicious activities, intrusions, or attacks are appropriately logged in. Also, the implementation has required to log all of successful and unsuccessful login attempts. Lastly, we addressed the following attacks in your design and implementation:
        1) Brute force
        2) SQL Injection
        3) Buffer Overflow
        4) XSS
        5) Cross Site Request Forgery 
