# ELK
EKL이모저모


## 셋업
- 도커셋업 https://github.com/deviantony/docker-elk.git    


- 신경써야하는 포트 3가지 5601 Kibana, 9200 Elasticsearch HTTP ,9300 Elasticsearch TCP transport   
- heap 메모리 에러시 -> docker-stack.yml , docker-compose.yml 에서 ES_JAVA_OPTS: "-Xmx512m -Xms512m" 으로 256 -> 512 변경할것     


## docker compose 파라미터
docker-compose up --scale elasticsearch-data=3 --no-recreate -d -> data노드 3개로증가 
