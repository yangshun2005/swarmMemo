## swarm使用

### 1. swarm常用命令节选
```
# 查看swarm集群情况
docker node ls

# 初始化swarm集群的manager节点
docker swarm init --advertise-addr <IP-String>

# 修改时区和时间
cp /usr/share/zoneinfo/Asia/Shanghai  /etc/localtime

date -s "2019-05-13 22:44"

```

![be961c19a65c45e66a43447d923246fd](swarm 使用.resources/BAA32746-AB00-445D-AB2D-612964F4FBC9.png)

![50bb1b1ff4421d115df8b6930228696b](swarm 使用.resources/DCA04DF2-767B-461F-AEB3-4F95543199BA.png)

![c28515806fb121c9c034b51ab0f1e0eb](swarm 使用.resources/7734D361-5108-436B-A6B9-52AF9BF2F4B9.png)

![3be52351ee0c0e368632e8732fa5b44e](swarm 使用.resources/4E83D1BC-4076-4942-B7A9-C2436F0F3D31.png)

### 2.  部署和常用命令
![cc1f5d7768dc062153a03a852d3532d6](swarm 使用.resources/3AC486E4-9175-4F40-A4FE-B75F42CD6E07.png)

![66a4340ac22c4609eb8928912e9113bd](swarm 使用.resources/1DDD76C1-B194-44A9-A421-0493984F7ED9.png)

 ### 3. 数据持久化
![06c4940af8fa773dd8579a5d39c19b41](swarm 使用.resources/2E75B23E-C003-478D-972E-48E0147742CA.png)
 
![064065964caa7e7a74db8ab01c05cece](swarm 使用.resources/31C841BA-4925-4D9D-902C-61E8C0837ABE.png)

 ### 4.发布服务和负载均衡
 ![f40c21b9f1a4e96d8b27650687ed57d4](swarm 使用.resources/F06B09BC-2407-4E8A-85A1-7217C48BBD68.png)
 
 ![47e58c837150661ae3d0b1fd3e5f716d](swarm 使用.resources/CA47497E-C01D-4F05-B29A-D685464E9608.png)
 ![bdd70e5ff36fb1d951c90e2ac06f49bf](swarm 使用.resources/6257C876-0277-4C4A-A83D-396FAD700350.png)
 ##### 在manage节点使用 $docker network ls  可以查看集群内组网模式和信息（即可以查看有几个swarm网络）  需要注意该manage节点不比k8s的master，他仅是处理docker swarm的CURD分发命令，其生死不影响集群有效性，实现了去中心设计
![68328a2ffa966619068a39e7c0fe829c](swarm 使用.resources/4EEFFA62-AFB9-404D-9190-87CBD8FE058C.png)

### 5.服务发现
![88795d21e5301b101a00bf10adc757e8](swarm 使用.resources/D4DEDD9D-F660-4523-8066-A83E190560AB.png)
![0458a3891792a70eafbffe70e0f7dfe7](swarm 使用.resources/AAD29E21-B569-47E2-8AE3-94DF309DE55A.png)
![0c3e255ec8d2208183ff83721d1eb495](swarm 使用.resources/3F49480A-7ABA-4D3E-AB17-ACDB9AAF0F14.png)

#### 服务发现机制实例
![fb4b10f00a88700ae55a3e956d4a52b9](swarm 使用.resources/C468908B-F180-405D-B505-29E0B04BCC4C.png)
![590834b18ae0a1d9fd21759ff13d8c2a](swarm 使用.resources/C4F00911-FE69-4DCB-8836-CF2E412661DA.png)
![2122b609f738849422a12187845fb3e3](swarm 使用.resources/427F0D65-CABD-475E-A9A7-CCB73DAA219C.png)
![b67f56d8fed58e53015a4f9108e659a9](swarm 使用.resources/CBE7E5CB-43F6-4FE7-83DF-64F50DD08340.png)

### 6.高可用架构
![705b8b1b69c0ce6fabca1ef03bd917b5](swarm 使用.resources/8218DFF7-AECC-40A9-B31E-A177C6AFAE1E.png)
![77f4ad83c6e46dd20e117d22a3a5a09d](swarm 使用.resources/8965D060-D9DF-43C7-9A89-390584F81027.png)
![79db9ba153c3e9d8671218e9dd16c7d6](swarm 使用.resources/F9AEEBD1-13EA-4D0E-9546-D43A7CA24DFC.png)
![167d6354f66993fb95a3ac8030ef72ac](swarm 使用.resources/5C6CC22A-2AC0-4204-AEC5-70944D08DDF7.png)

### 7.配置文件管理
![41ce9c5c5edeacc01680dd6806f36751](swarm 使用.resources/A15AB2AC-0C82-4F4A-88F2-26D1B327D4CA.png)


### 8.实例
![a58718586c5e143e6b285d041bd23d5d](swarm 使用.resources/16D099CE-FAA0-4C29-8776-98CE5A5F9ABA.png)
```
用于swarm的DockerFile地址 ：https://drive.google.com/file/d/1sdLKMltgxHVBnvqBxTqp-A_h0UoxURBt/view?usp=sharing
```
![5a68ba1a01f3ccbf2ff984a8b192ae7f](swarm 使用.resources/78E897BF-FE9B-4639-8AB7-6B2C69ECD7F4.png)
![8518424e574527c49ee88a01a5586f04](swarm 使用.resources/30C7D4D3-88BA-46DE-8AC8-74657AFE6E53.png)







,
.
.
.
.
.,
.
.
.
.
.,
.
.
.
.
.,
.
.
.
.
.,
.
.
.
.
.












===========================================
`http://blog.51cto.com/lizhenliang`