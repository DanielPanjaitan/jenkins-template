# jenkins-template

This project aims to create jenkins job that consist of unit test (phpunit, phpcs, phploc, pdepend, phpmd, phpcpd, and phpdox), github integration and polling scm method)

### installation
Before using this project, it is preferred to install phpunit, phpcs, phploc, pdepend, phpmd, phpcpd, and phpdox in local system or server and have cloned this project to local server.

- To create the job, either run:
```sh
$ cat config.xml | jenkins-cli -s http://localhost:8080/ create-job laravel-job
$ sudo chown -R jenkins:jenkins /var/lib/jenkins/jobs/laravel-job
$ jenkins-cli -s http://localhost:8080 reload-configuration
```

- then copy all of file and folder from cloned project to jenkins job folder
- configure the job from jenkins ui as needed
- run the job
