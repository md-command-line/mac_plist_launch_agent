### TLDR; to incorporate your main executable:
1) overide app/script.sh with terminal install instructions.
2) This repository can be found at https://github.com/MichaelDimmitt/mac_plist_launch_agent/

## Installation(program persists when installed until uninstalled.)
1) git clone your_project.git
2) cd your_project
3) git clone https://github.com/MichaelDimmitt/mac_plist_launch_agent.git
4) cd mac_plist_launch_agent
5) ./app/install_driver
6) ./app/uninstall_driver

7) now modify the script file to run your application 
<br>($DIR/.././your_application) or (open $DIR/../your_application)

### install and start 
4) ./mac_plist_launch_agent/app/install_driver.sh
### uninstall and stop
5) ./mac_plist_launch_agent/app/uninstall_driver.sh

## Template from which others can build Launch Agents.
Only for Macintosh Computers, enjoy.
Make an application or a script a launch agent.

Simple example of a mac app launch agent. People can use as a template.
<br>Starts and Stops via different bash scripts.

## Challenges (why needed)
Launch Agents do not immediately provide output<br>
to where a programmer can immediately see hello world.<br>
install_driver... sets the plist up and runs.

### to incorporate your main executable:
1) overide app/script.sh with terminal install instructions.

## how install_driver sets the plist up and runs:
app/install_driver allows plist to know your repo location<br>
app/install_driver script gathers "pwd" and injects it into the plist<br>
then install driver gives permission moves to standard location and runs.<br>
uses launchctl...


## Useful links

https://nathangrigg.com/2012/07/schedule-jobs-using-launchd<br>
https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man5/launchd.plist.5.html

## Large scale implementation:
project abstracted from:<br>
https://github.com/MichaelDimmitt/Aerial_Desktop
