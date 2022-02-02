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

## NOT: if it has error such as "max virtual memory areas vm.max_map_count [65530] is too low, increase to at least [262144]"

```
sudo sysctl -w vm.max_map_count=262144
sudo sysctl --system

```

## Step 3

```
open http://localhost:9000
login to as admin (user:admin, password: admin)

```

## Step 4

```
Create new project and take a token 

```
## Step 5

```
$sudo docker run --rm -e SONAR_HOST_URL="http://{$Your ip}:9000" -e SONAR_LOGIN="{YOU Token}" -e SONAR_PROJECTKEY="{$project key}" -v "{$Project_dir}:/usr/src" sonarsource/sonar-scanner-cli -Dsonar.projectKey="{$project_key}"

```
## Step 6

```
check your panel and analyze result

```



