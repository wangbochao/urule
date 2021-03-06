# 2.1\(2017-11-06\)

* 修复在规则执行完成后返回的matchedRules值总是为空的BUG
* 采用内置的算术表达式计算器代jexl来实现算术计算，同时不再依赖jexl包
* 解决在通过客户端调用规则流，如果这个规则流中存在通过规则包调用子规则流时，客户端调用出现空指针的BUG
* 所有设计器都会在页面中直接显示加载内容或保存数据时出现服务端的错误信息，以方便规则开发人员进行调整
* 修复客户端调用中文项目下知识包出错的BUG
* 优化源码查看功能，当源码XML格式不合法不再报错，而是直接显示未格式化的XML源码
* 添加urule.debug参数，该参数值为false时规则中定义的控制台输出动作将不再执行，反之则执行，默认为true

# 2.0.5\(2017-09-27\)

* 改进核心算法，当OR节点已被其它条件节点计算通过时就不再计算余下的条件节点，减少不必要计算
* 删除jsr94部分代码实现
* 删除jsr94包依赖

# 2.0.4\(2017-08-26\)

* 修复决策表编辑器右键选择变量无法过滤且没有滚动条的BUG.
* 改进规则设计器中右键菜单选择变量过滤器过滤功能.
* 改进变量库编辑器、常量编辑器、参数编辑器表格首行过滤功能.
* 改变原仿真测试将构建好的规则包存储于HttpSession作法，不再依赖HttpSession存储.
* 改进核心引擎AND节点算法。
