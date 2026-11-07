# 基于SpringBoot+Vue的爱心众筹系统

![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) ![Vue3](https://img.shields.io/badge/-Vue3-grey?style=flat-square) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MyBatis](https://img.shields.io/badge/-MyBatis-000000?style=flat-square&logo=mybatis&logoColor=white) 

## 项目介绍

本系统是一款面向公益互助场景的爱心众筹平台，针对求助材料分散难核验、善款流向不透明、捐助凭证难追溯以及进展公示滞后等痛点，把求助申报、平台审核、模拟捐赠、爱心证实、进展公示与提现拨付登记整合到同一套前后端分离工程中，支撑从发起筹款到资金使用回查的完整闭环。

系统采用 SpringBoot + Vue 架构，区分普通会员与系统管理员：会员端完成项目浏览筛选、模拟捐助与证书查验、发起筹款、进展发布、爱心证实与留言互动；管理员在数据看板审核项目、核对捐款与提现、管理证实留言与公益资讯，并通过 ECharts 观察筹款走势与分类占比。适合作为毕设、课设与公益数字化学习参考。

## 主要功能模块

- **用户认证与双角色分流**：会员与管理员统一登录注册，JWT 鉴权；登录后按角色进入门户首页或管理后台，/admin 路由与接口双重隔离
- **首页爱心大厅**：救助分类入口、急需接力项目、实时捐赠滚动动态与平台保障说明
- **众筹大厅检索**：按分类与筹款状态筛选，进入详情查看故事、目标进度、截止时间与捐助入口
- **模拟捐赠与电子证书**：选择金额与支付方式完成捐助，个人中心查询流水，爱心公示页校验证书编号
- **发起筹款申报**：填写受助信息、目标金额、证明材料与资金用途，提交后等待管理员审核上架
- **进展公示与善款提现**：发起人发布阶段进展与支出说明；按可提现额度申请拨付并上传费用凭证
- **爱心证实与留言互动**：社会人士提交关系背书与佐证照片；项目留言支持发起人回复与后台管理
- **公益资讯中心**：浏览政策法规、暖心救助与防诈科普等内容详情
- **经营数据看板**：累计善款、项目数、捐助人次与待审指标，筹款走势与分类占比可视化
- **项目与分类中台**：维护救助分类图片、审核上下架项目、跟踪进展动态
- **资金与互动审核**：捐款明细核对、提现审核划拨、爱心证实公示启停、留言管理
- **用户与资讯运营**：会员启停与资料维护、发布公益资讯封面与正文

## 技术架构

- **后端**：Spring Boot + MyBatis-Plus + JWT + Lombok
- **前端**：Vue 3 + TypeScript + Vue Router + Pinia + Element Plus + Vite + ECharts
- **数据库**：MySQL

<!-- screenshots-start -->
## 系统截图

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png" alt="登录页面" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E7%94%A8%E6%88%B7%E9%A6%96%E9%A1%B5.png" alt="用户首页" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E4%BC%97%E7%AD%B9%E5%A4%A7%E5%8E%85.png" alt="众筹大厅" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E5%8F%91%E8%B5%B7%E7%AD%B9%E6%AC%BE.png" alt="发起筹款" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E7%88%B1%E5%BF%83%E5%85%AC%E7%A4%BA.png" alt="爱心公示" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E7%AE%A1%E7%90%86%E5%91%98%E6%95%B0%E6%8D%AE%E7%9C%8B%E6%9D%BF.png" alt="管理员数据看板" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E5%90%8E%E5%8F%B0%E9%A1%B9%E7%9B%AE%E7%AE%A1%E7%90%86.png" alt="后台项目管理" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E5%90%8E%E5%8F%B0%E6%8D%90%E6%AC%BE%E6%98%8E%E7%BB%86.png" alt="后台捐款明细" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E8%AE%BA%E6%96%87%E5%9B%BE1.png" alt="论文图1" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/%E8%AE%BA%E6%96%87%E5%9B%BE2.png" alt="论文图2" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/charitycrowd/UML%E5%9B%BE%E5%88%97%E8%A1%A8.png" alt="UML图列表" width="600" />

<!-- screenshots-end -->

---

## 接毕业设计和论文

### 作者微信：vvsgxmn  (支持修改、 部署调试、 支持代做毕设)

### 接网站建设、小程序

### 选题+开题报告+任务书+程序定制+安装调试+论文+答辩ppt 都可以做

### 购买地址：[https://www.vvxx.love](https://www.vvxx.love)（vv毕设网）

### 支持 **一键生成 UML 图**：上传项目压缩包即可自动产出功能模块图、用例图、流程图、E-R 图、时序图等全套毕设图表。

### 提供 **免费配套软件下载 + 安装说明 + 部署教程**

![vv毕设网 - 一键画图](https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/uml-draw.png)

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/image-20260825133349317.png" alt="image-20260825133349317" />

⚠️ Bug添加微信**免费修复**，免费修复。其他平台的私信一律不管（微信方便发送文件）
