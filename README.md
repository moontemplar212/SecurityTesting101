# SecurityTesting101
Basic security testing

> https://www.guru99.com/what-is-security-testing.html \
> https://www.softwaretestinghelp.com/how-to-test-application-security-web-and-desktop-application-security-testing-techniques/

  - Vulnerability Scanning
  - Security Scanning
  - Penetration Testing
  - Risk Assessment
  - Security Auditing
  - Posture Assessment
  - Ethical Hacking

Security Testing Techniques:
  1. Application Access and User Management:
    a.  Roles and Right management: Is the appropriate level of access in an application commensurate with the user role / responsibilities?
    b.  Summarised in Authentication: Who are you? and Authorisation: What can you do?
      Authentication: 
        Password Management:
          - Encryption: Salting and hashing
          - Password quality rules
          - Default users or logins
          - Password recovery
          - Captcha
          - Logout functionality
          - Password change
          - Security Questionaire
      Authorisation: 
        Application specific: Do you have access to only what you need to do your job and no more?
          - Session management and cookies
          - Path traversal
          - Missing authorisation
          - Horizontal access controls
  
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
        - Algorithm usage such as SHA256
        - Certificate validity

3. Brute Force Attack:
        
        
        
        




System/Application Management:
  - Session timeout and cookies
  - Sensitive information should not be reachable using the browser back button

Security Testing Tools:
  - Netsparker
  - Indusface WAS
  - Intruder
  - OWASP (ZED, Dependency checks, Web Testing Environment )
  - Wireshark
  - W3af

