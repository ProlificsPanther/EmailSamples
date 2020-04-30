<h1>WithJava</h1>

Put 'mailtest.jar' into your CLASSPATH.  'mailtest.jar' contains the classes 'SendMail.class' and 'SendMail2.class', which are the supporting classes for the 'mailtest' and 'mailtest2' Panther screens, respectively.

Also, put 'mail.jar' into your CLASSPATH. It is located in the javamail-1.4.5 subdirectory.  Only 'mail.jar' and 'mailtest.jar', in addition to 'pro5.jar', are needed in your CLASSPATH. 

Two samples are provided.  The screen, 'mailtest', in 'mailtest.lib' uses the Java class 'SendMail', and is in the style of Panther event handlers written in Java.  The other screen, 'mailtest2', uses the Java class 'SendMail2', and is in the style of Java Object support directly from JPL.

For 'mailtest', "SendMail" is the java tag on the Send Mail button on that screen.  For 'mailtest2', the SendMail button executes a control string for validation, which calls a JPL procedure that is defined in the screen's JPL.  That JPL procedure uses Panther's sm_obj_xxx APIs to call methods of the 'SendMail2' class.

For either sample screen, if you select 'smtp.gmail.com' or 'webmail.prolifics.com', 'security' and 'port' are chosen for you to be correct for those mail servers.  Default values for other fields on the screen will need to be changed.

It is assumed that authentication is required.  The samples can be modified if this is not so, and can be enhanced in other ways.  Support for POP3 and IMAP can also be added.

The Java source code in this Panther sample, SendMail.java, was mostly copied from demo source code provided with Oracle's JavaMail 1.4.5. There are many demos in JavaMail 1.4.5 containing source code showing how to use additional features.

Add activation-1.1.jar only if you are using OpenJDK and point it to CLASSPATH.

Note that the subdirectory, javamail-1.4.5, contains a subset of Oracle's JavaMail 1.4.5.  Only the redistributable file, 'mail.jar' is provided herein.  Also, be aware of the restrictions on its use as described in the files, LICENSE.txt and distributionREADME.txt, which are also provided in the javamail-1.4.5 subdirectory.  You may download a full implementation of JavaMail from Oracle at 'http://www.oracle.com/technetwork/java/javamail/index.html'.

Need a Panther Web 552 Redhat Image? [Click Here](https://hub.docker.com/r/prolificspanther/pantherweb "Named link title") 

[Click Here](https://prolifics.com/panther-trial-license-request/ "Named link title") for a 45-day license.

How to set up a Panther Servlet Web Application? [Click Here](https://github.com/ProlificsPanther/PantherWeb/releases "Named link title")

Read our Documentation [here](https://docs.prolifics.com)
