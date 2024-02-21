#### Machine Controls
<br>


> to reboot the machine   

`# reboot`  |   `# systemctl reboot` 

`# init 6` : not recommended

---

#### Managing Services
<br>

> to enable the service

`# systemctl enable [service_name]`    


<br>

> to start the service

`# systemctl start [service_name]`

<br>

> to start and enable the service 

`# systemctl enable [service_name] --now`

<br>

---

#### MAN
<br>

> to view the manual page of any command 

`# man [ command ]`  
<br>

> to quit from the manual page

`press q`

<br>

> to get more info on how to use man command more effectively

`press h`

<br>

> to search for any keyword in the page

`press / and then type the keyword and then hit enter`

<br>

> to navigate across the different matches in the search 

`press n to move from top to bottom and N (shift+n) to move from bottom to top : one match at a time`

<br>

> to navigate to the begin and end of the page

`press g or < to go to the begining and press g OR > to go to the ending of the page`

<br>

> to see all the builtin commands 

`# man builtins`

<br>

> to navigate to the specific section of the man page 

`# man [section number] [ command ]`

<br>

> to update the indicies of man db

`# mandb`

<br>

> to view the manual of the man page

`# man man`

<br>

---

#### FIND THE LOCATION OF BINARY and MAN PAGE OF ANY COMMAND
<br>

> to view the manual of the man page

`# whereis [ command ]`

<br>

---

#### AUTO COMPLETION
<br>

> to auto complete the command path 

`press tab`

<br>

> to see all the suggestion for auto complettion of command path

`press tab tab`

---