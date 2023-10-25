# Ansible Conditionals, loops and delegation

Ansible complex variables (array and dictionaries) are very important in Ansible but it is important to manage/use them as well. 

This lesson dives in conditionals and loops.

In order to understand this lesson properly, a set of steps have been designed to be implemented in the following section.

**ENJOY !!!**

## Steps 

-   Create an inventory file named "inventory" with a group named "myinstance" and include localhost
-   Create a playbook named "tools-playbook.yml" using "myinstance" as a hosts parameter. The playbook should use tasks to ensure that the following conditions are met on the managed hosts:
    -   Define the following variables:
        -   List or array of package names variable named "package" with values "lighttpd" and "fzf"
        -   List or Array of packages named "more_packages" with "fd-find" and "ncdu" included
    -   Install the list of "packages" and Notify the "Start lighttpd" handler 
    -   Restart lighttpd service if installation packages has not changed
    -   Install the list of "more_packages" using a loop
    -   Create a handler to start lighttpd and enable it if installation packages has changed
-   Before running your playbook, run the ansible-playbook --syntax-check  command to verify that its syntax is correct
-   Run the playbook!
-   Ensure lighttpd is running using `sudo systemctl status lighttpd`

## Useful Links

For more information, please visit:

-   https://docs.ansible.com/ansible/latest/user_guide/playbooks.html
-   https://docs.ansible.com/ansible/latest/modules/modules_by_category.html
-   https://docs.ansible.com/ansible/latest/user_guide/playbooks_conditionals.html
-   https://docs.ansible.com/ansible/latest/user_guide/playbooks_loops.html
-   https://docs.ansible.com/ansible/latest/user_guide/playbooks_delegation.html

License
-------

BSD

Author Information
------------------

 Asier Cidon - Cloud Consultant

 asier.cidon@redhat.com
 