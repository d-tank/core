# core
docker run -it --net='host' -P -e IP=$(/sbin/ip route|awk '/24/ { print  $9}') -e discovery=$DISCOVERY_STRING dtank/core

^^ copy discovery url/token into /usr/local/bin/run-etcd
