# 配置

不用配置也能直接在命令行界面下工作，但有时候也需要去做点配置。先了解一下怎么配置。

## Windows

cmder 的配置文件是在 cmder 所在目录下的 `config/user-profile.sh` 。配置参考文档：[https://github.com/cmderdev/cmder](https://github.com/cmderdev/cmde)

## **macOS**

macOS 与 Linux 都属于 UNIX 类型的操作系统，所以它们有一些共通点。影响命令行界面的配置文件一般叫 `.bash_profile`，每个用户的主目录下面都有一个这样的文件，也就是不同的用户可以使用不同的配置文件。

打开命令行工具，使用在命令行界面下的编辑器去编辑这个配置文件。

```
vi ~/.bash_profile
```

`vi` 是编辑工具，`~` 表示用户主目录，`.bash_profile` 是要编辑的文件。打开文件以后，使用方向键移动光标，确定要编辑要进入编辑模式，按一下小 i ，插入下面两行配置：

```
PS1=" → "
PS1="\n$PS1"
```

按 `esc` 退出编辑模式，再输入 `:wq` ，保存并退出文件。

让配置生效可以重新打开命令行操作界面（终端），也可以执行：

```
source ~/.bash_profile
```

相关视频：[终端的提示符](https://ninghao.net/video/4557?a=51729)

