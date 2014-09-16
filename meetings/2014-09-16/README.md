# Modifications To Go #

1. 以班级为核心进行管理：

    > * 创建班级页面新增入学年份，Grade表示该班级的初始年级，随时间自动更新（每年9月份）
    > * 班级列表页面隐藏过期的班级（Grade > maximal offered grade of school)；实现排序、filter(optional)；新增列学生人数列，去掉Term列
    > * Enroll Students页面新增按钮从csv导入，整体将新增学生的功能放到其下（csv导入，批量填写（姓、名、学号、家长姓名与电话、性别、所在区、所在市（默认学校注册的市）），单项填写）
    > * 班级列表页面、学生列表页面可打印
    > * 学生不设独立用户名，令用户名=roll number
    > * (Optional)搜索学生功能

2. 教师页：

    > * 新增在职状态一列、分类列（是否班主任、是否授课）
    > * 教师列表页可打印（当前）
    > * 新增教师页支持csv导入和批量填写（姓、名、教师编号、性别、出生年份、主授课科目），单条填写页与上述相同

3. 课程页：

    > * 创建课程页：去除Period与Room两项，显示顺序调整为：Term, Course, Teacher, Units(Multiple)
    > * Course简化：只记录科目（Prepopulated）；Term只显示下两个学期
