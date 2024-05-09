# Lab Report 3

## Part 1

1. This is a failure-inducing code that was in our JUnit testing.
```
  public void testReverseInPlace2() {
    int[] input2 = { 4, 5, 6 };
    ArrayExamples.reverseInPlace((input2));
    assertArrayEquals(new int[]{ 6, 5, 4 }, input2);
  }
```

2. This is a non-failure-inducing code that is our JUit testing.
```
  static int[] reversed(int[] arr) {
    int[] newArray= new int[arr.length];
    for(int i = 0; i < ar.length; i += 1) {
      newArray[i] = arr[arr.legnth - i - 1];
    }
    return newArray;
  }
```

3. These are the symptoms of running the failure-inducing code from above.

  ![image](https://github.com/TallAverageTree/cse15l-lab-reports/assets/146666323/66302cde-b0a8-4669-ab09-c1e629c38abe)

4. This is the fixed code from #1 that now works without errors.
```
  static void reverseInPlace(int[] arr) {
    int[] inputArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      inputArray[i] = arr[arr.length - i - 1];
      }
    for(int i = 0; i < inputArray.length; i += 1) {##Pa
      arr[i] = inputArray[i];
      }
  }
```

5. The fix addresses the issue of the original code as the original code did not return the array that was reversed. The fix created a new array that was returned with the numbers in the array reversed.

## Part 2

The command I chose to use is `grep`. 

### Option 1
* -r, --recursive
* It recursively searches for patterns in files and directories.
* Example: `grep -r "search_term" ./technical`
* Example Outputs:
```
./technical/file1.txt
./technical/subdirectory/file2.txt
```

### Option 2
* -n, --line-number
* It finds the prefix of each line of output with the 1-based line number within its input file.
* Example: `grep -n "search_term" ./technical/file1.txt`
* Example Outputs:
```
1:This line contains the search_term.
3:This is the third line containing the search_term in file1.
```

### Option 3
* -i, --ignore-case
* It performs a case-insensitive search.
* Example: `grep -i "search_term" ./technical/file1.txt`
* Example Outputs:
```
This line contains the Search_Term in file1.
This is the third line containing the SeArCh_TeRm in file1.
```

## Option 4
* -l, --files-with-matches
* It suppresses the normal output and instead prints the name of each input file from which output would normally have been printed.
* Example: `grep -l "search_term" ./technical/*`
* Example Outputs:
```
./technical/file1.txt
./technical/subdirectory/file2.txt
```



Sources that I used:
- [Linuxize - Grep Command in Linux](https://linuxize.com/post/how-to-use-grep-command-to-search-files-in-linux/)
- [The Linux Documentation Project](https://man7.org/linux/man-pages/man1/grep.1.html)
- [GeeksforGeeks](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
