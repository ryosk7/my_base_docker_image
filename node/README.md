### Node.js and Vue.js on Docker for linux
This is Docker for Linux users tips.
"Non root permission on Docker container"
```sh
#shell
$ docker run -it -e LOCAL_USER_ID=`id -u $USER` node-mybase
```
Then you can login to docker container as user. 
```sh
#docker shell
$ node -v
v11.14.0
$ vue --version
2.9.6
```
Done!
Happy Vue and Docker life :whale:
