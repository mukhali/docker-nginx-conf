docker-compose restart

## 1 准备条件
* 安装好Docker。 

* 准备好域名。

## 2 修改配置文件
* 将run.sh中的域名修改成你自己的，邮箱也需要修改。

* 将 data/ngnix/conf.d 目录下的 conf文件中的域名修改成你的。

## 3 运行
~~~
bash run.sh
~~~

## 4 修改配置文件后按下面顺序重启
~~~
docker-compose stop

docker-compose -f docker-compose.yml up --force-recreate -d nginx

docker-compose restart
~~~

## 5 致谢

感谢[FastGitORG](https://github.com/FastGitORG)团队的付出，最初配置文件来之于FastGitORG。
