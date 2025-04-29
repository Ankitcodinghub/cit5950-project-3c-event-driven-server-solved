# cit5950-project-3c-event-driven-server-solved
**TO GET THIS SOLUTION VISIT:** [CIT5950 Project 3c: Event-driven Server Solved](https://www.ankitcodinghub.com/product/cit5950-project-3c-event-driven-server-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114495&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CIT5950  Project 3c: Event-driven Server Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<h1><a name="_Toc21855"></a>1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Project 3c: Event-driven Server</h1>
Overview

In Part B, you had implemented a multi-threaded TCP server that supports the 3-way handshake protocol. In this part, you are required to write a single-threaded server (async-tcpserver) that monitors multiple sockets for new connections using an event-driven approach, and perform the same 3-way handshake with many concurrent clients.

Instead of using threads, you will use the select API to monitor multiple sockets and an array to maintain state information for different clients. Along with the manual pages, read Beej’s guide to network programming (<a href="http://beej.us/guide/bgnet/">http://beej.us/guide/bgnet/</a><a href="http://beej.us/guide/bgnet/">)</a> on how to use the select function. We will also provide some sample code on select for you.

<h2><a name="_Toc21856"></a>1.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Requirements</h2>
<h3><a name="_Toc21857"></a>1.1.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Source files and arguments</h3>
All of the requirements from Part A remain the same, with the following changes:

<ul>
<li>You MUST implement the server in async-tcpserver.c instead of tcpserver.c</li>
<li>The makefile MUST create the executable async-tcpserver instead of tcpserver</li>
</ul>
<h3><a name="_Toc21858"></a>1.1.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Handshake Protocol</h3>
All of the requirements from Part A apply to Part C.

<h3><a name="_Toc21859"></a>1.1.3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; End of Line characters</h3>
All of the requirements from Part A apply to Part C.

<h3><a name="_Toc21860"></a>1.1.4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Miscellaneous</h3>
<ul>
<li>You MAY use the epoll family of functions to handle the asynchronous portion of the assignment instead of select.</li>
<li>You SHOULD read the manual pages in detail.</li>
<li>You SHOULD read the manual pages in detail, again.</li>
<li>The server MUST handle two different events for <em>each client: </em>Step 2 (three-way handshake first message HELLO X) and Step 4 (three-way handshake second message HELLO Z). This requirement refers to the Handshake Protocol above.</li>
<li>You MUST place the code for event handling logic into two functions named handle_first_shake and handle_second_shake.</li>
<li>You MAY assume that no more than 100 concurrent client connections will attempt to connect to the server.</li>
<li>You SHOULD reuse the client from Part A. You do not need to make any changes to the client for this part (unless there are still bugs).</li>
<li>All of the requirements from Part A apply to Part C.</li>
</ul>
<h2><a name="_Toc21861"></a>1.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Suggested Approach</h2>
This is a suggested approach. You are free to implement the solution in any manner you want.

<ol>
<li>Start by copying your Part A code into the new source file.</li>
<li>Instead of a single helper function to do the entire handshake protocol, refactor your code such that each individual handshake is handled by a separate event handler function. Your server should still work as a sequential server at this point.</li>
<li>Create two file descriptor sets: one to track <em>all </em>of the file descriptors you are interested in, another to track those that are ready to be <em>read</em>. Be sure to initalise these correctly (by reading the manual pages).</li>
<li>Create some kind of struct to track the state of a single client (e.g. client_state). Because the server will handle each individual handshake asynchronously, the client_state needs to remember what has already happened in order to perform the correct next step. Be sure to initialise it to a known default state.</li>
<li>Since there are potentially multiple clients communicating with the server, you’ll need to keep track of multiple clients, possibly in some kind of array (e.g. a client_state_array). Setup this data structure and properly initialise it as well.</li>
<li>Now for the asynchronous implementation. You’ll have to do some prep work before calling select:
<ul>
<li>Note the arguments to select (from the manual pages). The first argument is the highest file descriptor you are interested in (plus one). Since there are no clients connected right now, the only file descriptor that might have data to read is the listening socket. Be sure to add that socket to the “all” file descriptor set. Additionally, the highest file descriptor may change during the execution of the program (e.g. when you accept a new client), so you’ll need to track this value.</li>
<li>The second argument is a set of file descriptors that you want to read from. You could use the “all” file descriptor set, but unfortunately select modifies the set in-place; select essentially filters out file descriptors that aren’t ready to be read. This is why you have two file descriptor sets. The “all” set keep a record of all file descriptors, while the “read” set can safely be filtered.</li>
<li>Clear out whatever happens to be in the “read” set, then copy the “all” set to the “read” set. Now when select filters out non-ready file descriptors, the “read” set only has file descriptors that are ready to be read, and the “all” set still has a record of all the file descriptors of interest.</li>
<li>To make everything properly asynchronous, you need to disable blocking for the listening socket. Use fcntl to do this.</li>
</ul>
</li>
<li>Call select in a loop after all this setup is done. If everything is done correctly, you should be able to see your program exit the select call without error. If you check the contents of the “read”, you should see that the listening socket is still there. This is easier to do in gdb than with print statements (you should be using gdb anyway).</li>
<li>Now you can start handling file descriptors. After select returns, scan through all the possible file descriptors and check if it is set in the “read” set. If so, then there is an additional check: is it the listening socket, or is it a client socket?</li>
<li>If it is the listening socket, accept the incomming connection and store the new socket file descriptor into an unused client_state. Don’t forget to set this socket to non-blocking, add it to the “all” set, and update the highest file descriptor number you have seen so far. Now you can return to the start of the loop and select will filter-in this socket.</li>
<li>If it is not the listening socket, then it must be one of the clients. Find the client_state for this socket in your client state data structure, and check which handshake to process, calling the appropriate handling function.</li>
<li>Be sure to cleanup and reset everything after the second handshake.</li>
<li>Test your asynchronous server by running a client. You should see all the handshakes print as expected.</li>
<li>Further test your asynchronous server by running several clients back to back, sequentially. You should see each set of clients print the appropriate messages, in order.</li>
<li>Stress test your asynchronous server by running several clients concurrently. The messages may print out of order due to interleaving. See the Testing Interleaving section below.</li>
</ol>
<h2><a name="_Toc21862"></a>1.3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Submission</h2>
<ul>
<li>Your solution MUST compile when running make clean followed by make. Please do check this before submitting. Submissions that fail to compile will receive a 0.</li>
<li>You MUST submit all source and header files, and the makefile, in a tarball (.tar.gz) to the Gradescope assignment CIT 5950 Project 3c.</li>
<li>Your tarball SHOULD NOT contain compiled binaries or demo code files. • You have unlimited submissions until the due date specified by the syllabus.</li>
</ul>
<h2><a name="_Toc21863"></a>1.4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Grading</h2>
Project 3c will be marked on five rubric items. The descriptions for these tests are in the The Autograder section.

There is no peer review for this assignment. You will not be marked on code style.

The score at the due date is final. Do note that they do not sync with Canvas immediately; the course staff must manually release them.

<ol>
<li>Static Analysis : 0 points</li>
<li>Proxy Test : 20 points</li>
<li>Load Test : 30 points</li>
<li>Interleaving Clients Test : 30 points</li>
<li>Server Error Checking Test : 20 points</li>
</ol>
Total : 100 points

<h1><a name="_Toc21864"></a>2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Testing Interleaving</h1>
One of the challenges with 3b and 3c is that your code needs to handle client interleaving. For example, the server may get the first message from ClientA, followed by ClientB and then ClientC. However, the second message from ClientB might arrive at the server before ClientA or ClientC. The autograder will create this interleaving by using a custom tcpclient. The information below will show you how to set up your client and server code to test this interleaving before you submit to the autograder.

<ol>
<li>Run our concurrent request Python code</li>
</ol>
A python script has been provided with the sample code. To use this script, start your server, then run:

python3 ./concurrent-requests.py <em>portNumber</em>

where <em>portNumber </em>is the port used for the server.

This script will run your client program 100 times. The script should complete without errors and the server should still be running. If either program crashes, then there is likely an error in with thread handling (3b) or file descriptor management (3c). While this script will highlight major issues, it does not confirm that the server printed out all of the handshakes correctly. You can add counters for each handshake and print out the result. If both numbers are 100, your code is basically working and then you can test the interleaving.

<ol start="2">
<li>Introduce delays to your TCP client code to test your implementation</li>
</ol>
To create the interleaving, you need to add code to your TCP client. The example code provided below will result in a random delay (up to 100 msec) before the second message is sent from the client. You can do something similar to add a random delay between the connect and first message. The details of the code are in the comments. This delay will result in the server receiving the second message in a different client order than the first message. The script should exit without errors, the server should still be running, and the number of first and second handshakes should be 100. If you have questions about this testing, post on the course discussion forum or attend an office hour.

When you are ready to submit your code to the autograder, remove any extra print statements (such as printing out the number of handshake calls).

<ol start="3">
<li>Client Delay Code</li>
</ol>
Add the following include statement at the top of your code with the other include statements:

// Need to get timestamp to seed random number

#include &lt;sys/time.h&gt;

Add the following code just before the client sends the second message to the server:

<table width="634">
<tbody>
<tr>
<td width="634">// Extra code to create client interleaving;

// timestamp is only used to seed srand() so that each client sleeps

// a different time struct timeval timestamp; gettimeofday(&amp;timestamp, NULL); // get current timestamp

// use usec part of timestamp to seed random numbers;

// cannot use seconds because clients spawn too quickly to cause

// a variation in the time

srand((int)timestamp.tv_usec);

// get a random number between 0 and 99 int ranSleep_ms = (rand() % 100);

// usleep takes number of usec, mult by 1000 to get ms usleep(1000 * ranSleep_ms);

// Code to send the second message to the server should be here…
</td>
</tr>
</tbody>
</table>
&nbsp;

&nbsp;
