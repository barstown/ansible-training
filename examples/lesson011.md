# Roles

I stripped down the lesson for Roles from the forked material.
However, I'd like your takeaway to be that when you initialize a new role
it will automatically generate a directory structure that contains
many/all of the folders/files you'll need to get start. It simplies new role
creation and also helps with consistency.

I made a new role in the examples/roles directory, and I
am calling it in a playbook below. One thing to note is the name of the role
as there are resrictions to the characters you can use in role names.

Fun fact, you can define vars when you call a role in a playbook directly!

```yml
---
- name: Using an Ansible Role
  hosts: myinstance
  become: true

  roles:
    - role: web.server
      vars:
        foo: bar
```

Further, let's look at some of the directories in this role.
- Note there are both "defaults" and a "vars" directory. Both of these contain variables!
  - What's the difference?