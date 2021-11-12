<html lang="en"><head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
    <link rel="stylesheet" href="https://unpkg.com/@highlightjs/cdn-assets@10.7.1/styles/default.min.css">
<!--   <style></style><style type="text/css">/* this file is used for labs on cognitiveclass.ai that were written in markdown */

/* applies to images, i.e. "![]()" in markdown */
img {
  max-width: 100%;
  height: auto;
}

/* add padding and margins */
body {
  padding: 10px;
  margin: 10px;
}

/* applies to tables, i.e. "|--|--|" in markdown */
table td,
table th {
  padding: 0.75rem;
  vertical-align: top;
  border-top: 1px solid #dee2e6;
}

/* applies to using quotes, i.e. ">" in markdown */
blockquote {
  background: #f9f9f9;
  border-left: 10px solid #ccc;
  margin: 1.5em 10px;
  padding: 1em 10px 0.1em 10px;
  quotes: '\201C''\201D''\2018''\2019';
}

/* the headers need some spacing */

h1,
h2,
h3,
h4,
h5,
h6 {
  font-weight: 500;
  padding-top: 20px;
}

/* Add padding between nested list item */
ul > li > ul {
  padding-bottom: 1rem;
}

.code-badge-language {
  display: none;
}
.code-badge-copy-icon {
  background: url('data:image/svg+xml;base64,PHN2ZyBhcmlhLWhpZGRlbj0idHJ1ZSIgZm9jdXNhYmxlPSJmYWxzZSIgZGF0YS1wcmVmaXg9ImZhciIgZGF0YS1pY29uPSJjb3B5IiBjbGFzcz0ic3ZnLWlubGluZS0tZmEgZmEtY29weSBmYS13LTE0IiByb2xlPSJpbWciIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgdmlld0JveD0iMCAwIDQ0OCA1MTIiPjxwYXRoIGZpbGw9ImN1cnJlbnRDb2xvciIgZD0iTTQzMy45NDEgNjUuOTQxbC01MS44ODItNTEuODgyQTQ4IDQ4IDAgMCAwIDM0OC4xMTggMEgxNzZjLTI2LjUxIDAtNDggMjEuNDktNDggNDh2NDhINDhjLTI2LjUxIDAtNDggMjEuNDktNDggNDh2MzIwYzAgMjYuNTEgMjEuNDkgNDggNDggNDhoMjI0YzI2LjUxIDAgNDgtMjEuNDkgNDgtNDh2LTQ4aDgwYzI2LjUxIDAgNDgtMjEuNDkgNDgtNDhWOTkuODgyYTQ4IDQ4IDAgMCAwLTE0LjA1OS0zMy45NDF6TTI2NiA0NjRINTRhNiA2IDAgMCAxLTYtNlYxNTBhNiA2IDAgMCAxIDYtNmg3NHYyMjRjMCAyNi41MSAyMS40OSA0OCA0OCA0OGg5NnY0MmE2IDYgMCAwIDEtNiA2em0xMjgtOTZIMTgyYTYgNiAwIDAgMS02LTZWNTRhNiA2IDAgMCAxIDYtNmgxMDZ2ODhjMCAxMy4yNTUgMTAuNzQ1IDI0IDI0IDI0aDg4djIwMmE2IDYgMCAwIDEtNiA2em02LTI1NmgtNjRWNDhoOS42MzJjMS41OTEgMCAzLjExNy42MzIgNC4yNDMgMS43NTdsNDguMzY4IDQ4LjM2OGE2IDYgMCAwIDEgMS43NTcgNC4yNDNWMTEyeiI+PC9wYXRoPjwvc3ZnPg==');
  background-size: 100% 100%;
}

.code-badge {
  bottom: 0 !important;
  top: unset !important;
  background: unset !important;
}

.code-badge > .code-badge-check-icon {
  background: green;
}
.code-badge-check-icon {
  font-size: 1.2em;
  cursor: pointer;
  padding: 0 7px;
  background: url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGFyaWEtaGlkZGVuPSJ0cnVlIiBmb2N1c2FibGU9ImZhbHNlIiBkYXRhLXByZWZpeD0iZmFzIiBkYXRhLWljb249ImNoZWNrIiBjbGFzcz0ic3ZnLWlubGluZS0tZmEgZmEtY2hlY2sgZmEtdy0xNiIgcm9sZT0iaW1nIiB2aWV3Qm94PSIwIDAgNTEyIDUxMiIgc3R5bGU9IiYjMTA7ICAgIGNvbG9yOiAjMmFmZjMyOyYjMTA7Ij48cGF0aCBmaWxsPSJjdXJyZW50Q29sb3IiIGQ9Ik0xNzMuODk4IDQzOS40MDRsLTE2Ni40LTE2Ni40Yy05Ljk5Ny05Ljk5Ny05Ljk5Ny0yNi4yMDYgMC0zNi4yMDRsMzYuMjAzLTM2LjIwNGM5Ljk5Ny05Ljk5OCAyNi4yMDctOS45OTggMzYuMjA0IDBMMTkyIDMxMi42OSA0MzIuMDk1IDcyLjU5NmM5Ljk5Ny05Ljk5NyAyNi4yMDctOS45OTcgMzYuMjA0IDBsMzYuMjAzIDM2LjIwNGM5Ljk5NyA5Ljk5NyA5Ljk5NyAyNi4yMDYgMCAzNi4yMDRsLTI5NC40IDI5NC40MDFjLTkuOTk4IDkuOTk3LTI2LjIwNyA5Ljk5Ny0zNi4yMDQtLjAwMXoiLz48L3N2Zz4=');
  background-size: 100% 100%;
}
</style> -->
    </head>
  <body>
    <center>
      <img src="https://gitlab.com/ibm/skills-network/courses/placeholder101/-/raw/master/labs/module%201/images/IDSNlogo.png" width="300" alt="cognitiveclass.ai logo">
    </center>
    <h1>Hands-on Lab: Common Linux/Unix commands</h1>
    <p>Estimated time needed: <strong>40</strong> minutes</p>
    <h2>Objectives</h2>
    <p>In this lab, you will be introducted to the use basic Unix commands related to the following categories:</p>
    <ul>
      <li>General purpose commands.</li>
      <li>Directory management commands.</li>
      <li>File management commands.</li>
      <li>Access control commands.</li>
      <li>Text processing commands.</li>
      <li>Networking commands.</li>
    </ul>
    <h1>About Skills Network Cloud IDE</h1>
    <p>Skills Network Cloud IDE (based on Theia and Docker) provides an environment for hands on labs for course and project related labs. Theia is an open source IDE (Integrated Development Environment), that can be run on desktop or on the cloud. to complete this lab, we will be using the Cloud IDE based on Theia.</p>
    <h2>Important Notice about this lab environment</h2>
    <p>Please be aware that sessions for this lab environment are not persisted. Every time you connect to this lab, a new environment is created for you. Any data or files you may have saved in the earlier session would get lost. Plan to complete these labs in a single session, to avoid losing your data.</p>
    <h1>Exercise 1 - General purpose commands</h1>
    <p>Open a new terminal, by clicking on the menu bar and selecting <strong>Terminal</strong>-&gt;<strong>New Terminal</strong>, as in the image below.</p>
    <p>
      <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-LX0117EN-SkillsNetwork/labs/Bash%20Scripting/Lab%20-%20Linux%20Commands/images/new-terminal.png" alt="">
    </p>
    <p>This will open a new terminal at the bottom of the screen as in the image below.</p>
    <p>
      <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-LX0117EN-SkillsNetwork/labs/Bash%20Scripting/Lab%20-%20Linux%20Commands/images/terminal_bottom_screen.png" alt="">
    </p>
    <p>Run the commands below on the newly opened terminal. (You can copy the code by clicking on the little copy button on the bottom right of the codeblock below and then paste it, wherever you wish.)</p>
    <p><strong>1.1. Display the name of the current user</strong></p>
    <p><strong>whoami</strong></p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">whoami</span>
</code></pre>
    <p></p>
    <p>It will display the user name as <code>theia</code>. You are logged into this lab as <code>theia</code>.</p>
    <p>You can get a list of currently logged in users using the command '<strong>who</strong>'. But this command doesn't work in <em>theia</em> environment yet.</p>
    <p><strong>1.2. Know the user and group identity information</strong><br></p>
    <p><strong>id</strong></p>
    <p>This command displays the user id and group id information of the current user.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">applescript</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-applescript"><span class="hljs-built_in">id</span>
</code></pre>
    <p></p>
    <p>It will display the uid(user id) and gid(group id) for the user <code>theia</code>.</p>
    <p><strong>1.3. Display date and time</strong></p>
    <p><strong>date</strong></p>
    <p>The date command displays current date and time.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">applescript</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-applescript"><span class="hljs-built_in">date</span>
</code></pre>
    <p></p>
    <p>It has several options which help you get date in your favourite format.<br>The following command displays current date in mm/dd/yy format.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">applescript</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-applescript"><span class="hljs-built_in">date</span> <span class="hljs-string">"+%D"</span>
</code></pre>
    <p></p>
    <p>Here are some of the popular format specifiers that you can try out.</p>
    <table>
      <thead>
        <tr>
          <th>Specifier</th>
          <th>Explaination</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>%d</td>
          <td>Display the day of the month (01 to 31)</td>
        </tr>
        <tr>
          <td>%h</td>
          <td>Displays abbreviated month name (Jan to Dec)</td>
        </tr>
        <tr>
          <td>%m</td>
          <td>Displays the month of year (01 to 12)</td>
        </tr>
        <tr>
          <td>%Y</td>
          <td>Display four-digit year</td>
        </tr>
        <tr>
          <td>%T</td>
          <td>Display the time in 24 hour format as HH:MM:SS</td>
        </tr>
        <tr>
          <td>%H</td>
          <td>Display the hour</td>
        </tr>
      </tbody>
    </table>
    <p><strong>1.4. List the files and directories</strong></p>
    <p><strong>ls</strong></p>
    <p>List the files and directories in the current directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls</span>
</code></pre>
    <p></p>
    <p>You many not get any output if your directory is empty.</p>
    <p>The following command will list all the files in the <code>/bin</code> directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">jboss-cli</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-jboss-cli"><span class="hljs-keyword">ls</span> <span class="hljs-string">/bin</span>
</code></pre>
    <p></p>
    <p>List all files starting with <code>b</code> in the <code>/bin</code> directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">ls <span class="hljs-regexp">/bin/</span>b*
</code></pre>
    <p></p>
    <p>List all files ending with <code>r</code> in the <code>/bin</code> directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">ls <span class="hljs-regexp">/bin/</span>*r
</code></pre>
    <p></p>
    <p><strong>1.5. Get basic information about the operating system</strong></p>
    <p><strong>uname</strong></p>
    <p>By default the command prints the kernel name.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">uname</span>
</code></pre>
    <p></p>
    <p>You will see <code>Linux</code> printed in the output.</p>
    <p>Using the <strong>-a</strong> opton prints all the system information in the following order: Kernel name, network node hostname, kernel release date, kernel version, machine hardware name, hardware platform, operating system.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">css</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-css">uname -<span class="hljs-selector-tag"><span class="hljs-selector-tag">a</span></span>
</code></pre>
    <p></p>
    <p><strong>1.6. Get information about active processes</strong></p>
    <p><strong>ps</strong></p>
    <p>ps lists the processes that are currently running and their PIDs (process ids).</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ps</span>
</code></pre>
    <p></p>
    <p>The output contains the processes that are owned by you.</p>
    <p>The <strong>-e</strong> option displays all the processes running on the system. The includes processes owned by other users also.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ps -e</span>
</code></pre>
    <p></p>
    <p><strong>1.7. Get information on the running processes and system resources</strong></p>
    <p><strong>top</strong></p>
    <p>top command provides a dynamic real-time view of the running system.</p>
    <p>It shows the summary information of the system and the list of processes or threads which are currently managed by the Kernel.</p>
    <p>It gives information related to cpu and memory usage per process.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">coq</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-coq"><span class="hljs-built_in">top</span>
</code></pre>
    <p></p>
    <p>Here is a sample output.</p>
    <p>
      <img src="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-LX0117EN-SkillsNetwork/labs/Bash%20Scripting/Lab%20-%20Linux%20Commands/images/top-command-screenshot.png" alt="">
    </p>
    <p>When started for the first time, you'll be presented with the following elements on the main top screen.</p>
    <ol>
      <li>Summary Area. - shows information like system uptime, number of users, load average, memory usage etc.</li>
      <li>Fields/Columns Header.</li>
      <li>Task Area.</li>
    </ol>
    <p>The output keeps refreshing until you press '<strong>q</strong>' or <strong>Ctrl+c</strong></p>
    <p>If you want to exit automatically after a specified number of repetitions, use the <strong>-n</strong> option as in the following example:</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">apache</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-apache"><span class="hljs-attribute"><span class="hljs-attribute">top</span></span> -n <span class="hljs-number"><span class="hljs-number">10</span></span>
</code></pre>
    <p></p>
    <p>using 'top' we can find out which process is consuming the most resources. You can press the following keys while 'top' is running to sort the list :</p>
    <p>M - sort by memory usage<br>P - sort by CPU usage<br>N - sort by process ID<br>T - sort by the running time<br></p>
    <p><strong>1.8. Display Messages</strong></p>
    <p><strong>echo</strong></p>
    <p>echo command displays the given text on the screen.<br></p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">bash</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-bash"><span class="hljs-built_in"><span class="hljs-built_in">echo</span></span> <span class="hljs-string"><span class="hljs-string">"Welcome to the linux lab"</span></span>
</code></pre>
    <p></p>
    <p>These special characters help you better format your output.<br></p>
    <table>
      <thead>
        <tr>
          <th>Special Character</th>
          <th>Meaning</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>\n</td>
          <td>Represents a newline character</td>
        </tr>
        <tr>
          <td>\t</td>
          <td>A tab character</td>
        </tr>
      </tbody>
    </table>
    <p>Use the <strong>-e</strong> option of the echo command when working with special characters.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">bash</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-bash"><span class="hljs-built_in"><span class="hljs-built_in">echo</span></span> -e <span class="hljs-string"><span class="hljs-string">"This will be printed \nin two lines"</span></span>
</code></pre>
    <p></p>
    <p><strong>1.9. Download a file from the internet.</strong></p>
    <p><strong>wget</strong></p>
    <p>wget command helps you to donwload a file at a given url.</p>
    <p>This command download the file usdoi.txt from the given url.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">wget https:<span class="hljs-regexp">//</span>cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud<span class="hljs-regexp">/IBM-DB0250EN-SkillsNetwork/</span>labs<span class="hljs-regexp">/Bash%20Scripting/u</span>sdoi.txt

</code></pre>
    <p></p>
    <p>Verify using the ls command.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls</span>
</code></pre>
    <p></p>
    <p><strong>1.10. View the Reference Manual</strong></p>
    <p><strong>man</strong></p>
    <p>man command displays the user manual of the command given as argument.</p>
    <p>For example, to see the manual page of 'ls' command, use:</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">powershell</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-powershell"><span class="hljs-built_in">man</span> <span class="hljs-built_in">ls</span>
</code></pre>
    <p></p>
    <h1>Exercise 2 - Directory Management Commands</h1>
    <p><strong>2.1. Print the name of your current working directory.</strong></p>
    <p><strong>pwd</strong></p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">bash</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-bash"><span class="hljs-built_in"><span class="hljs-built_in">pwd</span></span>
</code></pre>
    <p></p>
    <p>This will print <code>/home/project</code>.</p>
    <p><strong>2.2. Create a directory</strong></p>
    <p><strong>mkdir</strong></p>
    <p>mkdir creates a new directory.</p>
    <p>To create a directory named 'scripts' in your current directory, run the following command.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">arduino</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-arduino">mkdir scripts 
</code></pre>
    <p></p>
    <p>Use the <code>ls</code> command to verify if the <code>scripts</code> directories got created.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls</span> 
</code></pre>
    <p></p>
    <p><strong>2.3. Change your current working directory.</strong></p>
    <p><strong>cd</strong></p>
    <p>To get into the directory <code>scripts</code> directory, run the command below .</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">bash</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-bash"><span class="hljs-built_in"><span class="hljs-built_in">cd</span></span> scripts
</code></pre>
    <p></p>
    <p>Use the <code>pwd</code> command to verify if your current working directory has changed.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">bash</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-bash"><span class="hljs-built_in"><span class="hljs-built_in">pwd</span></span>
</code></pre>
    <p></p>
    <p>If you use <strong>cd</strong> without any directory name, it will move you back to your home directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">bash</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-bash"><span class="hljs-built_in"><span class="hljs-built_in">cd</span></span>
</code></pre>
    <p></p>
    <p>Use the <code>pwd</code> command to verify if your current working directory has changed.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">bash</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-bash"><span class="hljs-built_in"><span class="hljs-built_in">pwd</span></span>
</code></pre>
    <p></p>
    <p>Run the command below to move to the parent directory. <code>..</code> is a shortcut that refers to the parent directory of your current directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">gams</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-gams"><span class="hljs-function"><span class="hljs-title">cd</span></span> ..
</code></pre>
    <p></p>
    <p><strong>2.4. Get a list of files in a directory</strong></p>
    <p><strong>ls</strong></p>
    <p>Lists the files in the current directory or the directory given as argument.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls  -l</span>
</code></pre>
    <p></p>
    <p>Prints a long list of files that has additional information compared to the simple <code>ls</code> command.</p>
    <p>Here are some popular options that you can try with the ls command.</p>
    <table>
      <thead>
        <tr>
          <th>Option</th>
          <th>Description</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>-a</td>
          <td>list all the files including hidden files</td>
        </tr>
        <tr>
          <td>-d</td>
          <td>list directories themselves, not their contents</td>
        </tr>
        <tr>
          <td>-h</td>
          <td>with -l and -s, print sizes like 1K, 234M, 2G etc</td>
        </tr>
        <tr>
          <td>-l</td>
          <td>long listing of files which include information about permission, owner, size etc</td>
        </tr>
        <tr>
          <td>-F</td>
          <td>classify files by appending type indcator like *,/ etc. to file names</td>
        </tr>
        <tr>
          <td>-r</td>
          <td>reverse order while sorting</td>
        </tr>
        <tr>
          <td>-S</td>
          <td>sort by file size, largest first</td>
        </tr>
        <tr>
          <td>-t</td>
          <td>sort by time, newest first</td>
        </tr>
      </tbody>
    </table>
    <p>Get a long listing of all files in /etc, including hidden files, if any.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">jboss-cli</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-jboss-cli"><span class="hljs-keyword">ls</span> -la <span class="hljs-string">/etc</span>
</code></pre>
    <p></p>
    <p>To list the files based on modifcation time, use <strong>-t</strong> option.</p>
    <p>The most recently modified file will be on top.</p>
    <p>This is more frequently used with <strong>-l</strong> option.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">powershell</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-powershell"><span class="hljs-built_in">ls</span> <span class="hljs-operator">-lt</span>
</code></pre>
    <p></p>
    <p>To view the current directory attributes instead of their contents, use the following command. If you want any other directory's attributes, provide the directory name as argument.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">jboss-cli</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-jboss-cli"><span class="hljs-keyword">ls</span> -ld <span class="hljs-string">/etc</span>
</code></pre>
    <p></p>
    <p>To list the files sorted by file size in descending order, use <strong>-S</strong> option.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">stata</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-stata"><span class="hljs-keyword">ls</span> -<span class="hljs-keyword">lS</span>
</code></pre>
    <p></p>
    <p>To get the files sorted by file size in ascending order, add <strong>-r</strong> option.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls -lrS</span>
</code></pre>
    <p></p>
    <p><strong>2.5. Delete directory</strong></p>
    <p><strong>rmdir</strong></p>
    <p>rmdir removes a directory.</p>
    <p>Let us create a <code>dummy</code> directory in the the <code>/tmp</code> folder .</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">mkdir <span class="hljs-regexp">/tmp/</span>dummy
</code></pre>
    <p></p>
    <p>Verify by using the <code>ls</code> command.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">jboss-cli</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-jboss-cli"><span class="hljs-keyword">ls</span> <span class="hljs-string">/tmp</span>
</code></pre>
    <p></p>
    <p>Delete the dummy directory</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">rmdir <span class="hljs-regexp">/tmp/</span>dummy
</code></pre>
    <p></p>
    <p>Verify by using the <code>ls</code> command.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">jboss-cli</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-jboss-cli"><span class="hljs-keyword">ls</span> <span class="hljs-string">/tmp</span>
</code></pre>
    <p></p>
    <p>Note: Before removing any directory make sure that you do not have any files or sub directories.</p>
    <p><strong>2.6. Search and locate files</strong></p>
    <p><strong>find</strong></p>
    <p>Find command is used to search for files in a directory. You can search for files based on different categories like file name, file type, owner, size, timestamps etc.<br></p>
    <p>Find command conducts the search in the entire directory tree starting from the directory name given.</p>
    <p>This command finds all txt files in the subfolders of the /etc directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">routeros</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-routeros"><span class="hljs-builtin-name">find</span> /etc -name <span class="hljs-string">'*.txt'</span> 
</code></pre>
    <p></p>
    <p>Along with the listing of txt files, you may get some <code>Permission denied</code> errors.</p>
    <p>That is normal, as you have limited access on the lab machine.</p>
    <p><strong>2.7. Display the amount of disk space available on file systems</strong></p>
    <p><strong>df</strong></p>
    <p>The 'df' command displays the information of device name, total blocks, total disk space, used disk space, available disk space and mount points on a file system.</p>
    <p>Without any arguments, the commands shows the information for all currently mounted file systems.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">df</span>
</code></pre>
    <p></p>
    <p>Use the <strong>-h</strong> option to view the disk space usage in human readable format, i.e, in megabytes, gigabytes etc.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">df -h</span>
</code></pre>
    <p></p>
    <h1>Exercise 3 - File Management Commands</h1>
    <p><strong>3.1. Display file contents</strong></p>
    <p><strong>cat</strong></p>
    <p>cat command displays contents of files.</p>
    <p>The following command prints the content of the file usdoi.txt which you have downloaded earlier.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">cat usdoi</span>.txt
</code></pre>
    <p></p>
    <p>If you get a file not found error, then run these commands.</p>
    <p><code>cd</code> takes you to your home directory.</p>
    <p><code>wget</code> download the file.</p>
    <p><code>cat</code> will print the file onto the screen.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">cd
wget https:<span class="hljs-regexp">//</span>cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud<span class="hljs-regexp">/IBM-DB0250EN-SkillsNetwork/</span>labs<span class="hljs-regexp">/Bash%20Scripting/u</span>sdoi.txt
cat usdoi.txt
</code></pre>
    <p></p>
    <p><strong>3.2. Display file contents page-wise</strong></p>
    <p><strong>more</strong></p>
    <p>The <strong>more</strong> command displays the file contents page by page.</p>
    <p>Press <strong>spacebar</strong> to display the next page.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">dos</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-dos"><span class="hljs-built_in">more</span> usdoi.txt
</code></pre>
    <p></p>
    <p><strong>3.3. Display first few lines of a file</strong></p>
    <p><strong>head</strong></p>
    <p>Print the first 10 lines of the file usdoi.txt.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">head usdoi</span>.txt
</code></pre>
    <p></p>
    <p>You can specify the number of lines to be printed.</p>
    <p>Print the first 3 lines of the file usdoi.txt.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">apache</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-apache"><span class="hljs-attribute"><span class="hljs-attribute">head</span></span> -<span class="hljs-number"><span class="hljs-number">3</span></span> usdoi.txt
</code></pre>
    <p></p>
    <p><strong>3.4. Display last lines of a file</strong></p>
    <p><strong>tail</strong></p>
    <p>Print the last 10 lines of the file usdoi.txt.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">tail usdoi</span>.txt
</code></pre>
    <p></p>
    <p>You can specify the number of lines to be printed.</p>
    <p>Print the last 2 lines of the file usdoi.txt.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">apache</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-apache"><span class="hljs-attribute"><span class="hljs-attribute">tail</span></span> -<span class="hljs-number"><span class="hljs-number">2</span></span> usdoi.txt
</code></pre>
    <p></p>
    <p><strong>3.5. Copy files</strong></p>
    <p><strong>cp</strong></p>
    <p>Copy usdoi.txt into a file named usdoi-backup.txt.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">stylus</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-stylus">cp usdoi<span class="hljs-selector-class">.txt</span> usdoi-backup<span class="hljs-selector-class">.txt</span>
</code></pre>
    <p></p>
    <p>Use <code>ls</code> command to verify if the copy was successful.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls</span>
</code></pre>
    <p></p>
    <p>The command below copies the content of /etc/passwd to a file named 'users.txt' under the current directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">cp <span class="hljs-regexp">/etc/</span>passwd users.txt
</code></pre>
    <p></p>
    <p>Use <code>ls</code> command to verify if the copy was successful.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls</span>
</code></pre>
    <p></p>
    <p><strong>3.6. Move, Rename a file</strong></p>
    <p><strong>mv</strong></p>
    <p>mv command moves a file from one directory to another.</p>
    <p>While moving a file, if the target file is existing, it is overwritten.</p>
    <p>If the source and target directories are same, it works like rename operation.</p>
    <p>Rename <code>users.txt</code> as <code>user-info.txt</code></p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">nginx</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-nginx"><span class="hljs-attribute"><span class="hljs-attribute">mv</span></span> users.txt user-<span class="hljs-literal"><span class="hljs-literal">info</span></span>.txt
</code></pre>
    <p></p>
    <p>Use <code>ls</code> command to verify.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls</span>
</code></pre>
    <p></p>
    <p>Move <code>user-info.txt</code> to the <code>/tmp</code> directory</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">nginx</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-nginx"><span class="hljs-attribute"><span class="hljs-attribute">mv</span></span> user-<span class="hljs-literal"><span class="hljs-literal">info</span></span>.txt /tmp
</code></pre>
    <p></p>
    <p>Use <code>ls</code> command to verify.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls</span>
</code></pre>
    <p></p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">jboss-cli</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-jboss-cli"><span class="hljs-keyword">ls</span> -l <span class="hljs-string">/tmp</span>
</code></pre>
    <p></p>
    <p><strong>3.7. Create a blank file</strong></p>
    <p><strong>touch</strong></p>
    <p>Create an empty file named myfile.txt</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">touch myfile</span>.txt
</code></pre>
    <p></p>
    <p>Use <code>ls</code> command to verify.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls -l</span>
</code></pre>
    <p></p>
    <p>If the file already exists, the touch command updates the access timestamp of the file.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">touch usdoi</span>.txt
</code></pre>
    <p></p>
    <p>Use <code>ls</code> command to verify.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls -l</span>
</code></pre>
    <p></p>
    <p><strong>3.8. Remove files</strong></p>
    <p><strong>rm</strong></p>
    <p>The rm command is ideally used along with the <strong>-i</strong> option, which makes it ask for confirmation before deleting.</p>
    <p>Remove the file <code>myfile.txt</code>. Press y to confirm deletion, or n to cancel</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">stylus</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-stylus">rm -<span class="hljs-selector-tag">i</span> myfile<span class="hljs-selector-class">.txt</span>
</code></pre>
    <p></p>
    <p>Use <code>ls</code> command to verify.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls -l</span>
</code></pre>
    <p></p>
    <p><strong>3.9. Create and manage file archives</strong></p>
    <p><strong>tar</strong></p>
    <p>tar command allows you to copy multiple files and directories into a single archive file.</p>
    <p>The following command creates an archive of the entire '/bin' directory into a file named <code>bin.tar</code>.<br></p>
    <p>The options used are as follows:</p>
    <table>
      <thead>
        <tr>
          <th>Option</th>
          <th>Description.</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>-c</td>
          <td>Create new archive file</td>
        </tr>
        <tr>
          <td>-v</td>
          <td>Verbosely list files processed</td>
        </tr>
        <tr>
          <td>-f</td>
          <td>Archive file name</td>
        </tr>
      </tbody>
    </table>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">mipsasm</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-mipsasm">tar -cvf <span class="hljs-keyword">bin.tar </span>/<span class="hljs-keyword">bin
</span></code></pre>
    <p></p>
    <p>To see the list of files in the archive, use <strong>-t</strong> option:</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">tar -tvf bin</span>.tar
</code></pre>
    <p></p>
    <p>To untar the archive or extract files from the archive, use <strong>-x</strong> option:</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">tar -xvf bin</span>.tar
</code></pre>
    <p></p>
    <p>Use <code>ls</code> command to verify that the folder <code>bin</code> is extracted.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls -l</span>
</code></pre>
    <p></p>
    <p><strong>3.10. Package and compress archive files</strong></p>
    <p><strong>zip</strong></p>
    <p>zip command allows you to compress files.</p>
    <p>The following command creates a zip named config.zip and of all the files with extension <code>.conf</code> in the <code>/etc</code> directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">zip config.zip <span class="hljs-regexp">/etc/</span>*.conf
</code></pre>
    <p></p>
    <p>The <strong>-r</strong> option can be used to zip the entire folder.</p>
    <p>The following command creates an archive of the '/bin' directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">python</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-python"><span class="hljs-built_in"><span class="hljs-built_in">zip</span></span> -r <span class="hljs-built_in"><span class="hljs-built_in">bin</span></span>.<span class="hljs-built_in"><span class="hljs-built_in">zip</span></span> /<span class="hljs-built_in"><span class="hljs-built_in">bin</span></span>
</code></pre>
    <p></p>
    <p><strong>3.11. Extract, list, or test compressed files in a ZIP archive</strong></p>
    <p><strong>unzip</strong></p>
    <p>The following command lists the files of the archive called 'config.zip'</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">arduino</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-arduino">unzip -l config.zip
</code></pre>
    <p></p>
    <p>The following command extracts all the files in the archive bin.zip.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">python</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-python">unzip <span class="hljs-built_in"><span class="hljs-built_in">bin</span></span>.<span class="hljs-built_in"><span class="hljs-built_in">zip</span></span>
</code></pre>
    <p></p>
    <p>You should see a folder named <code>bin</code> created in your directory.</p>
    <h1>Exercise 4 - Access Control Commands</h1>
    <p>Each file/directory has permissions set for the file owner, group owner and others.</p>
    <p>The following permissions are set for each file:</p>
    <table>
      <thead>
        <tr>
          <th>Permission</th>
          <th>symbol</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>read</td>
          <td>r</td>
        </tr>
        <tr>
          <td>write</td>
          <td>w</td>
        </tr>
        <tr>
          <td>execute</td>
          <td>x</td>
        </tr>
      </tbody>
    </table>
    <p>To see the permissions currently set for a file, run <strong>ls -l</strong> command.</p>
    <p>For example, to see the permissions for a file named 'usdoi.txt' in your current directory, run:</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls -l usdoi</span>.txt
</code></pre>
    <p></p>
    <p>A sample output looks like:</p>
    <p>-rw-r--r-- 1 theia theia 8121 May 31 16:45 usdoi.txt</p>
    <p>The permissions set here are 'rw-r--r--'</p>
    <p>Here, owner has read and write permissions, group owner has read permission and others also have read permission.</p>
    <p><strong>4.1 chmod</strong></p>
    <p>chmod command lets you change the permissions set for a file.</p>
    <p>The change of permissions is specified with the help of a combination of the following characters:<br></p>
    <table>
      <thead>
        <tr>
          <th>Option</th>
          <th>Description.</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>r, w and x</td>
          <td>representing read, write and execute permissions respectively</td>
        </tr>
        <tr>
          <td>u,g and o</td>
          <td>representing user categories owner, group and others respectively</td>
        </tr>
        <tr>
          <td>+, -</td>
          <td>representing grant and revoke operations respectively</td>
        </tr>
      </tbody>
    </table>
    <p>The command below removes read permission for all (user,group and other) on usdoi.txt.<br></p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">chmod -r usdoi</span>.txt               
</code></pre>
    <p></p>
    <p>Verify the changed permissions.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls -l usdoi</span>.txt
</code></pre>
    <p></p>
    <p>Add read access to all on usdoi.txt.<br></p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">chmod</span> +r usdoi.txt                
</code></pre>
    <p></p>
    <p>Verify the changed permissions.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls -l usdoi</span>.txt
</code></pre>
    <p></p>
    <p>To remove the read permission for 'others' category.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">chmod o-r usdoi</span>.txt
</code></pre>
    <p></p>
    <p>Verify the changed permissions.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ls -l usdoi</span>.txt
</code></pre>
    <p></p>
    <h1>Exercise 5 - Text Processing Commands</h1>
    <p><strong>5.1. Count lines, words or characters</strong></p>
    <p><strong>wc</strong></p>
    <p>If you want to find the number of lines, words and characters in a file, for example 'usdoi.txt'.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">wc usdoi</span>.txt
</code></pre>
    <p></p>
    <p>The output contains the number of lines followed by number of words followed by number of characters in the file.</p>
    <p>Print only the number of lines in 'usdoi.txt'.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">wc -l usdoi</span>.txt
</code></pre>
    <p></p>
    <p>Print only the number of words in 'usdoi.txt'.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">wc -w usdoi</span>.txt
</code></pre>
    <p></p>
    <p>Print only the number of characters in 'usdoi.txt'.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">wc -c usdoi</span>.txt
</code></pre>
    <p></p>
    <p><strong>5.2. Perform search operations within the text</strong></p>
    <p><strong>grep</strong></p>
    <p>grep command allows you to specify patterns and search for lines matching the pattern, from the input text.</p>
    <p>The following command prints all lines in the file <code>usdoi.txt</code> which contain the word <code>people</code>.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">grep people usdoi</span>.txt
</code></pre>
    <p></p>
    <p>Some of the frequently used options of grep are:</p>
    <table>
      <thead>
        <tr>
          <th>Option</th>
          <th>Description.</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>-n</td>
          <td>Along with the matching lines, print the line numbers also</td>
        </tr>
        <tr>
          <td>-c</td>
          <td>Get the count of matching lines</td>
        </tr>
        <tr>
          <td>-i</td>
          <td>Ignore the case of the text while matching</td>
        </tr>
        <tr>
          <td>-v</td>
          <td>Print all lines which do not contain the pattern</td>
        </tr>
        <tr>
          <td>-w</td>
          <td>Match only if the pattern matches whole words</td>
        </tr>
      </tbody>
    </table>
    <p>Prints all lines from the <code>/etc/passwd</code> file, which do not contain the pattern <code>login</code>.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">gradle</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-gradle"><span class="hljs-keyword">grep</span> -v login <span class="hljs-regexp">/etc/</span>passwd
</code></pre>
    <p></p>
    <h1>Exercise 6 - Networking commands</h1>
    <p><strong>6.1. Show the system's host name</strong></p>
    <p><strong>hostname</strong></p>
    <p>To view the current host name, run the command below .</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">hostname</span>
</code></pre>
    <p></p>
    <p>You can use the <strong>-i</strong> option to view the IP adrress of the host:</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">css</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-css">hostname -<span class="hljs-selector-tag"><span class="hljs-selector-tag">i</span></span>
</code></pre>
    <p></p>
    <p><strong>6.2. Test if a host is reachable</strong></p>
    <p><strong>ping</strong></p>
    <p>Check if <a href="http://www.google.com/?utm_medium=Exinfluencer&amp;utm_source=Exinfluencer&amp;utm_content=000026UJ&amp;utm_term=10006555&amp;utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMLX0117ENSkillsNetwork27653394-2021-01-01" target="_blank" rel="external">www.google.com</a> is reachable. The command keeps sending data packets to the <a href="http://www.google.com/?utm_medium=Exinfluencer&amp;utm_source=Exinfluencer&amp;utm_content=000026UJ&amp;utm_term=10006555&amp;utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMLX0117ENSkillsNetwork27653394-2021-01-01" target="_blank" rel="external">www.google.com</a> server and prints the response it gets back. (Press <strong>Ctrl+C</strong> to stop pinging)</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">stylus</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-stylus">ping www<span class="hljs-selector-class">.google</span><span class="hljs-selector-class">.com</span>
</code></pre>
    <p></p>
    <p>If you want to ping only for a limited number of times, use <strong>-c</strong> option.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">stylus</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-stylus">ping -c <span class="hljs-number">5</span> www<span class="hljs-selector-class">.google</span><span class="hljs-selector-class">.com</span>
</code></pre>
    <p></p>
    <p><strong>6.3. Display network interface configuration</strong></p>
    <p><strong>ifconfig</strong></p>
    <p>Configures or displays network interface parameters for a network.</p>
    <p>Display the configuration of all network interfaces of the system:</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">ebnf</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-ebnf"><span class="hljs-attribute">ifconfig</span>
</code></pre>
    <p></p>
    <p>Display the configuration of the ethernet adapter.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">apache</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-apache"><span class="hljs-attribute"><span class="hljs-attribute">ifconfig</span></span> eth<span class="hljs-number"><span class="hljs-number">0</span></span>
</code></pre>
    <p></p>
    <p>eth0 is usually the primary network interface that connects your server to the network.</p>
    <p>You can see your server's ip address in the line number 2 after the word inet.</p>
    <p><strong>6.4. Transfer data from or to a server</strong></p>
    <p><strong>curl</strong></p>
    <p>Access the file at the given url and display the contents on to the screen.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">curl https:<span class="hljs-regexp">//</span>cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud<span class="hljs-regexp">/IBM-DB0250EN-SkillsNetwork/</span>labs<span class="hljs-regexp">/Bash%20Scripting/u</span>sdoi.txt

</code></pre>
    <p></p>
    <p>Access the file at the given url and save it in the current directory.</p>
    <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">curl -O https:<span class="hljs-regexp">//</span>cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud<span class="hljs-regexp">/IBM-DB0250EN-SkillsNetwork/</span>labs<span class="hljs-regexp">/Bash%20Scripting/u</span>sdoi.txt

</code></pre>
    <p></p>
    <h1>Practice exercises</h1>
    <ol>
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>Display the content of /home directory.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>Use 'ls' command.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">jboss-cli</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-jboss-cli"><span class="hljs-keyword">ls</span> <span class="hljs-string">/home</span>
</code></pre>
      <p></p>
    </details>
    <ol start="2">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>Ensure that you are in your home directory.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>Use 'cd' to move to the home directory and then use 'pwd' to verify'.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">bash</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-bash"><span class="hljs-built_in"><span class="hljs-built_in">cd</span></span>
<span class="hljs-built_in"><span class="hljs-built_in">pwd</span></span>
</code></pre>
      <p></p>
    </details>
    <ol start="3">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>Create a new directory called 'final' in your home directory.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>Use 'mkdir' command.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">arduino</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-arduino">mkdir <span class="hljs-keyword">final</span>
</code></pre>
      <p></p>
    </details>
    <ol start="4">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>View the permissions of the newly created directory 'final'.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>Use -d and -l options of the ls command.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">actionscript</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-actionscript">ls -ld <span class="hljs-keyword">final</span>
</code></pre>
      <p></p>
    </details>
    <ol start="5">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>Create a new blank file named 'display.sh' in the <code>final</code> directory</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>use 'cd and 'touch' commands.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">stata</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-stata"><span class="hljs-keyword">cd</span> final
touch <span class="hljs-keyword">display</span>.<span class="hljs-keyword">sh</span>
</code></pre>
      <p></p>
    </details>
    <ol start="6">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>Copy <code>display.sh</code> as <code>report.sh</code>.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>Use the cp command.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">stata</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-stata">cp <span class="hljs-keyword">display</span>.<span class="hljs-keyword">sh</span> <span class="hljs-keyword">report</span>.<span class="hljs-keyword">sh</span>
</code></pre>
      <p></p>
    </details>
    <ol start="7">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>Delete the file 'display.sh'.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>Use 'rm' command.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">stata</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-stata"><span class="hljs-keyword">rm</span> -i <span class="hljs-keyword">display</span>.<span class="hljs-keyword">sh</span>
</code></pre>
      <p></p>
    </details>
    <ol start="8">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>List the files in /etc directory in the ascending order of their access time.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>Use the ls command with right options.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">jboss-cli</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-jboss-cli"><span class="hljs-keyword">ls</span> -ltr <span class="hljs-string">/etc</span>
</code></pre>
      <p></p>
    </details>
    <ol start="9">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>Display the current time.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>Use the format option '%T' of the date command.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">applescript</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-applescript"><span class="hljs-built_in">date</span> <span class="hljs-string">"+%T"</span>
</code></pre>
      <p></p>
    </details>
    <ol start="10">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>Display the number of lines in the /etc/passwd file.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>use the wc command with right option.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">wc -l <span class="hljs-regexp">/etc/</span>passwd
</code></pre>
      <p></p>
    </details>
    <ol start="11">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em>Display the lines that contain the string 'not installed' in /var/log/bootstrap.log page-wise.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>use the grep and more commands.</p>
      </blockquote>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">stata</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-stata">grep <span class="hljs-string">"not installed"</span> /<span class="hljs-keyword">var</span>/<span class="hljs-keyword">log</span>/<span class="hljs-keyword">bootstrap</span>.<span class="hljs-keyword">log</span> | <span class="hljs-keyword">more</span>
</code></pre>
      <p></p>
    </details>
    <ol start="12">
      <li>Problem:</li>
    </ol>
    <blockquote>
      <p><em><code>https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0250EN-SkillsNetwork/labs/Bash%20Scripting/top-sites.txt</code> contains most popular websites. Find out all the websites that have the word <code>org</code> in them.</em></p>
    </blockquote>
    <details>
      <summary>Click here for Hint</summary>
      <blockquote>
        <p>use the wget command to download the file.</p>
      </blockquote>
      <p>use the grep command to search</p>
    </details>
    <details>
      <summary>Click here for Solution</summary>
      <pre class="code-badge-pre"><div class="code-badge">
        <div class="code-badge-language">awk</div>
        <div title="Copy to clipboard">
            <i class="code-badge-copy-icon code-badge-copy-icon"></i>
        </div>
     </div><code class="hljs language-awk">wget https:<span class="hljs-regexp">//</span>cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud<span class="hljs-regexp">/IBM-DB0250EN-SkillsNetwork/</span>labs<span class="hljs-regexp">/Bash%20Scripting/</span>top-sites.txt
grep org top-sites.txt 
</code></pre>
      <p></p>
    </details>
    <h2>Authors</h2>
    <p>Ramesh Sannareddy</p>
    <h3>Other Contributors</h3>
    <p>Rav Ahuja</p>
    <h2>Change Log</h2>
    <table>
      <thead>
        <tr>
          <th>Date (YYYY-MM-DD)</th>
          <th>Version</th>
          <th>Changed By</th>
          <th>Change Description</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>2021-05-30</td>
          <td>0.1</td>
          <td>Ramesh Sannareddy</td>
          <td>Created initial version of the lab</td>
        </tr>
      </tbody>
    </table>
    <p>Copyright (c) 2021 IBM Corporation. All rights reserved.</p>
    <script>window.addEventListener('load', function() {
snFaculty.inject();
});</script>
    <script src="https://skills-network-assets.s3.us.cloud-object-storage.appdomain.cloud/scripts/inject.43989f87.js"></script>
    <script src="https://unpkg.com/@highlightjs/cdn-assets@10.7.1/highlight.min.js"></script>
    <script src="https://unpkg.com/highlightjs-badge@0.1.9/highlightjs-badge.min.js"></script>
  

<style>
@media print {
   .code-badge { display: none; }
}
    .code-badge-pre {
        position: relative;
    }
    .code-badge {
        display: flex;
        flex-direction: row;
        white-space: normal;
        background: transparent;
        background: #333;
        color: white;
        font-size: 0.875em;
        opacity: 0.5;
        transition: opacity linear 0.5s;
        border-radius: 0 0 0 7px;
        padding: 5px 8px 5px 8px;
        position: absolute;
        right: 0;
        top: 0;
    }
    .code-badge.active {
        opacity: 0.8;
    }

    .code-badge:hover {
        opacity: .95;
    }

    .code-badge a,
    .code-badge a:hover {
        text-decoration: none;
    }

    .code-badge-language {
        margin-right: 10px;
        font-weight: 600;
        color: goldenrod;
    }
    .code-badge-copy-icon {
        font-size: 1.2em;
        cursor: pointer;
        padding: 0 7px;
        margin-top:2;
    }
    .fa.text-success:{ color: limegreen !important }
</style><div id="CodeBadgeTemplate" style="display:none">
    <div class="code-badge">
        <div class="code-badge-language">{{language}}</div>
        <div title="Copy to clipboard">
            <i class="{{copyIconClass}} code-badge-copy-icon"></i>
        </div>
     </div>
</div></body></html>
