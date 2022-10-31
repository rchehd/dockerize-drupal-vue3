<p align="center">
  <img src="https://cdn.svgporn.com/logos/docker-icon.svg" width="200" height="100"  alt="VueJS Logo"/>
  <img src="https://cdn.svgporn.com/logos/vue.svg" width="200" height="100"  alt="Docker Logo"/>
  <img src="https://cdn.svgporn.com/logos/drupal.svg" width="200" height="100"  alt="Drupal Logo"/>
</p>

### Dockerizing Drupal && VueJS 3
### Based on <a href="https://github.com/nicer00ster/dockerize-drupal-vue">nicer00ster/dockerize-drupal-vue</a>
### Updates
- VueJs updated from 2 to 3
- Added Vue router to create multipages application
- Update Node from 12 to 16

## Installation

To spin up the whole application for the first time in dev mode:
<br/>
**Make sure to install the latest version of [Docker](https://www.docker.com/) and Python 3.5 or greater before continuing**
```sh
$ git clone https://github.com/rchehd/dockerize-drupal-vue3.git
$ cd dockerize-drupal-vue3
$ copy .env.default to .env
$ set project name in .end PROJECT_NAME=your_project_name
# 
# Install all the docker containers:
$ make install
#  if you get error change owner of drupal directory "sudo chmod -R 777 drupal"
#
# To destroy all containers and data associated:
$ make down
#
# To pause the containers:
$ make stop
#
# To bring the containers back up: 
$ make up
```
**Backend url: http://drupal.docker.localhost/
<br>
Frontend url: http://app.docker.localhost/**