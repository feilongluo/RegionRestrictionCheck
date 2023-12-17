## 使用方法

**使用脚本前请确认curl已安装**

````bash
bash <(curl -L -s https://github.com/feilongluo/RegionRestrictionCheck/raw/main/check.sh)
````

##### 只检测IPv4结果：
````bash
bash <(curl -L -s https://github.com/feilongluo/RegionRestrictionCheck/raw/main/check.sh) -M 4
````

##### 只检测IPv6结果：
````bash
bash <(curl -L -s https://github.com/feilongluo/RegionRestrictionCheck/raw/main/check.sh) -M 6
````

##### 指定检测的网卡名称：
````bash
bash <(curl -L -s https://github.com/feilongluo/RegionRestrictionCheck/raw/main/check.sh) -I eth0
````

##### 选择脚本语言为英文：
````bash
bash <(curl -L -s https://github.com/feilongluo/RegionRestrictionCheck/raw/main/check.sh) -E
````

**或者直接运行以下Docker命令** (兼容ARM架构)
````docker
docker run --rm -ti --net=host lmc999/regioncheck && docker rmi lmc999/regioncheck
````