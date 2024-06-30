
## Automated GitLab Runner Registration - A Fun Project

**Objective:**

The goal of this project is to automate the GitLab Runner registration process. This will allow you to easily set up and configure runners in your environment, without having to repeat manual steps each time.

**Prerequisites:**

-   Ansible installed on your system
-   Access to a Git repository containing the Ansible playbook

**Steps:**

1.  Execute the main playbook:

Bash

```
ansible-playbook playbook.yml
```

2.  This will do the following:
    
    -   Install Docker on the Runner server (for Docker executor) and create the necessary configurations.
    -   Register one runner with Shell executor and another runner with Docker executor.

**To run the runner locally:**

1.  Locate the Vagrant file in the repository.
2.  Execute the command `vagrant up`.

This will create a virtual machine (VM) and automatically install and configure GitLab Runner on it.

**Notes:**

-   You can edit the runner settings in the `playbook.yaml` file.
-   For more information on Ansible, please refer to [https://docs.ansible.com/](https://docs.ansible.com/).
-   For more information on GitLab Runner, please refer to [https://docs.gitlab.com/runner/](https://docs.gitlab.com/runner/).

**Benefits of this project:**

-   **Automation:** This project automates the GitLab Runner registration process, which can save you time and effort.
-   **Consistency:** This project ensures that your runners are consistently configured, which can help prevent problems.
-   **Scalability:** This project allows you to easily scale your runners, as you no longer need to perform manual steps for each runner.

**By completing this project, you can simplify and streamline the GitLab Runner setup and configuration process.**
