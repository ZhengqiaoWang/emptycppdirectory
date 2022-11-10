# Project Name

这是一个空的C++项目目录~

## 目录规范

- 项目目录
  - bin：存放编译完成的结果
  - include：引入的第三方头文件
  - common：项目公共的代码文件
  - lib：引入的三方库
  - third_party：引入的子模块
    - grpc
    - libevent
    - ....
  - interface：项目接口
  - app1：进程1或库1
    - include：进程1独自引用的第三方头文件
    - interface：进程1独自的对外接口
    - etc：配置文件
    - lib：进程1引用的三方库
    - src：进程1的代码文件
  - app2：进程2或库2
    - include：进程2独自引用的第三方头文件
    - interface：进程2独自的对外接口
    - etc：配置文件
    - lib：进程2引用的三方库
    - src：进程2的代码文件
  - ut：单元测试
    - common: 公共代码单元测试
    - app1：app1单元测试
    - app2：app2单元测试
  - tools: 项目工具集合
  - README.md 项目主页
  - .gitignore git忽略规则

目前不包括`makefile`或者`CMake`，可以根据需要设置。

目录中的`.gitkeep`文件用于让目录成功通过`git`上传，若目录存在文件则可以删除。