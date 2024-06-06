# Lab Report 5


## Original Student Post

Hi Everyone,

I'm encountering a NullPointerException when I run my Java program, and I'm not sure what's causing it. The error seems to occur when I try to access an element in an array. 
I've attached a screenshot of the error message and the relevant part of my code. I suspect it might have something to do with the initialization of my array.

Code:
```
public class ArrayExample {
  public static void main(String[] args) {
    String[] words = new String[3];
    words[0] = "hello";
    words[1] = "world";
    System.out.println(words[2].toUpperCase());
    }
}
```
Error Screenshot:

![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/b054e9d0-dd22-48d9-9f18-cf23f295ee86)

## TA Response

Hi,

It looks like the NullPointerException is happening because you're trying to call toUpperCase() on words[2], which hasn't been initialized yet. Try adding a check to see if 
the element is null before calling toUpperCase().

## Student Response

I've updated the null check and here is the updated code and output.

Updated Code:
```
public class ArrayExample {
    public static void main(String[] args) {
        String[] words = new String[3];
        words[0] = "hello";
        words[1] = "world";
        if (words[2] != null) {
            System.out.println(words[2].toUpperCase());
        } else {
            System.out.println("words[2] is null");
        }
    }
}
```
Error Screenshot Update:

![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/ec8620dc-dc73-4917-912c-b958ad6a8878)

## Final Report:

File & Directory Structure:

- ArrayExample.java in the root directory.
- run.sh in the root directory.

Contents of Each File Before Fixing the Bug:

ArrayExample.java:
```
public class ArrayExample {
    public static void main(String[] args) {
        String[] words = new String[3];
        words[0] = "hello";
        words[1] = "world";
        System.out.println(words[2].toUpperCase());
    }
}
```
run.sh:
```
javac ArrayExample.java
java ArrayExample
```
Command Line to Trigger the Bug:
```
bash run.sh
```
Description of What to Edit to Fix the Bug:

To fix the bug, add a null check before trying to call a method on words[2]. This prevents the NullPointerException by ensuring 
that the code only attempts to call toUpperCase() if the element is not null.

Updated ArrayExample.java:
```
public class ArrayExample {
    public static void main(String[] args) {
        String[] words = new String[3];
        words[0] = "hello";
        words[1] = "world";
        if (words[2] != null) {
            System.out.println(words[2].toUpperCase());
        } else {
            System.out.println("words[2] is null");
        }
    }
}
```

With these changes, the program now checks if words[2] is null before calling toUpperCase(), preventing the NullPointerException and printing an appropriate message if words[2] is null.

## Part 2
- Something that I didn't know in the second half of the quarter that I learned was VIM. I thought that it was super cool and interesting to learn about how you can alter and change an entire
  file from just the terminal/command line. I had always thought that you had to go to the actual file location to change and alter the contents, but ever since I've learned about VIM, I have
  been using it more and more to make changes to files without needing to go to the file. 
