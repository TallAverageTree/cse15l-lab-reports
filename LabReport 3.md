# Lab Report 3


# Part 1


## First Message
![First_Message](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/2f0ef8bc-c3d1-4aeb-9c2b-4018cb0c61ca)


## What methods are being used?
- The `handleRequest` method of the `Handler` class is called, and within it, the `logPrintedMessage` method is called to log the message. Finally, `getChatHistory` method is called to retrieve the chat history for the user "Ryan".
## What are relevant arguments to methods/values of relevant fields to the class?
- In the `handlerequest` method, the arumenurl.getPath(): "/add-message"
- In the `handlerequest` method, url.getQuery(): "s=Hi Jonathon&user=Ryan"
## Any values of relevant fields of the class change from this request?
- In the `Handler` class, `logPrintedMessage` method is called with the message "Ryan: Hi Jonathon\n".
## Arguments that Changed from the Specific Request
Changes to relevant fields of the Handler class:
  - The `logPrintedMessage` method is called with the message "Ryan: Hi Jonathon\n". This message is appended to the log file.


## Second Message
![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/0c25c6f1-fa14-4fc5-80c0-09f50df84d7f)


## What methods are being used?
- The `handleRequest` method in `Handler` Class, `logPrintedMessage` method in the `Handler` Class, `getChatHistory` method in the `Handler` Class, and `main` method in the `ChatServer` Class.
## What are relevant arguments to methods/values of relevant fields to the class?
Arguments of `handRequest`:
- URI url: Represents the request URL.
- url.getPath(): "/add-message"
- url.getQuery(): "s=Hi%20Ryan&user=Johnathon"
Arguments of `logPrintedMessage`:
- message: "Johnathon: Hi Ryan\n"
## Any values of relevant fields of the class change from this request?
- In the `Handler` class, `logPrintedMessage` method is called with the message "Ryan: Hi Jonathon\n".
## Arguments that Changed from the Specific Request
Changes to relevant fields of the `Handler` class:
- The `logPrintedMessage` method is called with the message "Ryan: Hi Jonathon\n". This message is appended to the log file.


# Part 2


## LS on Local Machine
![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/50a2c3cc-69dc-418b-9b84-5ed9a13af5ef)


## LS on IENG6 Machine
![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/11776376-3f0c-4528-ba21-0afd0d74170e)


## Login Without Password
![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/dfa0f4c7-c813-4789-9142-46eb1df6d33b)


# Part 3

> Something new that I learned in week 3 was how to connect to another machine using my local terminal and machine. I found it very interesting with the fact that I could
> login to another computer, even more so when I could do it without using a password. It was very cool to learn that I could do projects and store my assignments on another
> computer so that I don't always have to use my storage on my own computer.
