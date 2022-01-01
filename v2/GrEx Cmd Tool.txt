@echo off      
title Grex Cmd Tool v2
color 9f                                                                                                                                
echo :'######:::'########::'########:'##::::'##::::
echo '##... ##:: ##.... ##: ##.....::. ##::'##:::::
echo  ##:::..::: ##:::: ##: ##::::::::. ##'##::::::
echo  ##::'####: ########:: ######:::::. ###:::::::
echo  ##::: ##:: ##.. ##::: ##...:::::: ## ##::::::
echo  ##::: ##:: ##::. ##:: ##:::::::: ##:. ##:::::
echo . ######::: ##:::. ##: ########: ##:::. ##::::
echo :......::::..:::::..::........::..:::::..:::::
echo 				           Master Tool
echo -}
echo +----------------------------------------------------+
echo + GrEx Cmd Tool                                      +
echo + Version 2.00.                                      +
echo + For help press 'help'                              +
echo + For credits press 'credits'                        +
echo +                                                    +
echo + Thank you !!!                                      +
echo +----------------------------------------------------+ 
echo.

:cmd

set /p choice=GrEx Cmd Tool:

if %choice%==help goto help
if %choice%==credits goto credits
if %choice%==clear goto cls
if %choice%==write goto write
if %choice%==make.file goto make.file
if %choice%==rename.file goto rename.file
if %choice%==delete.file goto delete.file
if %choice%==write.in.file goto write.in.file
if %choice%==make.folder goto make.folder
if %choice%==open goto open
if %choice%==kill goto kill
if %choice%==close.computer goto close.computer
if %choice%==restart.computer goto restart.computer
if %choice%==cancel.computer goto cancel.computer
if %choice%==files.c goto files.c
if %choice%==files.user goto files.user
if %choice%==date goto date
if %choice%==time goto time
if %choice%==hardware goto hardware
if %choice%==editor goto editor
if %choice%==color goto color
if %choice%==version goto version
if %choice%==programs goto programs
if %choice%==local.net goto local.net
if %choice%==local.computer goto local.computer
if %choice%==computer.user goto computer.user
if %choice%==drive.info goto drive.info
if %choice%==maths goto maths
if %choice%==local.ip goto local.ip
if %choice%==net.server.ip goto net.server.ip
if %choice%==trace.ip goto trace.ip
if %choice%==ping.ip goto ping.ip
if %choice%==net.connections.ip goto net.connections.ip  
if %choice%==stop.connections goto stop.connections
if %choice%==start.connections goto my_start.connections
if %choice%==hide.file goto hide.file
if %choice%==appear.file goto appear.file
if %choice%==change.directory goto change.directory
if %choice%==show.history goto show.history
if %choice%==show.text.file goto show.text.file
if %choice%==bootedit goto bootedit
if %choice%==resize goto resize
if %choice%==attack goto attack
if %choice%==print.file goto print.file
if %choice%==cmd.help goto cmd.help
if %choice%==x goto exit_

goto error


:help
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
echo }bootedit          ~ Edit in Boot.cfg file              +
echo }resize            ~ Resize the cmd window              +
echo }attack            ~ Attack in target ip {ping overflow}+
echo }print.file        ~ Print a text file                  +
echo }cmd.help          ~ More information about cmd         +
echo }x                 ~ Terminate the Programm             +
echo +-------------------------------------------------------+      
echo.
echo.
echo.
goto cmd


:credits
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
echo }The Version of this program is 2.00.                   +
echo }                                                       +
echo }                                                       +
echo }         About GrEx Development Team:                  +
echo }GrEx Development Team is a Greek programming-          +
echo }hacking(white hat) team.The members of the team        +
echo }(until now) are: Hepic,El.Sonador, kwnos100.           +
echo },Knss,Senior Vidar.                                    +
echo +-------------------------------------------------------+  
echo.
echo.
echo.
goto cmd


:my_cls
cls
goto cmd


:write
echo.
set /p setence=Write a setence:
echo.
echo %setence%
echo.
echo.
echo.
goto cmd


:make.file
echo.
set /p name=Write a name for the file:
echo GrEx Cmd Tool > %name%
echo.
echo.
echo.
goto cmd


:rename.file
echo.
set /p name=Enter the name of the file:
echo.
set /p new_name=Enter the new name of the file:
ren %name% %new_name%                                        
echo.
echo.
echo.
goto cmd


:delete.file
echo.
set /p name=Enter the name of the file:
del %name%
echo.
echo.
echo.
goto cmd


:write.in.file
echo.
set /p name=Enter the name of the file:
echo.
set /p setence=Write a setence:
echo %setence% >> %name%
echo.
echo.
echo.
goto cmd


:make.folder
echo.
set /p name=Write a name for the folder:
mkdir %name%
echo.
echo.
echo.
goto cmd


:open
echo.
set /p something=Write something that you want to open:
start %something%
echo.
echo.
echo.
goto cmd


:kill
echo.
set /p something=Write something that you want to kill:
taskkill -im %something%.exe
echo.
echo.
echo.
goto cmd


:close.computer
echo.
set /p seconds=Enter the seconds:
echo.
set /p word=Enter a word:
shutdown -s -t %seconds% -c %word%
echo.
echo.
echo.
goto cmd


:restart.computer
echo.
set /p seconds=Enter the seconds:
echo.
set /p word=Enter a word:
shutdown -r -t %seconds% -c %word%
echo.
echo.
echo.
goto cmd


:cancel.computer
shutdown -a
echo.
echo.
echo.
goto cmd


:files.c
tree C:\
echo.
echo.
echo.
goto cmd


:files.user
tree
echo.
echo.
echo.
goto cmd


:date
date
echo.
echo.
echo.
goto cmd


:time
time
echo.
echo.
echo.
goto cmd


:hardware
systeminfo
echo.
echo.
echo.
goto cmd


:editor
edit
echo.
echo.
echo.
goto cmd


:color
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



:version
ver
echo.
echo.
echo.
goto cmd


:programs
echo.
tasklist
echo.
echo.
echo.
goto cmd


:local.net
echo.
net view
echo.
echo.
echo.
goto cmd


:local.computer
echo.
net user
echo.
echo.
echo.
goto cmd


:computer.user
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



:drive.info
echo.
vol
echo.
echo.
echo.
goto cmd


:maths
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


:local.ip
echo.
ipconfig -all
echo.
echo.
echo.
goto cmd


:net.server.ip
echo.
set /p server=Enter the internet server:
echo.
nslookup %server%
echo.
echo.
echo.
goto cmd


:trace.ip
echo.
set /p sth=Enter something:
echo.
tracert %sth%
echo.
echo.
echo.
goto cmd


:ping.ip
echo.
set /p sth=Enter something:
echo.
ping %sth%
echo.
echo.
echo.
goto cmd


:net.connections.ip
echo.
netstat -a -n -o
echo.
echo.
echo.
goto cmd


:stop.connections
echo.
ipconfig -release
echo.
echo.
echo.
goto cmd


:start.connections
echo.
ipconfig -renew
echo.
echo.
echo.
goto cmd


:hide.file  
echo.
set /p file=Enter a file:
echo.
attrib +h %file% 
echo.
echo.
echo.
goto cmd


:appear.file  
echo.
set /p file=Enter a file:
echo.
attrib -h %file% 
echo.
echo.
echo.
goto cmd


:change.directory
echo.
set /p directory=Enter a directory:
echo.
cd %directory%
echo.
echo.
echo.
goto cmd


:show.history
echo.
doskey /history
echo.
echo.
echo.
goto cmd


:show.text.file
echo.
set /p file=Enter a file:
echo.
type %file%
echo.
echo.
echo.
goto cmd


:bootedit
echo.
bootcfg
echo.
echo.
echo.
goto cmd


:resize
echo.
set /p sizex = Enter the x value ~ 
set /p sezey = Enter the y value ~ 
mode con cols = %sizex%  lines = %sizey%
echo.
echo.
echo.
goto cmd

:attack
echo.
set/p name = Enter target IP ~ 
set/p data = Enter usage of data{untl 6400) ~ 
ping %name%  -t -l %data%
echo.
echo.
echo.
goto cmd

:print.file
echo.
set/p name = Enter the file name ~ 
set/a ex = .txt
set /a printfile=%name%%ex%
print printfile
echo.
echo.
echo.
goto cmd

:cmd.help
echo.
echo Cmd is a port to communicate with Windows NT
echo {Windows Kernel} so you can do anything you
echo want with  commands.The disadvance is
echo that commands difficult to learn and understand
echo this is some of command of Windows cmd...
echo take a look ...remarked how difficult are the 
echo commands as opposed to the commands 
echo of the program GrEx which is much easier
echo Press any key to continue
pause >nul
help
echo.
echo.
echo.
goto cmd


:exit_
cls
echo +--------------------------------------------------------------+
echo +Thanks for using GrEx CMD Master tool v.02 +
echo +--------------------------------------------------------------+
echo ~ Press any key to continue...
pause >nul
exit



:color_error
echo.
echo please select one of 5 choices
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