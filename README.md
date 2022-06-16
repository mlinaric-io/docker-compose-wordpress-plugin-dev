# docker-compose-wordpress-plugin-dev

Environment for WordPress plugin development in containers

## Requirements

  - GNU/Linux OS
  - docker (with docker-compose)
  - git config user.name and user.email set

## Usage

```bash
# clone repository
git clone https://github.com/mlinaric-io/docker-compose-wordpress-plugin-dev

# make project.sh executable
chmod +x docker-compose-wordpress-plugin-dev/project.sh

# rename 'docker-compose-wordpress-plugin-dev' to the preferred
# name of our new plugin because plugin is named after parent
# folder of the project. Default plugin name is
# 'docker-compose-wordpress-plugin-dev'
mv docker-compose-wordpress-plugin-dev newpluginname

# go to 'newpluginname' and run 'project.sh start'
cd newpluginname && ./project.sh start
```

Wordpress site with activated 'newpluginname' shall be accessible on 'http://localhost'

## List of services from docker-compose.yml 

- composer
- node
- phpcbf
- phpcs
- phpdoc
- phpmyadmin
- phpunit

## License

docker-compose-wordpress-plugin-dev is licensed under [MIT license](LICENSE)
