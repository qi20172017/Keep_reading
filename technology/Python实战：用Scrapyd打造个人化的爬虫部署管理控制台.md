![](D:\qifumin_work\keep_reading\Keep_reading\img\20200429160545.png)

---------------------------------------------

来自掘金小册

### 开篇

爬虫部署还是不部署取决于项目需求，也要考虑目标数据的时效性。

部署：数据更新频繁

不部署：十天半个月还不会有新数据的，这种爬一下就行了

### 基础篇一：安装与启动

#### 1，本地安装与启动

很常规，用pip install 安装就行了

启动  直接scrapyd

#### 2，在linux中：

配置远程需要修改一下配置文件

pip3 show scrapyd    查找scrapyd的位置

> 是`/site-packages/scrapyd/`下，有一个名为`default_scrapyd.conf`的文件，其中有个设`bind_address`，将其修改为`0.0.0.0`后保存，然后在服务器上重启 Scrapyd 服务即可。