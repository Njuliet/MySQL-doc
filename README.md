# MySQL-doc
## 数据库基本设计
##### 学生信息表information设计
| 中文名称 | 表名 | 字段属性 | 默认值 | 备注 |
|---------|-----|---------|-------|------|
| 学号 | stuid | int(4) | 从1计数 | 主码 |
| 姓名 | stuname | string(10) | 无 | 不能为空 |
| 电话 | stutel | string(11) | 无 | 不能为空 |
| 年龄 | stuage | int(4) | 无 | 1-150 |
| 性别 | stusex | string(4) | F | F女M男 |
| 状态位 | status | string(4) | 1 | 1显示0不显示|


##### 课程信息表course设计
| 中文名称 | 表名 | 字段属性 | 默认值 | 备注 |
|---------|-----|---------|-------|------|
| 课程号 | courseId | int(11) | 无 | 主码 |
| 课程名 | coursename | string(45) | 无 | 不能为空 |
| 学分  | credit | string(45) | 无 | 不能为空 |


##### 学生成绩表score设计
| 中文名称 | 表名 | 字段属性 | 默认值 | 备注 |
|---------|-----|---------|-------|------|
| 学号 | stuid | int(20) | 无 | 外码 |
| 课程号 | courseId | string(20) | 无 | 与学号共同组成本表主码 |
| 成绩 | stuscore | int(20) | 无 | 0-100 |

## 数据库具体源码
[src](https://github.com/Njuliet/code)

## 每天计划
1. [第一天](https://github.com/Njuliet/MySQL-doc/blob/master/20170612.md)
2. [第二天](https://github.com/Njuliet/MySQL-doc/blob/master/20170613.md)
3. [第三天](https://github.com/Njuliet/MySQL-doc/blob/master/20160614.md)
4. [第四天](https://github.com/Njuliet/MySQL-doc/blob/master/20170615.md)
5. [第五天](https://github.com/Njuliet/MySQL-doc/blob/master/20170616.md)
6. [第六天](https://github.com/Njuliet/MySQL-doc/blob/master/20170619.md)
7. [第七天](https://github.com/Njuliet/MySQL-doc/blob/master/20170620.md)
8. [第八天](https://github.com/Njuliet/MySQL-doc/blob/master/20170621.md)
9. [第九天](https://github.com/Njuliet/MySQL-doc/blob/master/20170622.md)
