- 与[[接收机]]无关的数据交换格式/**R**eceiver **IN**dependent **EX**change
- 存储格式：ASCII/文本文件
- 通用性强，已成为[[全球卫星导航系统GNSS|GNSS]]测量领域的国际通用标准

### 文件结构
- **文件头**和**数据记录（文件体）**
- 一行不超过80列宽
- 文件头中每个记录的第61~80列为标签
- 读取数据取**小数点前三位**（后两位是状态码）

### 命名规则
- RINEX 2.XX版
	- 8 + 3
	- ssssdddf.yyt
	- ssss：测站名
	- ddd：年积日
	- f：时段号
	- yy：年号
	- t：文件类型
- RINEX 3.XX版
	- SSSSMRCCCS_YYYYDDDHHMMNNNFRQTT.FMT
	- SSSS：测站名
	- MR：接收机编号
	- CCC：国家代码
	- YYYYDDDHHMM：观测开始时间
	- NNN：观测时段长度
	- FRQ：采样间隔
	- TT：卫星系统+数据类型
	- FMT：rnx或crx