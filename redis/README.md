## 部署redis的ansible脚本

### 要修改的参数
- 1. hosts_yaml文件，这是ansible的清单文件，使用yaml格式编写的，非ini格式，为了使用列表参数。
- 2. group_vars/all文件，这是ansible的变量文件
- 3. 如果要部署其他版本的redis，注意redis_version变量必须和redis的版本完全一致



### 支持的版本
redis 5.x版本以上


### 使用
```
ansible-playbook -i hosts_redis redis.yml
```