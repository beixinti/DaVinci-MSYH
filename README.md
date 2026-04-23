# ⚠️警告：在运行此脚本后，Word 软件中的宋体亦会变成黑体。如果你希望恢复，请运行 `restore.bat` 。  

# DaVinci-MSYH

DaVinci Resolve 使用简体中文时，显示的是 宋体。本项目支持在 Windows 系统上将宋体修改为微软雅黑，方便使用。

## ✏️使用方法

[在 Release 中下载 Source Code 即可。](https://github.com/beixinti/DaVinci-MSYH/releases)

若您希望使用微软雅黑，请以**管理员权限**运行 apply.bat；

如果您需要恢复，请以**管理员权限**运行 restore.bat。

## ✅测试通过版本

💻DaVinci Resolve **20** on Windows 11 x64

## 🤔原理

DaVinci Resolve 基于 Qt 框架开发的，它在中文环境下渲染难看，本质上是因为它在代码中硬编码了对特定字体（如宋体）的调用，且在 Qt 的字体匹配算法中，宋体的优先级高于微软雅黑。

通过注册表进行字体替换，让系统在达芬奇请求“宋体”时，自动给它“微软雅黑”。

## 🙏鸣谢

[知乎 - momo](https://www.zhihu.com/question/1903211161530392654)

## 字体版权声明

微软雅黑由 **方正 (Founder Type)** 设计，版权归微软所有；
宋体（中易宋体）版权归 **北京中易电子公司** 所有。
