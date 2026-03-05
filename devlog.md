# Dev Log — 2026-03-04
## 今日开发内容
今天开始建立项目开发日志系统，并在项目目录中创建用于记录开发过程的 Markdown 文件。
通过终端操作创建、删除和重新命名文件，最终确定使用 `devlog.md` 作为统一的开发日志文件，并使用 VS Code 进行编辑。

## 新增内容
功能：
- 建立开发日志记录机制

文件：
- devlog.md

## 修改内容
无

## 问题记录

### 问题1：

现象：  
- 尝试使用 `code devlog.md` 打开文件时终端提示：zsh: command not found: code

原因：
- VS Code 的 `code` 命令尚未被添加到系统 PATH，因此终端无法识别该命令。

解决方法：
- 在 VS Code 中安装并启用了 `code` 命令，使终端可以直接调用 VS Code。

操作步骤：
1. 打开 VS Code  
2. 按 `Cmd + Shift + P` 打开 Command Palette  
3. 搜索并执行：Shell Command: Install 'code' command in PATH

### 问题二

现象：
- 生成SSH密钥失败

原因：
- 在生成 SSH 密钥的过程中，操作步骤不熟悉，导致密钥生成流程未正确完成。

解决方法：
- 重新输入正确代码

解决步骤：
1. 重新执行生成 SSH 密钥命令：ssh-keygen -t ed25519 -C "yuboyu0131@icloud.com"

备注：
- -t：表示加密类型（type）
- -C：表示备注（comment）

### 问题三

现象：
- 在执行添加远程仓库命令时失败

原因：
- 代码语法错误

解决方法：
- 重新输入正确指令

解决步骤：
1. 输入正确指令：git remote add origin git@github.com:Relic-31/develop_practice_01.git

## 今日总结
今天完成了开发日志系统的建立，并在项目目录中创建 `devlog.md` 用于记录开发过程。

在实践过程中学习了 SSH 密钥的生成方法以及 Git 远程仓库的添加方式。

初步完成了开发环境和版本管理工具的基础配置，为后续项目开发做好了准备。

# dev log 2026-03-05

## 今日开发内容
编写了github_todo里面的基本结构

## 新增内容
功能：
- 让git不提交相关文件

文件：
- .gitignore（主文件夹）
- __pycache__/（python缓存文件夹）
- *.pyc（python缓存文件）
- .DS_Store

## 修改内容
删除了之前用于联系的几个txt文件
- hello.txt
- hello_01.txt
- hello_again.txt

## 问题记录

## 今日总结