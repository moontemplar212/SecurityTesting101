# Security Testing 101
Basic security testing

---

> https://www.guru99.com/what-is-security-testing.html  
>
> https://www.softwaretestinghelp.com/how-to-test-application-security-web-and-desktop-application-security-testing-techniques/  

---

Security testing is about making sure that authorised access is granted where and when it is needed to protect data and that unauthorised access is restricted.<br>

There are seven major areas of security testing:<br>

  1. Vulnerability Scanning  
  2. Security Scanning  
  3. Penetration Testing  
  4. Risk Assessment  
  5. Security Auditing  
  6. Posture Assessment  
  7. Ethical Hacking  

---

Security Testing Techniques:<br>
  1. **Application Access and User Management:**<br>
    > Roles and Right management: Is the appropriate level of access in an application commensurate with the user role / responsibilities?<br>
    > Authentication: Who are you?<br>
        Password Management:  
          - Encryption: Salting and hashing  
          - Password quality rules  
          - Default users or logins  
          - Password recovery  
          - Captcha  
          - Logout functionality  
          - Password change  
          - Security Questionaire  
    - Authorisation: What can you do?<br>
        Application specific: Do you have access to only what you need to do your job and no more?
          - Path traversal  
          - Missing authorisation  
          - Horizontal access controls  
          - Sensitive information should not be reachable using the browser back button  
  
  2. Data Protection:  
    a. Data Access: Does the user have access to view and utilise the data which they are supposed to use?  
    b. Storage: How is the data stored:  
      Database Management:  
        - Roles and Rights  
        - CRUD: Create, Read, Update, Delete  
        - Encryption and data flow  
        - Query for plaintext usernames and passwords  
        - Query for business critical or sensitive information  
      Web Management:  
        - Data transfer is encrypted and decrypted properly particularly in 'submit' actions  
        - Sensitive information displayed in the address bar is not in a human readable format  
        - Approrpiate algorithm usage such as SHA256 and excluding weak algorithms  
        - Certificate validity  

3. Brute Force Attack:  
  a. Assuming a valid username, a successful login is attempted using software tools by trying to guess the password again and again  
    Suspension of an account for 30 minutes once 3 or more incorrect attempts have been made is a common method for dealing with this attack type  

4. SQL Injection and XSS ( Cross-Site Scripting ):  
  - Field length should be smaller than the required space to input a script  
  - Field length should be as long as is needed for the required input field  
  - HTML and script tags input should be prohibited  
  - Anonymous access methods should be disabled  
  a. SQL Injection:  
    - Any inputs should be sanitised prior to executing code in the database  
    - Detection techniques  
    - Standard SQL injection techniques  
    - Fingerprint the database  
    - Exploitation Techniques  
    - SQL Injection Signature Invasion Techniques  
  b. XSS ( Cross-Site Scripting ):  
    - Any redirects from untrusted sources should be discarded  

5. Service Access Points (Sealed And Secure Open):
  a.   
  
6. Session Management:  
  a. Session timeout:  
    - Session expiry after an explicit idle time  
    - Session termination after a maximum lifetime  
    - Session termination after log out  
    - User session count and/or multiple simultaneous sessions  
  b. Cookies:
    - Cookie scope and duration  
    - Cookie entropy  

7. Error Handling  
  a. Error Codes:  
    - Check for error codes such as 400, 404, 408, etc.  
    - Error messages should not return any critical information that could be used for hacking purposes  
    - Stack traces should not be included as they may contain information for hackers  

8. Specific Risky Functions:  
  a. Payments  
    - Crypotgraphic storage
    - Buffer overflows
    - MITM attacks
    
  b. File Uploads
    - Restricting uploads to whitelisted file types
    - May want to parse the contents of the file before upload

Security Testing Tools:
  - Netsparker
  - Indusface WAS
  - Intruder
  - OWASP (ZED, Dependency checks, Web Testing Environment )
  - Wireshark
  - W3af

