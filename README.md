# ぼくの最強のDocker image だよ！！

## Docker on Linux用
Dockerのコンテナにローカルと同じuserで入れるよ☆

### Docker imageをbuild
```sh
#shell
$ docker build -t mybase .
```
### Docker imageを別ファイルに作る
RubyやNodeを好きに入れてイメージを作成
```dockerfile
#Docker file
FROM mybase

CMD ["/bin/bash"]
```
build!!
```sh
#shell
docker build -t myimage .
```
以下のコマンドでDockerのコンテナにローカルユーザーと同じUIDで入る
```sh
#shell
docker run -it -e LOCAL_USER_ID=`id -u $USER` myimage
```
Let's happy Docker!:whale:
