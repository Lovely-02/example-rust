# example-rust

Rust 项目模板。

## 环境要求

- [Rust](https://www.rust-lang.org/tools/install)（edition 2024）

## 快速开始

```bash
cargo run
```

## 构建

```bash
cargo build --release
```

## 测试

```bash
cargo test
```

## 支持平台

| 平台 | 架构 | 目标 |
|------|------|------|
| Windows | x86_64 | `x86_64-pc-windows-msvc` |
| Windows | aarch64 | `aarch64-pc-windows-msvc` |
| macOS | x86_64 | `x86_64-apple-darwin` |
| macOS | aarch64 | `aarch64-apple-darwin` |
| Linux | x86_64 | `x86_64-unknown-linux-gnu` |
| Linux | aarch64 | `aarch64-unknown-linux-gnu` |

## 发布流程

项目使用 [release-please](https://github.com/googleapis/release-please-action) 自动化版本管理：

1. 向 `main` 分支推送提交
2. release-please 自动生成/更新发布 PR
3. 合并发布 PR 后，CI 自动构建全部平台产物并上传至 GitHub Releases
