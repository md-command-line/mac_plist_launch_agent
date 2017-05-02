## Instillation with ruby Rakefile
1) clone project
2) cd project
3) rake install

## Uninstall with ruby Rakefile
1) cd project
2) rake uninstall

## Template from which others can build Launch Agents.
Make an application or a script a launch agent.

Simple example of a mac app launch agent. People can use as a template. Starts and Stops via different bash scripts. 
## Challenges (why needed)
Launch Agents do not immediately provide output<br>
to where a programmer can immediately see hello world.<br>
install_driver... sets the plist up and runs.

## how install_driver sets the plist up and runs:
install_driver allows plist to know your repo location<br>
install_driver script gathers "pwd" and injects it into the plist<br>
then install driver gives permission moves to standard location and runs.<br>
uses launchctl...

## Useful links 

https://nathangrigg.com/2012/07/schedule-jobs-using-launchd<br>
https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man5/launchd.plist.5.html

project abstracted from:<br>
https://github.com/MichaelDimmitt/ScreenSaver_to_DesktopBackground_mac
