Stop and delete all containers:
docker stop $(docker container ls -q) && docker rm $(docker container ls -qa)


docker build -t identidock .

docker run -dit -p 5000:5000  --name identidockapp identidock

Trouble shooting:
docker logs identidockapp

curl localhost:5000
