# Day4_linuxUSER
# File hierarchy/system=file managment
 spesial o of linux rather than window which uses files.
 - structured directory/folder/
 - system file ==> used files by the operating systems
 linux: system files appear under the root directory(/)
 file structure detail
 
1 )
/ root
 - every directory start from root
 - /root is power prevelage
 - only root owner can write on the directory
 - / is the place of storing files of user
 bin-binary executables
 - Essential command files for single user are stored 
2 )
/BOOT
 /boot -Boot loader files
 - kernal initrd,vmlinux,grub files are located here
 3 )
 /dev-Essensial device files
 - attachved terminal devices are stored by linux as file in /dev.
 - eg./dev/ttt1,/dev/usbmon0/
 4 )
 /etc - et cetera
 - contain configuration file required by all progarms
 - also contain startup and shutdown  shell scripts
 - eg./etc/hosts(ip address).
 5 )
 /home-home directory
 - directory for users that stores users personal file
 - ~=== /home/username
6 ) 
/lib- liabrary essential for the binaries in /bin & /sbin
 =>liabrary filenamea are either id*  or lib*,so*
 eg.Id-2.11.1. so libncurses.so.5.7
7 ) 
/media-mouted point for removable media such as CD-ROMs
 - mounted  liabrary storage of that is temporary
 - eg./media/cdrom forCD-ROM;
 8 )
 /mnt- Temporary mounted file
 - temlporary mount dirrctory where sysadmins can mount filesystem.
9 )
/opt-optional application software packages 
 - store inistalled files
 10 )
 /sbin-essential system binary 
 - store information for addministrators/root/ for system mentenance purpose 
 command for single users have 'previous command of sudo to act like root to run  commands in sbin'
 11 )
 /tmp -Temporary files
 - create files for temporary use are stored here.
 - deleted when the system is rebooted.
12 )
/usr- User utilities
 - acontain binaries,liabrary,documentation,and, source-code for second  levelprograms.
 - eg./usr/bin-look files in bin for other users
 -       /usr/sbin
 
 text editor
 - lused for text processing.
 - in linux lthere are
 - operated  on linux terminal->VIM
                  ->Nano
                  ->Emacs
                  ->Neovim
    may be commands or softwares
    linux Graohical text editors
    ->Sublime
     ->Vscode
     ->Gedit
     ->Pluma ...
     **VIM(VI IMPROVED)
     
     1st text editor starting from unix that users can only see and a single edit line known for VI(line editor) 
     - powerful but creaptic due to mode and hard to learn
     MOdes of VIM
     1.COMAND MODE
     2.INPUT
     3.VISUAL=>manipulation is allowed
     according to selection of texts
     1.character wise visual mode->letter by letter
     press 'v'
     2.line wise mode ==> selecting line press "shift+v"
     3.block wise mode==>select recvtangular text blocks of text press"ctrl+v or ctrl+q'
     4.NORMAL->defualt value(no write,save,)
     to write=>enter to insert mode
     to save==> enter  to command mode inside it i ca  save,quit,force save and quit,undo,execiute bash ;command,save and quit
     save :w
     quit :q
     force quit and save :wq!
     undo :u
     execute command :%!yourcommand
     while bing vim aftrer selevtio deletion is done by pressing d.
     copy y
     pest p


**Nano 
gnu nano text editor that is very easy and and by defaul by it is pre installed in linux. usus short cuts
nano nano.txt
undo->before
redo->after
^====   ctrl /    
ctrl +s~save
ctrl+u  ~ undo
alt +e ~ redo
ctrl + X ~exit
ctrl +shift+ C ~ copy
ctrl+shift+X ~ cut
ctrl+shift+V~ paste
?open,wirte 
ctrl + R -> append a file. as  ~/ path/filename


Linux User managment
 on  computer system computer user are known as user.
 Group~every user have group when they create a username.
 evegry user also have file amd application that is stored on home.
 to know user name on linux we use "whoami"
 => users have power/root/ cereater of linux system who can add users. and previlage/user/
  Root id =0,
  Normal User id starts with 1-999
  if user want to be act like root,it uses the 'sudo' infront of the command.
  the first user id is 1000.
  sudo=super user do! used to by pass permission  denie message.
  onlinux to ceate user we ise
  - Useradd -> simple
  -sudo useradd username
  users created here have shell type of sh.
  - adduser ->Detailed
sude adduser username
group is created on same name as username
 users created here have shell type of bash.
 - the user file are stored in /etc/passwd
 - user password asre stored inside /etc/shadow which places in hexadeci may be but it is goingto be  decripted/solved/.
 - encript/look/
 - only one root is available.
 - hacker,takedown/takeover,keliven hemi, reccommended films.
