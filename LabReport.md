# Lab Report Blog
![CD Examples](CDExamples.png)
`cd`: The absolute directory for `cd` is /c/Users/calan/lecture1. I got the output of going back to the parent directory because when you run `cd` by itself in the terminal, it takes 
      you back to the parent directory. This is not an error.
`cd lecture1/messages`: The absolute directory for `cd lecture1/messages` is /c/Users/calan. I got the output of changing my directory to messages. This is not an error. 
`cd en-us.txt`: The absolute directory for `cd en-us.txt` is /c/Users/calan/lecture1/messages. I got the output "Not a directory". This is an error because `cd` is finding a directory
                while en-us.txt is a file, which results in an error.

![LS Examples](LSExample.png)
`ls`: The absolute directory for `ls` is /c/Users/calan/lecture1. I got the output ![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/8bbfe6d7-4b46-41c3-bcee-0de6c1598d3d).
      This is not an error, as it shows the list from the directory of lecture1.
`ls messages`: The absolute directory for `ls messages` is /c/Users/calan/lecture1. I got the output ![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/fd2b4bce-9b2f-4620-8996-cc3cd4ba3182).
               This is not an error, as it shows the list that is within the directory of messages.
`ls en-us.txt`: The absolute directory for `ls en-un.txt` is /c/Users/calan/lecture1/messages. I got the output ![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/c4ade155-27c0-4b25-84a7-dc8fa097b944).
                This is an error, as there is not list within en-un.txt. This results in an error.

![CAT Examples](CATExamples.png)
`cat`: The absolute directory for `cat` is /c/Users/calan/lecture1. I got no output, as it resulted in a continuous loop, which resulted in no output.
       ![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/834d715e-fd57-4bbb-8025-45f2e8e41b23). This is an error.
`cat messages`: The absolute directory for `cat messages` is /c/Users/calan/lecture1. It resulted in the output ![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/d6f23566-fdbd-4de5-a4b7-d15a1243bc8a).
                This is an error, as you cannot concatenate a directory.
`cat messages/en-us.txt`: The absolute directory for `cat messages/en-us.txt` is /c/Users/calan/lecture1. It resulted in the output ![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/4e95951d-fd3c-4da2-9cbb-4498b8edfd8e).
                          This is not an error, as it concatenated the text within the file of en-us.txt.





