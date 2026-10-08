> **本仓库是 [Flow Ring](https://github.com/Dongxibie/flow-ring-phase7-package) 的分阶段开发记录（第 4 步 · 环核心 RingCore）。**
> 完整产品（源码 / 截图 / 下载即用的 Windows 安装包）在 **[flow-ring-phase7-package](https://github.com/Dongxibie/flow-ring-phase7-package)**，建议从产品仓库开始了解本项目。

---

# Flow Ring · 第 4 步：环核心 RingCore

Flow Ring 是一个 Windows 桌面快捷环：按住鼠标侧键唤出悬浮圆环，把光标拖向某个方向后松开，即可执行常用动作，不用离开当前窗口。项目按开发阶段拆分为 7 个仓库，本仓库是其中的第 4 步。

## 本步骤完成内容

RingCore 完整实现与测试：

- InputStateMachine：合法迁移表 + 非法迁移异常 + EventArgs
- ProfileResolver：processName / windowTitle / windowClass / regex 匹配
- ContextEngine 接口 + NullContextEngine
- RingResolver：方向解析 + LockCenter 死区
- RingEngine：Holding → Selecting → Executing 全流程 + 子 Ring
- ActionDispatcher：按 Kind 路由 Executor

## 验证结果（阶段记录）

- RingCore 46 个 xUnit 测试全绿
