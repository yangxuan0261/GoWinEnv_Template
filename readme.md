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

