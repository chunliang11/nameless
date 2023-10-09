# nameless

### 简介

旨在按照较为完善的思路经验写成工具收集资产，避免重复性的工作，

目前还在完善思路的过程中一边进行书写，优化建议请提issues

![](https://github.com/chunliang11/nameless/blob/main/images/11.png)

### 步骤

ICP备案批量查询：ICP.py

DNS解析子域名：subdomain.py

子域名解析ip：domain-ip.py

端口扫描：PortScan.py


### 运行

#### ICP.py

运行`ICP.py` , `sys.agv[1]` 参数读取公司名称查找备案，建议使用爱企查导出股份穿透图数据，填充到txt中配合使用

PS：挂代理无法访问企查查，不能挂代理使用

![](https://github.com/chunliang11/nameless/blob/main/images/aiqicha.png)

![](https://github.com/chunliang11/nameless/blob/main/images/icp.png)

#### subdomain.py

运行`subdomain.py`,将自动对ICP.py中输出的文件中的域名进行解析，请在对应的地方添加key值，以正常使用

PS:本质是一个爬虫，访问网站需要代理，

![](https://github.com/chunliang11/nameless/blob/main/images/Snipaste_2023-09-22_09-52-38.png)

![](https://github.com/chunliang11/nameless/blob/main/images/doamin.png)

### domain-ip.py

运行`domain-ip.py`,将自动对subdomain.py中输出的文件中的子域名进行ip解析

![](https://github.com/chunliang11/nameless/blob/main/images/domain-ip.png)

### PortScan.py

运行`PortScan.py`,将自动对domain-ip.py中输出的文件中的ip进行端口扫描

![](https://github.com/chunliang11/nameless/blob/main/images/portscan.png)

### 更新日志

0.1
2023/9/22
- ICP备案信息查询
- DNS子域输出


0.2
2023/9/28
- subdomain脚本输出格式修改
- 增加domain-ip子域名解析ip脚本输出

0.3
2023/10/09
- 增加Portscan端口扫描脚本输出
