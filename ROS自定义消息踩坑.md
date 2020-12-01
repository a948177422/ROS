https://blog.csdn.net/zhoudekuai/article/details/102555483

在用ros python自定义消息时碰到一个坑，在使用消息时产生：

```python
from xxx.msg import xxx

ImportError: No module named msg
```

原因是因为我代码中包含了项目名称的一个.py文件，如ros模块名称为abc,然后在python脚本中又包含了一个abc.py的文件，就会产生冲突，把abc.py文件重命令为其他名称即可。
