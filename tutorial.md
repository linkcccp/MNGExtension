### 添加河流

1. 在map/definition.csv文件里填写省份信息，格式为 **province;red;green;blue;x;x**
2. 在map/default.map文件里更改 **max_provinces** 值，数值为definition.csv文件里填写的最大省份代码加1
3. 由于要添加河流，在eu4里实现是将省份转变为海洋省份，所以要在map/default.map文件里的 **sea_starts** 在加上添加的省份代码
4. 在map/provinces.bmp文件里画图，同时也去除掉rivers.bmp里相对应的河流
5. 在map/heightmap.bmp文件中画图
6. 在map/area.txt中新建一个区域
7. 将新建的area添加到region.txt里对应的地区，也可以新建一个地区
8. 如何新增了一个region，那么就到map/superregion.txt里添加相对应的位置，没有则不管
9. 在map/continent.txt里将添加的省份代码填写到相对应的大洲
10. 在localisation文件夹里仿照格式本地化，[编码转换网站](https://paratranz.cn/utilities/converter)，省份文件为 **prov_names_l_english.yml** 和 **prov_names_adj_l_english.yml**
11. 添加历史，在history/provinces仿照海洋省份创建文件
12. 进入steam，eu4右键属性，在高级用户可以选择输入对启动选项的修改这里填写 
    1.  `-nudge`
13. 对模型摆放好位置之后，保存，导出的文件位于 **我的文档/Paradox Interactive/Europa Universalis IV/文件夹下，存储模型位置信息的文件为/map/position.txt**
14. 添加海峡文件 **adjacencies.csv**，仿照格式添加海峡文件，开头两个省份代码，中间sea，sea后面是海洋省份代码，然后4个 **-1**，最后注释，用英文分号隔开
14. 剪切放到自己的mod里
15. 完成

### 注意
- PS从rgb模式切换到索引模式的时候，**调版** 选择 **自定**，然后点击载入对应的 **ACT** 文件，之后确定

### 添加山脉

1. definition.csv填写省份信息
2. default.map更改省份最大值
3. provinces.bmp画图
4. 省份添加continent.txt