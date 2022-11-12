<h3> To check Desktop environment; major distributions gnome and kde </h3>

    ls /usr/bin/*session

-----------------------------------------------------------------------------------------------

<h3> Releaese </h3>

    lsb_release - print distribution-specific information

Linux standard base

    lsb_release -a

for more information

    lsb_release --help

--------------------------------------------------------------------------------------------

<h3>Print system specific information</h3>
    
    uname

Kernel name

    uname -s

Node name

    uname -n
    uname -a #all the details

More information 
    
    man uname

To print hostname
    
    hostname

To print effective username/Logged in user
    
    whoami

Displaying information about USB buses in the system and the devices connected to them.
    
    lsusb

Displaying information about PCI buses in the system and devices connected to them    
    
    lspci

--------------------------------------------------------------------------------------

Cursor Movement

    up-arrow # to see previous command
    tab - to print remaning words in a command

--------------------------------------------------------------------------------------

# Some more commands

<h3>displaying calendar</h3>

    cal

<h3> to display the amount of free memory</h3>

    free

<h3> to close a terminal session</h3>

    exit

----------------------------------------------------------------------------------------
<h3>list specific file</h3>

    ls -l <nameoffile>  

-----------------------------------------------------------------------------------------

<h3>Field explanation </h3>
Field 1 – file permission <br>

* – normal file
* d : directory
* s : socket file
* l : link file

<br>

    -rw-r--r--  1 bhupendra bhupendra        60 Aug 28 21:09 ntp-server.txt
    user,group,any/others

Field 2 – Number of links: (like 1,2,3 depends)<br>
Field 3 – Owner<br>
Field 4 – Group<br>
Field 5 – Size (bytes)<br>
Field 6 – Last modified date and time<br>
Field 7 – File name<br>

    ls -a #list all the hidden files and directories

--------------------------------------------------------------------------------------------- 

<h3> to write some content inside a file </h3> 

    echo 
    echo <somemsg> > <nameoffile> #if file NA on the file is created, overright of data is already available
    echo <somemsg> >> <name of the file> #append contents in a file

<h3>  change permission of the file</h3> 

    chmmod #change file mode bits

numeric -
<br>0 - nothing
<br>4 -only read
<br>2 - only write
<br>1 - only execute
<br> <br>
4+1 = 5 read and execute <br>
4+2 = 6 read and write both <br>
4+2+1 = 7 read,write and execute <br>
    
    chmod 700 a.txt #readwriteexeute to user only


Letters

    r -read
    w - write
    x -execute 
<br>

    u -user
    g -group
    o -other

<br>
Assign user 'read write and execute' permissions (+ to add) 

    chmod u+rwx a.txt  

Remove user's 'read write and execute' permissions (- to remove)

    chmod u-rwx a.txt  

---------------------------------------------------------------

<h3> copy a file</h3>

    cp <sourcepath> <destinationpath>
<h3> move file </h3>

    mv <sourcepath> <destinationpath>

--------------------------------------------------------------------

<h3> Mapping of host and IP address:</h3>

    BHIoT$ cat /etc/hosts
    127.0.0.1	localhost
    127.0.1.1	iot
    127.0.1.2	bhupendra.iot


<h3> The following lines are desirable for IPv6 capable hosts </h3>

    ::1     ip6-localhost ip6-loopback
    fe00::0 ip6-localnet
    ff00::0 ip6-mcastprefix
    ff02::1 ip6-allnodes
    ff02::2 ip6-allrouters


-----------------------------------------------------------------------------------------------

&copy;  2022, Rohit Akurdekar&trade;