create Gitlab directory
`mkdir gitlab`
creat a variable for Gitlab directory
`export GITLAB_HOME=$(pwd)/gitlab`
now run `docker-compose up -d`
after creating and running all containers you can get root password from gitbal-ce container
`docker exec -it gitlab-ce grep 'Password:' /etc/gitlab/initial_root_password`
now you can login to your gitlab with root user and the password
