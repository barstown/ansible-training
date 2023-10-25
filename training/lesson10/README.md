# Ansible Templates

Ansible Templates are a powerful tool which allows custom files can be generated based on variables. This lesson implements some examples about their implementation.

In order to understand this lesson properly, a set of steps have been designed to be implemented in the following section.

**ENJOY !!!**

## Resources

In order to assist this laboratory implementation, a set of resources have been added:

-   httpd.conf (Default Apache configuration file in Red Hat Enterprise Linux 8)
-   index.html (Basic HTML document structure)

## Steps 

-   Create an inventory file named "inventory" with a group named "myinstance" and include localhost
-   Create a playbook named "templates-playbook.yml" using "myinstance" as a hosts parameter. The playbook should use tasks to ensure that the following conditions are met on the managed hosts:
    -   Define an variable named "file_contents" which contains the a string of "hello world!"
    -   Copy the provided "file.txt.j2" template to your home directory
-   Before running your playbook, run the ansible-playbook --syntax-check  command to verify that its syntax is correct
-   Run the playbook!
-   Test the apache server

## Useful Links

For more information, please visit:

-   https://docs.ansible.com/ansible/latest/user_guide/playbooks.html
-   https://docs.ansible.com/ansible/latest/modules/modules_by_category.html
-   https://docs.ansible.com/ansible/latest/user_guide/playbooks_intro.html
-   https://docs.ansible.com/ansible/latest/modules/template_module.html
-   https://jinja.palletsprojects.com/en/2.10.x/
  
License
-------

BSD

Author Information
------------------

 Asier Cidon - Cloud Consultant

 asier.cidon@redhat.com
 