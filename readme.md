> windows 下 go 工程模板.

---

### 使用姿势

#### 引入项目

以引入项目 *GoMicro* 为例

1. 以 *子模块* 的方式引入到 *src* 目录下: *src/GoMicro*

2. 然后在 项目内用模块化的方式管理包. 并把第三方包缓存到 *vendor* 目录下

    ```json
    F:\a_link_workspace\go\GoWinEnv_new (master -> origin)
    $ cd src\GoMicro\
    F:\a_link_workspace\go\GoWinEnv_new\src\GoMicro (master -> origin)
    $ go mod init GoMicro
    F:\a_link_workspace\go\GoWinEnv_new\src\GoMicro (master -> origin)
    $ go mod vendor
    ```

    然后把 *vendor* ignore 掉



---

### 从新编译 tools

*bin* 目录下已经编译好了一系列工具. 如果要更新到最新的可以重新编译. 一定要 vpn 环境.



1. 弄好代理, Proxifier 代理到 ssr. 这样命令行才能走到 代理上

2. *ctrl + shift + p*, 输入 *go install*, 选择 *go: install/update tools*, 然后全选, 点击ok

    ![](http://yxbl.itengshe.com/20190908005151-1.gif)

    只要代理弄好了, 全部都能安装成功. 生成的 一些列 *exe* 会在 *bin* 目录下

    ```json
    Installing 1 tool at F:\a_link_workspace\go\GoWinEnv_new\bin
      goimports
      ...
    
    Installing golang.org/x/tools/cmd/goimports SUCCEEDED
    ...
    
    All tools successfully installed. You're ready to Go :).
    ```