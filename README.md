# cse330-homework-3-implementing-semaphores-solved
**TO GET THIS SOLUTION VISIT:** [CSE330 Homework 3-Implementing Semaphores Solved](https://www.ankitcodinghub.com/product/cse330-homework-3-implementing-semaphores-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;59943&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE330 Homework 3-Implementing Semaphores Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
Using the threads, you have implemented, implement semaphores. Since the threads are non-preemptive, you do not need to ensure atomicity of the semaphores (they are already atomic).

Implement the following: (you can either create file called sem.h or write it in your main c file)

<ol>
<li><strong>Semaphore data structure: </strong>A value field and a queue of TCBs.</li>
<li><strong>InitSem(semaphore, value): </strong>Initializes the value field with the specified value.</li>
<li><strong>P(semaphore): </strong>The P routine decrements the semaphore, and if the value is 0 or less than zero then blocks the process in the queue associated with the semaphore.</li>
<li><strong>V(semaphore): </strong>The V routine increments the semaphore, and if the value is 0 or negative, then takes a PCB out of the semaphore queue and puts it into the run queue. Note: <strong>The V routine also “<em><u>yields</u></em>” to the next runnable process.</strong> //this is important.</li>
<li>Implement a solution to the Producer Consumer Problem with the following settings: <em><u>There are P producers all in while loops that loop N times, each producing 1 item in one loop</u>. </em></li>
</ol>
<em><u>There are C consumers all in while loops that loop N times each consuming 1 item in one loop</u></em><em>. </em>

<em><u>Every consumer or producer yields at the end of a loop to the next process</u></em><em>.</em>

&nbsp;

<em><u>Consider that the buffer size is B items.</u></em>

<em><u>You will be given a Queue of numbers, where positive numbers denote the producer ID and negative numbers denote consumer ID</u></em>

<em><u>Arrange your ready queue accordingly</u></em>

<em><u>Start with the first thread in the queue and run it.</u></em>

<em><u>At the end of each loop before yield a consumer should print the following: if consumer X is consuming an item then print</u></em>

<em><u>printf”\n Consumer %d is consuming item generated by Producer %d”,X,Y) else print</u></em>

<em><u>printf(“\n Consumer %d is waiting\n”,X)</u></em>

<em><u>At the end of each loop before yield the producer should print the following:</u></em>

<em><u>if producer X is producing an item then print</u></em>

<em><u>printf(“Producer %d is producing item number %d”, X,Y)</u></em>

<em><u>else print</u></em>

<em><u>printf(“\n Producer %d is waiting \n”, X)</u></em>

<em><u>&nbsp;</u></em>

<strong>How will you implement P(S) and V(S)?</strong>

<strong>&nbsp;</strong>

P(S) requires two operations: a) block when S&lt;= 0 and b) let go when S &gt; 0;

&nbsp;

The task (b) is easy as nothing needs to be done except for decrementing the semaphore value.

&nbsp;

To perform task (a) for every semaphore you declare you have to create a new queue semQ. Whenever a thread executed P(S) and S &lt;= 0 the TCB of the thread gets deleted from the ReadyQ and inserted at the <strong>end</strong> of the semQ. Then the process calls yield(). In this way if the thread remains in the semQ it never gets executed again.

&nbsp;

V(S) requires two operations a) increment S and b) unblock <strong>one</strong> process. To unblock a process, you will deleted the <strong>head</strong> of semQ and add at the <strong>end</strong> of the ReadyQ. This way the processes can perform yield and the unblocked process will execute again.

&nbsp;

<strong>Test cases</strong>

<strong>&nbsp;</strong>

Similar to project 1, we will test your code using input redirection. The first line of each test case file will be of the form:

&nbsp;

B,P,C,N

&nbsp;

Where B is the buffer size, P is the number of producers, C is the number of consumers, and N is the number of times producers and consumers run their while loop. (Note all producers and consumers run the same number of while loop).

&nbsp;

This line will be followed by P+C numbers (one number in each line). Each number denotes process ID. Positive numbers indicate producer process ID, while negative numbers indicate consumer process ID.

&nbsp;

Example test case

2,3,1,2

1

-1

2

3

&nbsp;

Example test case output

&nbsp;

For this particular test case we have buffer size 2, 3 producers and 1 consumer, and each producer or consumer executes their while loops 2 times.

We have two semaphores here: a) Full (for the Consumer) and b) Empty (for the Producer).

&nbsp;

Initially the ready queue looks like the following

&nbsp;

ReadyQ à 1 -1 2 3

&nbsp;

Our Buffer is initially empty

&nbsp;

The Full and Empty queues remain empty

&nbsp;

The first producer produces an item and prints

&nbsp;

<em>Producer 1 is producing item number 1</em>

&nbsp;

After this print the producer yields so the new ready queue looks like the following

&nbsp;

ReadyQ à -1 2 3 1

&nbsp;

Buffer à <u>P1</u>&nbsp; <u>__</u>

&nbsp;

The first consumer then executes and prints

&nbsp;

<em>Consumer 1 is consuming item generated by Producer 1</em>

&nbsp;

The ready queue now looks like the following

&nbsp;

ReadyQ à 2 3 1 -1

&nbsp;

Buffer à __&nbsp;&nbsp;&nbsp; __

&nbsp;

The second producer then executes.

&nbsp;

<em>Producer 2 is producing item number 1</em>

&nbsp;

Then it yields

&nbsp;

ReadyQ à 3 1 -1 2

&nbsp;

Buffer à <u>P2</u>&nbsp;&nbsp;&nbsp; <u>__</u>

&nbsp;

Producer 3 then executes

&nbsp;

<em>Producer 3 is producing item number 1</em>

&nbsp;

ReadyQ à 1 -1 2 3

&nbsp;

Buffer à <u>P2</u>&nbsp; <u>P3</u>

Producer 1 then attempts to produce but the buffer is full so has to wait

&nbsp;

<em>Producer 1 is waiting</em>

&nbsp;

EmptyQ à P1

&nbsp;

ReadyQ à -1 2 3

&nbsp;

Consumer 1 then executes. It unblocks P1 from empty queue and hence P1 joins the end of the ready queue. It then prints:

&nbsp;

<em>Consumer 1 is consuming item generated by Producer 2</em>

&nbsp;

After printing it exits because it is done.

&nbsp;

EmptyQ à empty

&nbsp;

ReadyQ à 2 3 1

&nbsp;

Buffer à <u>P3</u>&nbsp; __

&nbsp;

Process P2 executes

&nbsp;

<em>Producer 2 is producing item number 2</em>

<em>&nbsp;</em>

Then producer 2 is done so it exits

ReadyQ à 3&nbsp; 1

Buffer à <u>P3</u>&nbsp; <u>P2</u>

<u>&nbsp;</u>

Producer 3 then executes but is blocked because buffer is full

&nbsp;

<em>Producer 3 is waiting</em>

&nbsp;

EmptyQ à P3

&nbsp;

ReadyQ à 1

&nbsp;

Producer 1 then executes

&nbsp;

Producer 1 is waiting

&nbsp;

The Ready Q is empty so

&nbsp;

The program ends

&nbsp;

SO overall output is as follows

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

Producer 1 is producing item number 1

&nbsp;

Consumer 1 is consuming item generated by Producer 1

&nbsp;

Producer 2 is producing item number 1

&nbsp;

Producer 3 is producing item number 1

&nbsp;

Producer 1 is waiting

&nbsp;

Consumer 1 is consuming item generated by Producer 2

&nbsp;

Producer 2 is producing item number 2

&nbsp;

Producer 3 is waiting

&nbsp;

Producer 1 is waiting

&nbsp;

&nbsp;

&nbsp;
