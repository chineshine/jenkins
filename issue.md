## jenkins 平时遇到的相关issue
### Required context class hudson.FilePath is missing
way:
  将  jenkinsfile 中的 ```agent none``` 改为  ```agent any```

### Jenkins 定时任务
(这个仇一定要拿小本本记下来)  
Jenkins 定时任务有两个 [Build periodically,Poll SCM]  
Build periodically => 定时构建  
Poll SCM => 定时拉取代码,如果设置了这个,job 左边会有一个 polling log,或 git pulling log ,看这个日志实际是有执行的,但这个只是定时拉取了代码
