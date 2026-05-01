teamtalk-imcore跨平台核心库
主要组成：
1、netlib跨平台网络库
2、proto自定义内部协议
3、security安装加密库
4、slog自定义日志库封装
5、string字符串处理工具

编译方式：
1、进入proto目录下pb同步生成
2、开始代码编译
Linux构建方案：
    mkdir build && cd build
    cmake ../
    make
Windows构建方案：
    mkdir build && cd build
    cmake .. -G "Visual Studio 17 2022" -A Win32 ..
    # 打开生成的.sln文件进行构建
    # 或者使用命令行构建
    cmake --build . --config Release

外部依赖：
1、protobuf
2、spdlog