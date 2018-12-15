# ansible-stuff
Prior to running these, i'm doing an `ssh-copy-id` of my key to all nodes, to speed up the process. 

Mainly I'm using these for one-off execution of logic, using:

`ansible-playbook -i inventory -K playbook.yml`

The `.retry` files are leftovers from ansible runs, and can be ignored (but will be regenerated when things fail)

And for the lazy, who don't want to keep typing their sudo password:

`ansible-playbook -i inventory --extra-vars 'ansible_become_pass=blah' playbook.yml`

