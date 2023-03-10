#  智学网的爹 - Father of ZhiXue
### 通过智学网接口获取学生考试成绩，还有一些爹独到的分析。
### 本项目正在重构：前端使用Vue+Element，后端使用Python+FastAPI。
### 代码将在重构全部完成后上传。
### [点此查看文档](https://github.com/immoses648/father-of-zhixue)（还没写捏）


## 现实现学生功能
1. 查询成绩、排名等相关信息，包括：
    - 卷面得分、满分
    - 班级（可分行政班、教学班）、年级（、联考）排名及对应参加考试人数
2. 使用ECharts对学生成绩进行可视化图形展示，包括：
    - 学生某科目中考试得分率、排名折线图（智学网改版后学生端只有得分率大致的折线图）
    - 学生某次考试的雷达图（智学网只有班级，爹可以年级和联考都显示）
3. 对考试成绩进行多维度评价，包括：
    - 学生整体偏科
    - 学生的某次考试发挥偏好或偏差
    - 学生某一科中的某次考试发挥偏好或偏差
    - 学生在某一次考试中的某一科发挥偏好或偏差
    - 学生某张试卷排名是否在前20%（比例可调）
4. 查看考试单科班级、年级、联考相关统计数据，包括：
    - 平均分
    - 中位数
    - 最高分
    - 标准差
5. 查看本班联考比例前20%的同学（比例可调）
6. 查看试卷的阅卷数据，包括：
    - 所有题目的题型、得分及得分率
    - 主观题为一评、二评、仲裁或复核，评卷人、评卷时间等
7. 查看教师版原卷（显示评卷痕迹）

等。
### 大部分功能使用POST请求同一路径即可获取json格式的数据。


## 计划实现学生功能
1. 增加更多图形展示
2. 原卷查看优化（现用iframe，手机端支持巨差）
3. 赋分功能优化（现需手动导入赋分成绩）


## 管理员实现功能
1. 登录任一学生账户查看考试数据
> 由于爹是将获取到的考试数据存入数据库中，故无需学生的账号密码也可以查看已经存在数据库中的考试数据。
2. 只有第一条。（想不出来力）



### 教师由于智学网教师端自带的功能已经足够强大，所以还没想到什么好功能可以写。
### 对爹（指这套系统）有什么想法的可以联系：
  - 邮箱：[i@immoses.com](mailto:i@immoses.com)
  - QID：immoses
  - Q群：862767072
