# Lab 4: Vim (Week 7)

## Step 1: Accessing Files

I make sure that my directory is `lab7` and if it isn't, I make sure that I use the command `cd lab7` in order to change my directory. I then put into my terminal the command `vim ListExamples.java` in order
to access the doucment and start edting the document.

![vim ListExamples](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/eb58e0bf-455a-4f26-a037-d9a3e95877fb)

## Step 2: Locating Error

Keys Pressed: `<down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <down>, <right>, <right>, <right>, <right>, <right>, <right>, <right>, <right>, <right>, <right>, <right>, <right>, <x>, <i>, <2>, <esc>, <:>, <w>, <q>, <enter>`

Meaning: The line which I had to change was on line 43, so I pressed down until I reached line 43, then I moved right 11 times to get to the 1 in `index1 += 1;` line.

![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/cef428e8-93e3-4a40-86da-3a382f67fefd)

## Step 3: Editing the Error

Keys Pressed: `<x>, <i>, <2>, <esc>`

Meaning: Once we had moved our position to be right over the letter that we wanted to change from the last step, we pressed `<x>`, which is a vim command to delete the character our cursor is hovering. In this case, it would be the character "1". We then press `<i>` in order to insert a character where our cursor
is, which in this case would be "2". We then press `<esc>` in order to exit the editing process.

**Before:**

![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/0748d180-dfa6-4bf3-9903-648820920c0f)

**After:**

![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/0abc785a-d915-42ca-86f5-e0f19695430b)

## Step 4: Saving and Checking for Errors

Keys Pressed: `<:wq!>, <bash test.sh>`

Meaning: In order to save and exit from the file, we type in `<!wq>`, which is a vim command that saves and exits a file safely after you make your edits. We then type in to our terminal the command `<bash test.sh>` in order to make sure that our tests run correctly without error.
