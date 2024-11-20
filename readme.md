sudo docker stats
sudo docker container stop mqtt
sudo docker run -it --rm --name mqtt -p 1883:1883 -p 9001:9001 -v $(pwd)/mosquitto.conf:/mosquitto/config/mosquitto.conf eclipse-mosquitto
