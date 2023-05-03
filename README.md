Download Link: https://assignmentchef.com/product/solved-cs342-lab-1
<br>
<strong>Q1.</strong>The Internet <strong>Ping</strong> command bounces a small packet(s) to test network communications, and then shows how long this packet(s) took to make the round trip. The Internet Ping program works much like a sonar echolocation, sending a small packet of information containing an ICMP ECHO_REQUEST to a specified computer, which then sends an ECHO_REPLY packet in return. Explore more about the <em>ping </em>command and answer the following questions (Unix or GNU/Linux version only):

<ol>

 <li>What is the option required to specify the number of echo requests to send with <em>ping </em>command<em>? </em></li>

 <li>What is the option required to set time interval (in seconds), rather than the default one second interval, between two successive <em>ping</em></li>

</ol>

ECHO_REQUESTs?

<ol>

 <li>What is the command to send ECHO_REQUEST packets to the destination one after another without waiting for a reply? What is the limit for sending such ECHO_REQUEST packets by normal users (not superuser)?</li>

 <li>What is the command to set the ECHO_REQUEST payload/data size (in bytes)? If the payload size is set to 32 bytes, what will be the total packet size?</li>

</ol>

<strong>Q2. </strong>Select six hosts of your choice in the Internet (mention the list in your report) and experiment with pinging each host 25 times at three different hours of the day. You can use the following online tools for this experiment:

<ol>

 <li><a href="http://www.spfld.com/ping.html">http://www.spfld.com/ping.html</a></li>

 <li><u>https: </u><a href="http://www.subnetonline.com/pages/network-tools/online-ping-ipv4.php">//w</a><a href="http://www.subnetonline.com/pages/network-tools/online-ping-ipv4.php">  </a><a href="http://www.subnetonline.com/pages/network-tools/online-ping-ipv4.php">w</a><u>w </u><a href="http://www.subnetonline.com/pages/network-tools/online-ping-ipv4.php"> </a><a href="http://www.subnetonline.com/pages/network-tools/online-ping-ipv4.php">.subnetonline.com/pages/network-tools/online-ping-</a> <a href="http://www.subnetonline.com/pages/network-tools/online-ping-ipv4.php">php</a></li>

 <li>List out the average RTT for each host in tabular form, and explain whether RTT has a correlation with the geographical distance of the destinations from source</li>

 <li>Check if in any case, packet loss is greater than 0% and provide reason for the same</li>

 <li>Pick one of the above used hosts, and repeat the experiment with different packet sizes ranging from 64 bytes to 2048 bytes. Plot average RTT vs packet size.</li>

 <li>Explain how change in packet size, and time of the day impact RTT.</li>

</ol>

<strong>Q3. </strong>Select an IP address of your choice (mention the  address in your report) and capture the outcome of 1,000 pings in two separate files by executing the following <em>ping </em>commands.

<ul>

 <li>ping -n &lt;IPAddress&gt;</li>

 <li>ping -p ff00 &lt;IPAddress&gt;</li>

</ul>

Come up with a method to read and analyze the observations captured in the files and answer the following questions. You are free to look for a tool, programming/scripting language that is best suitable for the task and learn just enough of it to get the analysis done.

<ol>

 <li>What was the packet loss rate for each command?</li>

 <li>What was the minimum, maximum, mean, and median latency of the pings that succeeded? Ignore pings that failed in the calculation.</li>

 <li>Give plot to show the normal distribution of the ping latency.</li>

 <li>The two experiments are almost similar except in few aspects. Describe the significant network behavior difference (if any) you observed between the two experiments.</li>

</ol>

<strong>Q4.</strong>With regard to <strong><em>ifconfig</em></strong> and <strong><em>route</em></strong> commands, answer the following questions:

<ol>

 <li>Run <em>ifconfig </em>command and briefly describe its output (important attributes).</li>

 <li>What options can be provided with the <em>ifconfig </em>command? Mention and explain at least four options.</li>

 <li>Explain the output of <em>route command. </em><strong>(1)</strong></li>

 <li>Mention and explain at least four options of the <em>route </em> Execute the <em>route </em>command with these four options and show the output. <strong>(1)</strong></li>

</ol>

<strong>Total marks: 5</strong>

<strong>Q5.</strong>Answer the following questions related to <strong><em>netstat</em></strong> command.

<ol>

 <li>What is the command <em>netstat </em>used for? <strong>(1)</strong></li>

 <li>What parameters for <em>netstat </em>should you use to show the established TCP connections? Include a screenshot of the command and output <strong>(1)</strong></li>

 <li>What does “<em>netstat –r</em>” show? Explain all the fields of the output. <strong>(1)</strong></li>

 <li>What option of <em>netstat </em>can be used to display the status of all network interfaces? By using <em>netstat</em>, figure out the number of interfaces on your computer. <strong>(1)</strong></li>

 <li>What option of <em>netstat </em>can be used to show the statistics of all UDP connections? Run the command on your computer and show the output.</li>

</ol>

<strong>(1)</strong>

<ol>

 <li>Show and explain the function of loop-back interface. <strong>(1) Total marks: 6</strong></li>

</ol>

<strong>Q6.</strong>Perform a <strong>traceroute</strong> experiment (with same hosts used in <strong>Q2</strong>) at three different hours of the day, and then answer the questions below. Use any one of the following online tools for this experiment:

<ul>

 <li>http://ping.eu;</li>

 <li><a href="http://www.cogentco.com/en/network/looking-glass%3B">http://www.cogentco.com/en/network/looking-glass;</a></li>

 <li>https:<a href="http://www.ultratools.com/tools/traceRoute%3B">//ww</a>w<a href="http://www.ultratools.com/tools/traceRoute%3B">.ultratools.com/tools/traceRoute; </a> <a href="https://network-tools.com/">http://network-tools.com</a> <a href="https://network-tools.com/">;</a></li>

</ul>

<ol>

 <li>What is the use of traceroute tool? <strong>(1)</strong></li>

 <li>List out the hop counts for each host in each time slot. Determine the common hops between two routes if they exist. <strong>(1)</strong></li>

 <li>Check and explain the reason, if route to same host changes at different times of the day. <strong>(1)</strong></li>

 <li>Inspect the cases when traceroute does not find complete paths to some hosts, and explain the reasons. <strong>(2)</strong></li>

 <li>Is it possible to find the route to certain hosts which fail to respond with ping experiment? Give reasoning. <strong>(2) Total marks: 7</strong></li>

</ol>

<strong>Q7.</strong>Answer the following questions regarding <strong>ARP</strong>.

<ol>

 <li>How do you see the full ARP table on your machine? Explain eachcolumn of the ARP table. <strong>(2)</strong></li>

 <li>What command is used to add or delete an entry into the ARP table. Use this mechanism to add at least two new hosts to the ARP table and include a screenshot.<strong> (1)</strong></li>

 <li>Can there be an entry for any IP from different subnet in the ARP table of your</li>

</ol>

PC? Explain your answer. <strong>(2)</strong>

<ol>

 <li>Check and report what happens when you forcefully replace (using delete, add command of arp) the Ethernet address of an existing entry with the Ethernet address of another existing entry of the ARP table in your PC, and send ping to those IPs. Explain the behavior. <strong>(1+2) Total marks: 8</strong></li>

</ol>

<strong>Q8. </strong>Install network tool <strong>nmap </strong>in your PC and perform the following experiments:

<ol>

 <li>What is the command to check which PCs of your sub-net are up? <strong>(0.5)</strong></li>

 <li>How to detect firewall settings of your own PC using nmap? <strong>(0.5)</strong></li>

 <li>Run the command of question (a) at least 6 different times of a day, and find the number of hosts online. Plot the number of on PCs vs time, to see if there is an hourly trend for when computers are switched ON or OFF in your LAN. <strong>(1) Total marks: 2</strong></li>

</ol>