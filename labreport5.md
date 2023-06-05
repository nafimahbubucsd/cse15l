# Part 1: Debugging Scenario
###### Tutor's Response

Re: Debugging issue with reversed() method in ArrayExamples.java 

Hello John, I appreciate you reaching out for assistance. 
Today, I'll be aiding you in resolving this issue! 
Upon inspection, your ArrayTests.java file seems to be in good shape. However, there appears to be an issue with your ArrayExamples.java code, particularly the reversed() method. Could you kindly share your complete ArrayExamples.java code? 

In the meantime, I'd recommend running the following commands in your terminal:
```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar ArrayExamples.java``` 
```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ArrayTests```

If executing these two commands each time you test feels burdensome, consider creating a bash script. Here's a sample bash script "arraytest.sh":
```java
set -e
javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar ArrayExamples.java
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ArrayTests
```
After running the bash script in your terminal, try: 
```java
bash-3.2$ echo $?
```
This command will return 1 if there's an error, or 0 if everything is fine. It's a quick way to see if there's an error or not.

I'd appreciate it if you could share the outcome after executing these commands so I can better identify your exact issue. 

Best Wishes, 

Nafi Mahbub.


# Part 2: Reflection
One of the best parts of my time in the lab was when we learned about server.java and localhost. I didn't really know how to use Java code back then, so I asked the teaching assistants for a lot of help. But when I found out that I could change the URL and localhost server with Java code using VSCode, it felt awesome. That's when I started to enjoy coding and computer science even more. I was excited to learn new stuff like making an autograder, writing a bash script, learning about vim, and all that. This class and its lab were more useful than any other class I've taken before. I'm really thankful for all the helpful stuff we were taught.
