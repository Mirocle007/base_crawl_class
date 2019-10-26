## base_crawl_class


### 1. 文件组织说明

<br/>

├── demo.py: 简单演示了如何使用本项目的爬虫类进行爬虫
├── myproxy.py: 用于自动获取代理IP， 检测有无proxy.txt， 无则自动爬取最新的代理IP
├── mySpider.py: 封装的爬虫类， 可以作为其他爬虫的基类
├── myUserAgent.py: 用于随机取UserAgent
├── proxy.txt: 代理IP文件， 自动生成
├── README.md: 说明文档
├── requirements.txt: 安装环境
├── useragent.txt: UserAgent文件

<br/>

### 2. 功能：

<br/>

1. 主要是实现一个爬虫的基类， 可以随机获取代理以及UserAgent, 并且可以控制访问间隔为随机访问。

<br/>

### 3. 使用：

<br/>

1. 克隆项目:
```bash
git clone https://github.com/Mirocle007/base_crawl_class.git

cd base_cral_class

```

2. 安装虚拟环境：
```bash
virtualenv -p /usr/bin/python3 venv

source venv/bin/activate

```

3. 修改demo并运行
```bash
python demo.py
```

<br/>

### 4. 问题：

<br/>

本项目主要考虑代理IP以及UserAgent的随机获取， 而没有考虑爬虫的异步, url去重等问题。