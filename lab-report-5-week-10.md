# Week 10 lab Report

- In this lab, I am going to experimented with the many tests provided from commonmark-spec. Then I am going to choose any two tests from the 652 commonmark-spec tests where my implementation had different answers than the implementation we provided for lab 9. 

---
## Finding different test result
-  First, we need to get the results of the different implementations to compare. We can store these results in a text file using a bash script to call MarkdownParse on every file in our test directory, then use the > symbol to output it to a text file.
![Image](script.jpg)

- Next, we can compare out outputs using the vimdiff command. vimdiff will open a vim editor with all the differences in output for the files we give it in in the command line. In this case we will call `vimdiff my-markdown-parse/results.txt markdown-parse-week-9/results.txt`
![Image](Compare.jpg)

- After finding test files that produce different outputs, we can use VS Code's preview window to determine what links should be outputed to determine which implementation failed the test.
