# Sonarqube Docker Composer

## Step 1

```
$ git clone https://github.com/peyman13/sonarqube-docker-composer.git
$ cd sonarqube-docker-composer

```
## Step 2

```
$ sudo docker-composer up -d 

```

## Step 3

```
open http://localhost:9000
login to as admin (user:admin, password: admin)

```

## Step 4

```
create new project and take token 

```
## Step 5

```
$sudo docker run --rm -e SONAR_HOST_URL="http://{$Your ip}:9000" -e SONAR_LOGIN="{YOU Token}" -e SONAR_PROJECTKEY="{$project key}" -v "{$Project_dir}:/usr/src" sonarsource/sonar-scanner-cli -Dsonar.projectKey="{$project_key}"

```
## Step 6

```
check your panel and analyze result

```



