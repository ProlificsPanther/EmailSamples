Put 'mailtest.jar' into your CLASSPATH.  'mailtest.jar' contains the classes 'SendMail.class' and 'SendMail2.class', which are the supporting classes for the 'mailtest' and 'mailtest2' Panther screens, respectively.

Also, put 'mail.jar' into your CLASSPATH. It is located in the javamail-1.4.5 subdirectory.  Only 'mail.jar' and 'mailtest.jar', in addition to 'pro5.jar', are needed in your CLASSPATH. 

Two samples are provided.  The screen, 'mailtest', in 'mailtest.lib' uses the Java class 'SendMail', and is in the style of Panther event handlers written in Java.  The other screen, 'mailtest2', uses the Java class 'SendMail2', and is in the style of Java Object support directly from JPL.

For 'mailtest', "SendMail" is the java tag on the Send Mail button on that screen.  For 'mailtest2', the SendMail button executes a control string for validation, which calls a JPL procedure that is defined in the screen's JPL.  That JPL procedure uses Panther's sm_obj_xxx APIs to call methods of the 'SendMail2' class.

For either sample screen, if you select 'smtp.gmail.com' or 'webmail.prolifics.com', 'security' and 'port' are chosen for you to be correct for those mail servers.  Default values for other fields on the screen will need to be changed.

It is assumed that authentication is required.  The samples can be modified if this is not so, and can be enhanced in other ways.  Support for POP3 and IMAP can also be added.

The Java source code in this Panther sample, SendMail.java, was mostly copied from demo source code provided with Oracle's JavaMail 1.4.5. There are many demos in JavaMail 1.4.5 containing source code showing how to use additional features.

Note that the subdirectory, javamail-1.4.5, contains a subset of Oracle's JavaMail 1.4.5.  Only the redistributable file, 'mail.jar' is provided herein.  Also, be aware of the restrictions on its use as described in the files, LICENSE.txt and distributionREADME.txt, which are also provided in the javamail-1.4.5 subdirectory.  You may download a full implementation of JavaMail from Oracle at 'http://www.oracle.com/technetwork/java/javamail/index.html'.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
