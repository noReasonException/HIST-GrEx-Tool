@echo off      
                                           
echo   ,ad8888ba,             88888888888              
echo  d8"'    `"8b            88                       
echo d8'                      88                       
echo 88            8b,dPPYba, 88aaaaa     8b,     ,d8  
echo 88      88888 88P'   "Y8 88"""""      `Y8, ,8P'   
echo Y8,        88 88         88             )888(     
echo Y8a.    .a88 88         88           ,d8" "8b,   
echo   `"Y88888P"  88         88888888888 8P'     `Y8  Tool
echo -}
echo +----------------------------------------------------+
echo + GrEx Cmd Tool                                      +
echo + Version 0.01                                       +
echo + For help press 'help'                              +
echo + For credits press 'credits'                        +
echo +                                                    +
echo + Thank you !!!                                      +
echo +----------------------------------------------------+ 
echo.
                                                  

title Grex Cmd Tool
color 9f

:cmd

set /p choice=GrEx Cmd Tool:

if %choice%==help goto my_help
if %choice%==credits goto my_credits
if %choice%==clear goto my_cls
if %choice%==write goto my_write
if %choice%==make.file goto my_make.file
if %choice%==rename.file goto my_rename.file
if %choice%==delete.file goto my_delete.file
if %choice%==write.in.file goto my_write.in.file
if %choice%==make.folder goto my_make.folder
if %choice%==open goto my_open
if %choice%==exit goto my_exit
if %choice%==kill goto my_kill
if %choice%==close.computer goto my_close.computer
if %choice%==restart.computer goto my_restart.computer
if %choice%==cancel.computer goto my_cancel.computer
if %choice%==files.c goto my_files.c
if %choice%==files.user goto my_files.user
if %choice%==date goto my_date
if %choice%==time goto my_time
if %choice%==hardware goto my_hardware
if %choice%==editor goto my_editor
if %choice%==color goto my_color
if %choice%==version goto my_version
if %choice%==programs goto my_programs
if %choice%==local.net goto my_local.net
if %choice%==local.computer goto my_local.computer
if %choice%==computer.user goto my_computer.user
if %choice%==drive.info goto my_drive.info
if %choice%==maths goto my_maths
if %choice%==local.ip goto my_local.ip
if %choice%==net.server.ip goto my_net.server.ip
if %choice%==trace.ip goto my_trace.ip
if %choice%==ping.ip goto my_ping.ip
if %choice%==net.connections.ip goto my_net.connections.ip  
if %choice%==stop.connections goto my_stop.connections
if %choice%==start.connections goto my_start.connections
if %choice%==hide.file goto my_hide.file
if %choice%==appear.file goto my_appear.file
if %choice%==change.directory goto my_change.directory
if %choice%==show.history goto my_show.history
if %choice%==show.text.file goto my_show.text.file
goto error


:my_help
echo.
echo +-------------------------------------------------------+
echo }help              ~ Prints all commands                +
echo }credits           ~ Prints credits                     + 
echo }clear             ~ Clear the screen                   +
echo }write             ~ Print a alphanumeric               +
echo }make.file         ~ Creates a file                     +
echo }rename.file       ~ Renames a file                     +
echo }delete.file       ~ Deletes a file                     +
echo }write.in.file     ~ Writes into the file               +
echo }make.folder       ~ Creates a folder                   +
echo }open              ~ Opens a program                    +
echo }exit              ~ Terminate the GrEx Cmd Tool        +
echo }kill              ~ Kills a program                    +
echo }close.computer    ~ Closes the computer                +
echo }restart.computer  ~ Restarts the computer              +
echo }cancel.computer   ~ Cancels closing of computer        +
echo }files.c           ~ Shows all files in main hard drive +
echo }files.user        ~ Shows all current user files       +
echo }date              ~ Shows the current date             +
echo }time              ~ Shows the current time             +
echo }hardware          ~ Shows the pc capabilities          +
echo }editor            ~ Starts the old notepad             +
echo }color             ~ Change the GrEx tool color         +   
echo }version           ~ Shows Windows cmd version          +
echo }programs          ~ Shows the running programs         +
echo }local.net         ~ Shows the local connected devices  +
echo }local.computer    ~ Shows details of local computer    +
echo }computer.user     ~ Shows/change details of a user     +
echo }drive.info        ~ Shows the hard drive information   +
echo }maths             ~ You work with mathematics          +
echo }local.ip          ~ Shows the local ip addresses       +
echo }net.server.ip     ~ Shows the ip of a internet server  +
echo }trace.ip          ~ Shows the ip of your choice(trace) +
echo }ping.ip           ~ Shows the ip of your choice(ping)  +
echo }net.connections.ip~ A list with network connections(ip)+
echo }stop.connections  ~ Terminates connections             +
echo }start.connections ~ Re-establishes connections         +
echo }hide.file         ~ Hidden file attribute              +
echo }appear.file       ~ Appears file attribute             +
echo }change.directory  ~ Changes the directory              +
echo }show.history      ~ Shows the history of the commands  +
echo }show.text.file    ~ Shows the text of a file           +
echo +-------------------------------------------------------+      
echo.
echo.
echo.
goto cmd


:my_credits
echo.
echo +-------------------------------------------------------+
echo }         Why is it made?                               +
echo }This program is made because is hard for some people   +
echo }to use Cmd,so GrEx decided to make this program        +
echo }which will be almost like Cmd but with more            +
echo }understandable and easier to use commands,so           +
echo }everyone will can use it.                              +
echo }                                                       +
echo }                                                       +
echo }         About GrEx Cmd Tool:                          +
echo }The GrEx Cmd Tool is made by GrEx Development Team.    +      
echo }Developers are Hepic and El.Sonador.                   +
echo }The Version of this program is 0.01.                   +
echo }                                                       +
echo }                                                       +
echo }         About GrEx Development Team:                  +
echo }GrEx Development Team is a Greek programming-          +
echo }hacking(white hat) team.The members of the team        +
echo }(until now) are: Hepic,El.Sonador and kwnos100.        +
echo +-------------------------------------------------------+  
echo.
echo.
echo.
goto cmd


:my_cls
cls
goto cmd


:my_write
echo.
set /p setence=Write a setence:
echo.
echo %setence%
echo.
echo.
echo.
goto cmd


:my_make.file
echo.
set /p name=Write a name for the file:
echo GrEx Cmd Tool > %name%
echo.
echo.
echo.
goto cmd


:my_rename.file
echo.
set /p name=Enter the name of the file:
echo.
set /p new_name=Enter the new name of the file:
ren %name% %new_name%                                        
echo.
echo.
echo.
goto cmd


:my_delete.file
echo.
set /p name=Enter the name of the file:
del %name%
echo.
echo.
echo.
goto cmd


:my_write.in.file
echo.
set /p name=Enter the name of the file:
echo.
set /p setence=Write a setence:
echo %setence% >> %name%
echo.
echo.
echo.
goto cmd


:my_make.folder
echo.
set /p name=Write a name for the folder:
mkdir %name%
echo.
echo.
echo.
goto cmd


:my_open
echo.
set /p something=Write something that you want to open:
start %something%
echo.
echo.
echo.
goto cmd


:my_exit
exit
goto cmd


:my_kill
echo.
set /p something=Write something that you want to kill:
taskkill -im %something%.exe
echo.
echo.
echo.
goto cmd


:my_close.computer
echo.
set /p seconds=Enter the seconds:
echo.
set /p word=Enter a word:
shutdown -s -t %seconds% -c %word%
echo.
echo.
echo.
goto cmd


:my_restart.computer
echo.
set /p seconds=Enter the seconds:
echo.
set /p word=Enter a word:
shutdown -r -t %seconds% -c %word%
echo.
echo.
echo.
goto cmd


:my_cancel.computer
shutdown -a
echo.
echo.
echo.
goto cmd


:my_files.c
tree C:\
echo.
echo.
echo.
goto cmd


:my_files.user
tree
echo.
echo.
echo.
goto cmd


:my_date
date
echo.
echo.
echo.
goto cmd


:my_time
time
echo.
echo.
echo.
goto cmd


:my_hardware
systeminfo
echo.
echo.
echo.
goto cmd


:my_editor
edit
echo.
echo.
echo.
goto cmd


:my_color
echo.
echo Select colors(press the numbers,for your choice)
echo.
echo +-----------------Colors-------------------+
echo 1)black backround white letters            +
echo 2)Blue  backround white letters            +
echo 3)black backround green letters            +
echo 4)black backround red   letters            +
echo 5)write backround black letters            +
echo +------------------------------------------+
echo.
set /p color=Set color:
if %color%==1 goto blackwhite_color
if %color%==2 goto bluewhite_color
if %color%==3 goto blackgreen_color
if %color%==4 goto blackred_color
if %color%==5 goto whiteblack_color
goto color_error

:blackwhite_color
color 07
echo.
echo.
echo.
goto cmd

:bluewhite_color
color 9F
echo.
echo.
echo.
goto cmd

:blackgreen_color
color 0A
echo.
echo.
echo.
goto cmd

:blackred_color
color 0C
echo.
echo.
echo.
goto cmd

:whiteblack_color
color F0
echo.
echo.
echo.
goto cmd



:my_version
ver
echo.
echo.
echo.
goto cmd


:my_programs
echo.
tasklist
echo.
echo.
echo.
goto cmd


:my_local.net
echo.
net view
echo.
echo.
echo.
goto cmd


:my_local.computer
echo.
net user
echo.
echo.
echo.
goto cmd


:my_computer.user
echo.
set /p user=Enter a user:
net user %user%
echo.
set /p pass=Change password(y/n):
if %pass%==y goto yes
if %pass%==n goto no
goto pass_error
echo.
echo.
echo.
goto cmd

:yes
echo.
net user %user% *
echo.
echo.
echo.
goto cmd

:no
echo.
echo You choice not to change the password.
echo.
echo.
echo.
goto cmd



:my_drive.info
echo.
vol
echo.
echo.
echo.
goto cmd


:my_maths
echo.
set /p num1=Enter the first number:
echo.
set /p symbol=Enter a symbol:
echo.
set /p num2=Enter the second number:
echo.
echo.
set /a res=%num1%%symbol%%num2%
echo Result is: %res%
echo.
echo.
echo.
goto cmd


:my_local.ip
echo.
ipconfig -all
echo.
echo.
echo.
goto cmd


:my_net.server.ip
echo.
set /p server=Enter the internet server:
echo.
nslookup %server%
echo.
echo.
echo.
goto cmd


:my_trace.ip
echo.
set /p sth=Enter something:
echo.
tracert %sth%
echo.
echo.
echo.
goto cmd


:my_ping.ip
echo.
set /p sth=Enter something:
echo.
ping %sth%
echo.
echo.
echo.
goto cmd


:my_net.connections.ip
echo.
netstat -a -n -o
echo.
echo.
echo.
goto cmd


:my_stop.connections
echo.
ipconfig -release
echo.
echo.
echo.
goto cmd


:my_start.connections
echo.
ipconfig -renew
echo.
echo.
echo.
goto cmd


:my_hide.file  
echo.
set /p file=Enter a file:
echo.
attrib +h %file% 
echo.
echo.
echo.
goto cmd


:my_appear.file  
echo.
set /p file=Enter a file:
echo.
attrib -h %file% 
echo.
echo.
echo.
goto cmd


:my_change.directory
echo.
set /p directory=Enter a directory:
echo.
cd %directory%
echo.
echo.
echo.
goto cmd


:my_show.history
echo.
doskey /history
echo.
echo.
echo.
goto cmd


:my_show.text.file
echo.
set /p file=Enter a file:
echo.
type %file%
echo.
echo.
echo.
goto cmd


:color_error
echo.
echo pleasdeee select one of 5 choices
echo.
echo.
echo.
goto my_color


:pass_error
echo.
echo Please select (y/n)
echo.
echo.
echo.
goto my_computer.user


:error
echo.
echo Invalid command.Please try again!!!
echo.
echo.
echo.
goto cmd