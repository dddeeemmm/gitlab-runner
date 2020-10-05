gitlab-runner
=========

    Install GitLab Runner and join to GitLab 

Role Variables
--------------

    glrunner_install: true              [ true | false ] for skip installation
    glrunner_reconfig: false            [ true | false ] for remove old config
    gitlab_registration_token: ''       [ required ] registrtion token (go to the GitLab Admin Area and click Overview > Runners)


Example Playbook
----------------

    - hosts: glrunner-build
      become: true
      roles:
        - { name: gitlab-runner,  tags: glrunner }

License
-------

    MIT

Author Information
------------------

    Dmitrij Petrov
