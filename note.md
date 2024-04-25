
# mysql源码学习笔记


## mysql的目录结构：

mysql-source/
├── README              # 源码包的说明文件或欢迎信息
├── COPYING             # 许可证文件（如GPL v2）
├── INSTALL-*           # 安装指南和其他文档
├── configure*          # 自动化配置脚本
├── aclocal.m4          # Automake宏定义
├── build/              # 构建过程中产生的中间文件和目标文件
├── cmake/              # CMake构建系统的相关文件
├── scripts/            # 构建和安装脚本
├── sql/                # MySQL核心SQL处理代码
│   ├── parser/         # SQL解析器
│   ├── lex.ll         # SQL词法分析器（Flex）
│   └── ...
├── include/            # 头文件
│   ├── mysql_version.h  # 版本信息头文件
│   ├── my_global.h     # 全局定义和宏
│   └── ...
├── libmysql/           # 客户端API库源码
├── client/             # 客户端工具（如mysql、mysqldump等）源码
├── server/             # MySQL服务器源码
│   ├── ha_*            # 各种存储引擎实现（如ha_innodb、ha_myisam等）
│   ├── plugin/         # 插件相关源码
│   ├── sql/            # 服务器端SQL处理相关代码
│   ├── storage/        # 存储层代码
│   ├── handler/        # 表处理器接口及实现
│   ├── ...
│   └── mysqld_main.cc  # 服务器主程序入口
├── mysys/              # 操作系统抽象层，包含通用工具函数和数据结构
├── strings/            # 字符串处理函数库
├── regex/              # 正则表达式库
├── dbug/               # 调试库（用于调试模式下的输出）
├── tests/              # 测试框架和测试用例
├── mysql-test/         # 完整的集成测试套件
├── man/                # 手册页源文件
├── Docs/               # 文档源文件
└── ...


