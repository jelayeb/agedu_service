# agedu_service
running agedu as a service to provide daily updated linux storage report. 

the driven for this plugin was the need to have a detailed report available for data managers about thier data inside our linux file server. 
i used to generate those reports on demand eatch time they request it using agedue. 
agedu is a tool that does the same task as du "disk usage" command but it generate a report accessible via web browser. 
agedu tool is essential to be installed to use this plugin. 

unfortunately i couldn't find a way to keep agedu running automatically in the background after i extit my ssh session, therefore i had to use tmux for this task,
TMUX is multiplixer console, which is similar to screen, where you can keep tasks running in the background and connect to them when you back next time. 

REQUIREMENTS:
agedue
tmux

Services and Config Files:

 /etc/init.d/agedu_daemon
 
 
