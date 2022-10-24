# dnf中updateinfo命令代码跟踪

## dnf updateinfo

```
/usr/lib/python3.6/site-packages/dnf/cli/commands/updateinfo.py
```

![20221024_101052_84](image/20221024_101052_84.png)

![20221024_093926_70](image/20221024_093926_70.png)

![20221024_102428_65](image/20221024_102428_65.png)


默认就是带summay

![20221024_094058_15](image/20221024_094058_15.png)

基本步骤，

1. 实例化 ```class UpdateInfoCommand()```，执行 ```def __init__(self, cli)```
2. 执行静态方法```def set_argparser(parser):```
3. 执行配置，基于参数解析配置各种标志位，```def configure(self):```
4. 跳转具体dao方法，状态机+跳转 ```def run(self):```
5. 结束


## dnf updateinfo --summary




## dnf updateinfo --list


## dnf updateinfo --info







## 用法示例

![20221024_100325_80](image/20221024_100325_80.png)

![20221024_100348_23](image/20221024_100348_23.png)

![20221024_100408_41](image/20221024_100408_41.png)

![20221024_111247_11](image/20221024_111247_11.png)

![20221024_113611_96](image/20221024_113611_96.png)

![20221024_114413_46](image/20221024_114413_46.png) 


































































---
