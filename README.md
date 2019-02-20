# zjubca.bounty
A decentralized bounty system powerd by EOS.

# 1 需求分析

## 1.1 任务生命周期
* 认领期：悬赏发起方公布一项悬赏任务。赏金猎人可以在此阶段可以认领任务、无视任务、拒绝任务。认领任务后，可以选择立刻使任务进入执行期。
* 执行期：认领期结束后，任务自动进入执行期。赏金猎人需要在执行期内完成任务。完成任何后，可以选择立刻进入验收期。
* 验收期：执行期结束后，任务自动进入验收期。悬赏发起方验收完任务后，任务进入完成期。
* 完成：若悬赏发起方未在验收期内完成任务的验收，则将向赏金猎人支付违约金。

# 2 开发计划
## 2.1 前端：Web端
1. [ ] 任务编辑功能
	* [ ] 任务所有内容可编辑
2. [ ] 发布、验收、管理任务功能
    * [x] 发布
    * [ ] 验收
    * [ ] 管理
3. [ ] 其他细节
    * [x] 任务呈现部分的改进
    * [x] 任务状态的颜色需要随着状态的不同而变化：黄色、绿色、蓝色、黑色。
4. [ ] 与区块链交互部分
    * [ ] 钱包、账户部分
    * [ ] 数据库部分
## 2.2 后端：智能合约
1. [ ] 测试环境
    * [ ] 测试账户、钱包设置
    * [ ] 测试网重启
    * [ ] 数据库功能实现
  

## 2.3 开发过程日志
2019-2-18前略。

2019-2-20： 修复了task无法修改内容的bug
2019-2-20： 明白了造成新建task点进去后无内容的原因。
var taskData = tasksJsonData.tasks[taskId-1];
tasks.js是从文件里读取的，所以失败。加上：task.js-137: 
2019-2-20： 大致完善了任务

# 3 功能测试

(Remove Part 1 to 3 when finish developing.)

# 4 搭建要求

# 5 DApp网址
