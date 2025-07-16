


## HTBF-Dataset 介绍

### 西南交通大学复杂装备智能制造与工业软件团队智能运维课题组发布全球首个包含配套仿真模型的高速列车转向架故障（High-speed Train Bogie Fault, HTBF）数字孪生数据集。数据集中包含缩小比例的高速列车转向架故障模拟实验数据及其配套仿真模型，共计18种工况条件下的29类健康状态的多传感器数据数字孪生数据集，并且可通过配套的仿真模型进行数据扩充、验证与分析。
## 1.实验平台介绍

### 高速列车转向架故障模拟数字孪生实验台如图1、图2所示包含物理故障模拟试验台与虚拟故障仿真试验台，实验台主要包括构架、电机、齿轮箱、主轴、轮对以及轴箱等部分组成。实验台允许实验人员更换转向架传动链上的故障轴承和故障齿轮，以模拟转向架不同故障状态下的运行情况，为提高轴承与齿轮可靠性运行提供更为科学的实验数据。物理故障模拟试验台主要模拟轴箱与齿轮箱故障，轴箱轴承采用HRB 352213双列圆锥滚子轴承，齿轮箱轴承采用HRB 32305单列圆锥滚子轴承。

<img src="https://github.com/user-attachments/assets/06964a38-6f38-49b8-98d9-7a161c9bdcf3" width="700"/>

#### 图1 物理故障模拟试验台
<img width="700"  alt="微信图片_20250624153926" src="https://github.com/user-attachments/assets/731e13bb-7344-4bb7-8910-f89b13af458d" />

#### 图2 虚拟故障仿真试验台

## 2.故障模拟与实验设计

### HTBF转向架数据集包括29种健康状态的样本，其中包括齿轮箱故障、轴箱故障、复合故障三类。轴箱轴承与齿轮箱轴承分别包含四种故障形式，分别为滚动体故障、内圈故障、外圈故障与保持架故障，齿轮故障包含缺齿、断齿、齿面点蚀、齿面磨损故障形式。所有故障均由人工线切割方式产生且各类型故障包含以损伤程度为划分依据的不同等级的故障类型。如图3所示，展示了不同部件的典型模拟故障照片。 高速列车转向架故障模拟实验共包含18类运行工况，以模拟不同的高速列车运行状态。不同的电机转速模拟高速列车不同的运行速度，不同的横向载荷与纵向载荷模拟高速列车的不同负载与转向。具体工况设置见表1。

<img width="700" height="550" alt="PNG3" src="https://github.com/user-attachments/assets/29be965f-fa06-4162-87ef-a660b47006d9" />

#### 图3 轴承\齿轮故障件图片

<img width="700"  alt="工况设置" src="https://github.com/user-attachments/assets/3c6b4b39-875d-4a9e-b706-a3a40fb63bd9" />

#### 表1 实验工况设置一览表
## 3.采样设置
### 转向架故障模拟实验台布置了4套MS101050单轴加速度传感器、1套TES001T三轴加速度传感器，采集了包括轴箱、齿轮箱、电机三个测点部位的信号，共计5个通道，每个通道的采样频率均为25.6kHZ，具体传感器测点布置如图4所示。

<img width="700"  alt="传感器测点布置图(放大)" src="https://github.com/user-attachments/assets/948a2fe9-0c8f-4282-94cb-c19ed401eade" />

#### 图4 传感器测点布置图

## 4.数据文件夹结构
### HTBF转向架数据集数据存储文件夹结构与故障命名规则如图5、表2、表3所示，主文件夹名称为“High-Speed Train Bogie Fault Dataset”，其下包含具体的工况类型，例如“V1H1S1”,而每个工况文件夹下包含“Axlebox Fault”“Compound Fault”“Gearbox Fault”三类故障，最后则是对应到具体的故障类型，例如“RE1”“IR”等。每一个具体的故障类型文件夹下包含3个名称为“Sample1”“Sample2”“Sample3”CSV文件，每一个CSV文件中均包含5个通道的振动信号，其中振动信号长度为 60s。

<img width="700"  alt="文件夹结构" src="https://github.com/user-attachments/assets/03e1475e-c563-45ea-bbe7-52ab07364093" />

#### 图5 数据存储文件夹结构

<img width="750"  alt="故障命名规则" src="https://github.com/user-attachments/assets/5949182a-1201-48c2-a3d1-84cfb05043b0" />

#### 表2 故障轴承文件夹命名规则

<img width="750"  alt="齿轮故障命名规则" src="https://github.com/user-attachments/assets/57cef93b-e8be-4dda-937a-4925d639d24f" />

#### 表3 故障齿轮文件夹命名规则

## 5.采样信号示例
#### 图 6 展示了轴箱轴承故障样本振动信号的时域波形与 Hilbert 包络谱示例。

<img width="700" alt="image" src="https://github.com/user-attachments/assets/d648db12-ae47-4703-961c-4e2f91d50ca6" />


#### 图6 轴箱轴承故障振动信号示例


## 6.数据集下载与引用

### HTBF数字孪生数据集将陆续上传至该仓库，其中包括虚拟仿真模型、基线实验代码、实测信号等内容。 欢迎广大研究生、专家学者、工程师等研究人员利用该数据集进行科学研究工作，该数据集已开通了Baidu Netdisk下载渠道：[ https://pan.baidu.com/s/1fyrMASfIg6WHzV1e0JYeJQ?pwd=fps8]( https://pan.baidu.com/s/1fyrMASfIg6WHzV1e0JYeJQ?pwd=fps8)
<img width="350"  alt="下载二维码" src="https://github.com/user-attachments/assets/2d8d6447-72bf-44ac-a3c6-59d22f893ba5" />




### 如采用本试验台数据，请引用以下文献：

[1] Z. Li, K. Zhang, Q. Zheng, G. Ding, K. Ding, B. Zhang, J. Ma, H. Zhang. An Open-set Faults Diagnosis Method for Bogie Mechanical Transmission Components Based on Multi-channel Feature-enhanced Placeholder Learning[J]. **IEEE Transactions on Industrial Informatics**, 2025.

[2] Z. Li,K. Zhang, Q. Zheng, G. Ding, W. Hao, H. Zhang, W. Zhang. Unsupervised fault detection with multi-source anomaly sensitivity enhancing convolutional autoencoder for high-speed train bogie bearings[J]. **Expert Systems with Applications**, 2025.

## 7.致谢
### 感谢国家自然科学基金项目（批准号：52205130）和国家重点研发计划项目（批准号：2021YFB3400700）资助；感谢团队负责人丁国富教授和张海柱副教授及其他老师在经费申请、试验台设计过程中的大力支持，课题组成员李致萱、赖旭伟、章斌、丁昆、秦国浩、黄锋飞、王炳文、王俊人、王大龙、马嘉浩、姜进南、滕鹏涛、陈宇、陈超、洪永栋、李恒、张浩宇、崔文涛、刘纯豪、聂帅豪在实验数据采集及仿真模型构建过程中的宝贵贡献，以及浙江长兴昇阳科技有限公司协助试验台制造。
### 数据集使用过程中有任何问题，请联系:
###  张楷 zhangkai@swjtu.edu.cn
### 郑庆 qingzheng@swjtu.edu.cn






