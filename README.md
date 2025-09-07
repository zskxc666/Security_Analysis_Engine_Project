# Security_Analysis_Engine
鉴穹日志安全分析系统
# 配置
先运行log2json.py把原始的Web日志，转化为表准JSON格式，否则无法进行分析
python log2json.py normal.log > out.json
把转化完的日志，放在data目录下面，注意默认分析data目录下第一份日志，要分析第二份需删除第一份。

# 运行
运行run-engine.bat即可开始分析

# 生成
分析完之后会在out目录生成七个文件
一个是整体的分析报告
三个简略的JSON告警报告
三个完整的JSON告警报告

# 注意事项
必须要把原始格式的日志转化为JSON格式方可识别，目前只支持apache、nginx、Tomcat日志
