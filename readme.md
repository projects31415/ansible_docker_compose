# Repo with ansible playbooks for deploying simple docker-compose project(nginx_php_mysql)

```
alias ap=ansible-playbook
alias ag=ansible-galaxy
```

## install ansible dependencies
```
ag install -r requirements.yml
```

## (optional) install docker and docker-compose on server
```
ap -i inventories/dev playbooks/app_prepare.yml
```

## deploy docker-compose project
```
ap -i inventories/dev playbooks/app_deploy.yml
```
