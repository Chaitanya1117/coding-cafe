#CODING CAFE TASKS

###Q1: What did pwd print?
Ans 1. It prints the absolute file path.

###Q2: What did ls -a show that plain ls did not?
Ans 2. ls -a shows the hidden files alongside other files while ls only shows normal files.

###Q3: . Pick one line from ls -l. What do you think the first column means
Ans 3. The first column is a string which starts with -rw-r. The first character shows if it is file or directory

##Q4:. Why does that work from where you are standing? Which kind of path is coding-cafe/week02?
Absolute or Relative?
Ans 4. . It works without cd because coding-cafe/week02 is a relative path it's relative to wherever I'm currently standing . Since I was already sitting inside coding-cafe, the shell just follows the rest of the path from there.

###Q5. mv did two different jobs above. What were they?
Ans 5. mv did two jobs , the first one was that it moved README-backup.md into the week01/ folder , then it renamed it to old-readme.md

###Q6: . How many folders are on your PATH? (They are separated by :)
Ans 6. There are 22 folders on my path.

###Q7: Write down exactly where your python3 lives. You will need this again in a minute.
Ans 7. /usr/bin/python3

###Q8: . Compare your answer to 7 with the person next to you. Are they the same? If not, why might that be?
Ans 8: The person next to me had 27 folders which means they are different. They are not same because we installed python differently.

###Q9. What exactly did the shell say? Explain the error in your own words, using the word PATH.
Ans 9. It said pyton3: command not found.This error occurs because the shell searched through every single folder listed in my PATH variable and could not find any program that matches that misspelled name.

###Q10. .venv did not appear with plain ls. Why not? (Refer back to section 1.)
Ans 10. Because anything starting with a dot is treated as a hidden file/folder, and plain ls skips hidden stuff by default. That's exactly what we saw back in section 1 with ls -a showing more than ls.

###Q11. What changed about your prompt?
Ans 11. (.venv) showed up right at the start of the prompt, before my folder path.

###Q12. Compare this with what you wrote down for question 7. Is it the same path? If not, what does that tell you about what activate actually did to your PATH?
Ans 12. No its not the same path, this tells me that the activate command modified my PATH variable by placing the virtual environment 'bin' folder at the very front of the list.

###Q13. What is in the second list that was not in the first?
Ans 13. The second list contains certifi, charset normalizer, idna, pip, requests, urllib3 which was not there on the first one.

###Q14. Where does python3 point now?
Ans 14. It points to the global variable path again.

###Q15. Find what the -Rescue flag does.Write it in your words.
Ans 15. It tells a command to look inside a folder and repeat its action automatically for every single subfolder and file inside it.

###Q16. What is the difference between what Ctrl + C and Ctrl + D did?
Ans 16. Ctrl + C Interupts the current action but keeps the Python shell open whereas Ctrl + D sends an exit signal that fully closes the Python shell and returns to the command line.
