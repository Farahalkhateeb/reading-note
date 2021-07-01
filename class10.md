# java script Debugging



![js](https://www.cronj.com/blog/wp-content/uploads/java-script-debugging-1.png)





If you understand execution contexts (which have two
stages) and stacks, you are more likely to find the error
in your code.
Debugging is the process of finding errors. It involves a
process of deduction.


![debugging](https://developer-chrome-com.imgix.net/image/admin/99Omb7ALyJB7MfYpuqXp.png?auto=format)







The console helps narrow down the area in which the
error is located, so you can try to find the exact error.
JavaScript has 7 different types of errors. Each creates
its own error object, which can tell you its line number
and gives a description of the error.
If you know that you may get an error, you can handle
it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback.


In addition to viewing console.log() messages, you can also use the Console to evaluate arbitrary JavaScript statements. In terms of debugging, you can use the Console to test out potential fixes for bugs. Try it now:

If you don't have the Console drawer open, press Escape to open it. It opens at the bottom of your DevTools window.

In the Console, type parseInt(addend1) + parseInt(addend2). This statement works because you are paused on a line of code where addend1 and addend2 are in scope.

Press Enter. DevTools evaluates the statement and prints out 6, which is the result you expect the demo to produce.



![console](https://developer-chrome-com.imgix.net/image/admin/Z5dF1m9vAWBnpMG29Ltv.png?w=964)