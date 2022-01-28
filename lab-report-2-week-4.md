# Lab Report 2 Week 4

# Debugging

## BugFix 1

**Bug:** 

[Link to the failure inducing input text file](misc/text-file.java)

**Symptom:**

![Image](images2/error1.png)

**GitHub change:**

![Image](images2/error1githubsolution.png)

If the file did not end with a valid link, the code infinitely looped. This is shown by the symptom because it runs out of memory for a simple program because it keeps adding the same links to the `getLinks` method. This is solved by breaking the loop if it returns to the beginning.