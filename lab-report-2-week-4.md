# Lab Report 2 Week 4

# Debugging

## 1. First bug

**Bug:** 

[Link to the failure inducing input text file](misc/text-file.java)

**Symptom:**

![Image](images2/error1.png)

**GitHub change:**

![Image](images2/error1githubsolution.png)

If the file did not end with a valid link, the code infinitely looped. This is shown by the symptom because it runs out of memory for a simple program because it keeps adding the same links to the `getLinks` method. This is solved by breaking the loop if it returns to the beginning.

---

## 2. Second bug

**Bug:**

[Link to the second failure inducing input text file](misc/text-file3.java)

**Symptom:**

![Image](images2/error2.png)

**GitHub change:**

![Image](images2/error2githubsolution.png)

When the file contained an extra `[]` after the last valid link, the code infinitely looped. In this particular case it never adds anything to the array of links, which is why the symptom doesn't show running out of memory as an issue. This is solved by breaking the loop if any of the brackets or parenthese returns to the beginning, instead of just the first open bracket.

---

## 3. Third bug

**Bug:**

[Link to the third failure inducing input text file](misc/text-file4.java)

**Symptom:**

![Image](images2/error3.png)

**GitHub change:**

![Image](images2/error3githubsolution.png)

If the file had non-links that had text or space between the brackets and parentheses, it would still count as a valid link. The symptoms show that the code still added bad links, and also included empty links. I solved this by not executing the code to add the link if it identified that there was text between the brackets and parentheses, or if the link was empty.