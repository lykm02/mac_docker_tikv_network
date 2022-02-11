# mac_docker_tikv_network

### How Problem raise
I need to require spark program using tikv on mac. So I build a local tikv envrionment using docker.
The problem is I cannot ping to local tikv container IP, which cause connection timeout. The problem block the progress.

After some search. I found some helpful solutions.

Solution 1: openvpn


Solution 2: docker-connector
   https://github.com/wenjunxiao/mac-docker-connector/blob/mac/README.md
The origin doc from search engine is : https://www.haoyizebo.com/posts/fd0b9bd8/

It setup a docker image as vpnserver, all you need do is initializing configs and starting up image.


I picked up Solution 2, because it's easy to use.

