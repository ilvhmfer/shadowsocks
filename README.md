
clowwindy edited this page on 17 Aug 2015 · 55 revisions
PyPI version Build Status Coverage Status

一个可穿透防火墙的快速代理。

服务端
安装
Debian / Ubuntu:

apt-get install python-pip
pip install shadowsocks
CentOS:

yum install python-setuptools && easy_install pip
pip install shadowsocks
Windows:

参见 在 Windows 上安装服务端

使用
ssserver -p 443 -k password -m rc4-md5
如果要后台运行：

sudo ssserver -p 443 -k password -m rc4-md5 --user nobody -d start
如果要停止：

sudo ssserver -d stop
如果要检查日志：

sudo less /var/log/shadowsocks.log
用 -h 查看所有参数。你也可以使用 配置文件 进行配置。

服务器搭建
建议选择 Ubuntu 14.04 LTS 作为服务器以便使用 TCP Fast Open。除非有明确理由，不建议用对新手不友好的 CentOS。

为了更好的性能，VPS 尽量选择 XEN 或 KVM，不要使用 OpenVZ。推荐使用以下 VPS：

Digital Ocean 自带的内核无需自己编译模块即可使用 hybla 算法
Linode 功能强大，机房较多
客户端
Windows / OS X
Android / iOS
OpenWRT
在你本地的 PC 或手机上使用图形客户端。具体使用参见它们的使用说明。

文档
可以在 Wiki 里找到所有的文档。

License
Copyright 2015 clowwindy

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

Bugs and Issues
Troubleshooting
Issue Tracker
Mailing list
Download	Tutorial	Wiki	Troubleshooting
