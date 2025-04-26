# cop4600-ex7-pipes-solved
**TO GET THIS SOLUTION VISIT:** [COP4600  Ex7-Pipes Solved](https://www.ankitcodinghub.com/product/cop4600-ex7-pipes-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;77852&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COP4600 &nbsp;Ex7-Pipes Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (1 vote)    </div>
    </div>
The aim of this exercise is to familiarize you with pipes in Linux. Pipes are a common form of interprocess communication. <strong>Structure </strong>

The assignment is broken into three main parts. In each part, you will learn about a different way to implement pipes. The three parts are as follows:

<ol>
<li>Basic Pipes</li>
<li>Named Pipes</li>
<li>Pipe System Call</li>
</ol>
<h2>Basic Pipes</h2>
Basic pipes can be created in the terminal by placing the “|” operator between commands. Using “|” causes the output of the left command to be piped in as the input to the right command. For example, running “cat result.txt | grep -o “COP4600″ | wc -l” would return the number of times that the pattern “COP4600” is found in result.txt. The contents of the file are being piped into the grep command which then passed any matches into the wc command. The “wc -l” option returns the number of newlines which, in this case, equals the number of occurrences of the pattern.

For this part, an executable file named “part1.o” is provided via Canvas. When run, the executable will perform basic operations until it encounters a failure. The amount of successful operations completed before failing will vary. Here is a sample output of this program:

Your task is to create a C++ program that, when the output of “part1.o” is piped in, determines which operation number caused the failure. For example, your program would print “Program failed on operation 12” if it were run with the information from the above screenshot. For this part you will need to submit a screenshot that shows your code successfully running twice with input provided by “part1.o” through a basic pipe.

<h2>Named Pipes</h2>
Named pipes, also known as FIFOs (first-in first-out), are functionally similar to basic pipes except they are represented as a special file and are, therefore, a non-temporary part of the filesystem. A FIFO can be created using the “mkfifo [name]” command (similar to mkdir). A FIFO does not store the communicated data in the file system and only acts as a reference point for processes to establish a connection. Because of this, when a writer process opens the FIFO, it will block until a reader process opens the other end. Utilizing named pipes through the command line, therefore, will likely require multiple terminal windows.

For this part, implement the following:

<ol>
<li>Create a named pipe.</li>
<li>Modify your part 1 C++ code to read its input from a file (your named pipe). This program should be named “lastname_part2.cpp” where “lastname” is your last name.</li>
<li>Run “part1.o” and redirect its output into the named pipe.</li>
<li>Compile and run your part 2 program (input <strong>should not</strong> be redirected from the command line).</li>
<li>Repeat steps 3 and 4 then take a screenshot that shows the programs running to completion twice. Be sure to include all terminal windows that were used.</li>
</ol>
<h2>Pipe System Call</h2>
Both piping methods used above have required some form of post-compile time actions (i.e. redirecting output or creating a named pipe). In many cases, this may be a drawback. To set up a pipe entirely within the process’ code, the pipe system call can be used.

For this part you will use the “fork()” and “pipe()” system calls to implement the following:

<ol>
<li>Create a new C++ program named “lastname_part3.cpp” where “lastname” is your last name. The program should accept 5 command-line arguments (all integers).</li>
<li>The program should create two new child processes and utilize four pipes.</li>
<li>The parent process will send the 5 integers to the first child process using a pipe. This child will sort the integers and send the result to the parent process and the second child process using one pipe for each. The parent will print the result.</li>
<li>After receiving the sorted list from the first child process, the second child process will identify the median value of the list and send the result to the parent using a pipe. The parent will print the result.</li>
<li>Take a screenshot of the program running with the following integers passed in as command-line arguments (in the specified order): 42, 15, 8, 16, and 23.</li>
</ol>
