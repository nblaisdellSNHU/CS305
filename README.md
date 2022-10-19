# CS305

Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?
- Artemis Financial is a consulting company that develops individualized financial plans to their customers, including savings, retirement, investments, and insurance plans. 
- They want to create a custom software for interacting with them and their products, but they want to ensure that the most up-to-date and effective security measures are in place for their application.
- Specifically, they wanted to be able to use a hashing function to generate a checksum for their file uploading, to make sure the data is kept secure during transfer and encrypted along the way.

What did you do very well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?
- I feel I was able to identify the proper algorithm cipher (SHA-256) for the checksum requirement.
- It's very important to code securely so that we don't inadvertently introduce vulnerabilties into our software.
  - If we don't, we could lose data, money, or even worse potentially!
- By ensuring security in the software as we build it, it allows for the peace-of-mind knowing that all that can be done to make sure the data and integrity of the software is kept safe was done.

What part of the vulnerability assessment was challenging or helpful to you?
- At first, interpreting and understanding the OWASP dependency check report was difficult and I wasn't really sure where to look. However, after a few weeks of using the same report for multiple projects, and looking deeper into the information presented on the report, I feel I was able to understand it much more by the end of the course.

How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?
- By adding a REST endpoint using the Spring framework, and using the SHA-256 hashing algorithm to generate a checksum for a given (static) input.

How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?
- Before adding any new code, I ran the dependency check report, and then I ran the same report after making my code changes. After reviewing both reports, they were identical, meaning that the changes I made did not introduce any new bugs or vulnerabilities.

What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?
- I would use another dependency checking library to make sure any libaries in use in my applications aren't vulnerable, and if they are, I'm taking the measures to mitigate any of those vulnerabilties. 
- I would also make use of Google and databases like the NVD to see if there is any additional information for the libraries in use in my applications.

Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?
- I would show the report, which encapsulates most, if not all, of what was learned during this course.
