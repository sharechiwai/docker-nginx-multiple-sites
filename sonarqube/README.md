### SonarQube
```bash
docker-compose up
```

It is very like to record the following error, which lead to not be able to start the container  
`max virtual memory areas vm.max_map_count [65530] is too low, increase to at least [262144]`  
**Solution**  
execute the following command on the host  
```bash
sudo sysctl -w vm.max_map_count=262144
```

REF: https://sharechiwai.com/post/2022/2022-08-03-run-sonarqube-in-docker/