# Stephane ROBERT ansible Snippets for Visual Studio Code

This Visual Studio Code extension has snippets to help you write your Ansible
code when you are recommendations on my [personal blog](https://blog.stephane-robert.info/)

![ansible snippets vscode](https://github.com/stephrobert/ansible-snippets/raw/main/img/sr-ansible-snippet.gif)

**I ll add more snippets in a few days!!**

## List of snippets

**Format :**

* module
  * text to invoque

* playbook
* block
* ansible.builtin.add_host:
  * "add host to group"
* ansible.builtin.assert:
  * "Assert"
* ansible.builtin.copy:
  * "copy a file"
* ansible.builtin.debug:
  * "debug a task"
* ansible.builtin.file:
  * "create a file"
  * "touch a file"
  * "create a directory"
* ansible.builtin.get_url:
  * "download file"
* ansible.builtin.group:
  * "Create a group",
  * "Destroy a group",
  * "Modify a group"
* ansible.builtin.hostname:
  * "Manage hostname"
* ansible.builtin.lineinfile:
  * "include a line in a file"
* ansible.builtin.package:
  * "install a package"
* ansible.builtin.service:
  * "start a service"
  * "stop a service"
  * "enable a service"
  * "disable a service"
* ansible.builtin.service_facts:
  * "Get service state information as fact data"
* ansible.builtin.setup:
  * "get facts"
* ansible.builtin.set_fact:
  * "compute a variable"
  * "set a variable"
* ansible.builtin.stat:
  * "status of a file or a directory"
* ansible.builtin.template:
  * "generate a file from a template"
* ansible.builtin.unarchive:
  * "unarchive a compressed file"
* ansible.builtin.user:
  * "Create an user account",
  * "Destroy an user account",
  * "Modify an user account"
* ansible.builtin.wait_for:
  * "Waits for a condition before continuing"
* ansible.builtin.wait_for_connection:
  * "Waits until remote system is reachable"
* ansible.builtin.import_tasks:
  * "Import tasks"
* ansible.builtin.include_tasks:
  * "Include tasks"
* ansible.builtin.import_playbook:
  * "Import playbook"
* ansible.builtin.import_role:
  * "Import role"
* ansible.builtin.include_role:
  * "Include a Role"

<!-- set_fact, stat, blockinfile, lineinfile, assert, includes, wait_for, import_tasks, unarchive
- name: Add os specific variables
  ansible.builtin.include_vars: "{{ loop_vars }}"
  with_first_found:
    - files:
        - "{{ ansible_distribution | lower }}-{{ ansible_distribution_version }}.yml"
        - "{{ ansible_distribution | lower }}-{{ ansible_distribution_major_version }}.yml"
        - "{{ ansible_distribution | lower }}.yml"
        - "{{ ansible_os_family | lower }}.yml"
        - "{{ ansible_system | lower }}.yml"
        - "main.yml"
      paths:
        - "vars"
  loop_control:
    loop_var: loop_vars -->