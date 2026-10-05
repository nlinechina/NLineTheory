# 治理（Governance）

## 正统（canonical）认定权

联线理论（NLineTheory）的规范与参考实现，其 canonical（正统/权威）认定权
归版权方**湖南联线智库信息科技有限公司**所有。第三方实现（无论许可合规
与否）均不构成 canonical，除非获得书面认定。认定权不可让渡。

## 维护模式

现阶段为**单人维护者模式**：

- **Maintainer**：宋淑刚（[@ssgcn](https://github.com/ssgcn)，songshugang@nlinechina.com）
- **规范变更**（Specification）：由 Maintainer 审定后发布，变更理由公开记录
- **代码变更**（Reference Implementation）：PR 审定后由 Maintainer 合并
- 理论层变更须可溯源至理论文档原文；禁止无原文依据的桥接概念进入规范

## 版本与发布

- 规范版本：`Specification vX.Y`，按重大变更/次要变更/勘误三级演进
- 参考实现版本独立编号，与规范版本的对应关系在 CHANGELOG 中声明
- **Release 权限：仅 Maintainer**。正式 release 附带不可变 tag 与
  SHA-256 清单（`releases/manifests/`）
- 已发布的不可变 release 不回写修改；错误按 [ERRATA.md](ERRATA.md) 登记，
  在后续版本中体现
- 首次公开披露（v0.1）将同步存档至 Zenodo 并获取 DOI

## 未来演进

维护者扩展、RFC 流程、委员会制等变更将在本文件修订并记录于提交历史。
