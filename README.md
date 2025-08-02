# rustdesk-id-change

## 注意

默认服务器不允许修改ID，需要使用自建服务器。<br>
修改ID前把RustDesk客户端全部关闭。<br>

## win自定义ID

找到这个文件<br>
`C:\Windows\ServiceProfiles\LocalService\AppData\Roaming\RustDesk\config\RustDesk.toml`<br>
如果没有就新建，内容如下。 如果文件以存在需要把内容清空只保留id行。<br>

```toml
id = "MyNewID123"
```

## android自定义ID

找到这个文件<br>
`/data/user/0/com.carriez.flutter_hbb/app_flutter/RustDesk.toml`<br>
如果没有就新建，内容如下。 如果文件以存在需要把内容清空只保留id行。<br>

```toml
id = "MyNewID123"
```

## linux自定义ID(普通用户)

1.修改自建服务器配置<br>
2.关闭rustdesk服务，设置->常规->服务->停止<br>
3.找到这个文件`~/.config/rustdesk/RustDesk.toml`<br>
4.如果没有就新建，内容如下。 如果文件以存在需要把内容清空只保留id行。<br>
```toml
id = "MyNewID123"
```
5.打开rustdesk gui,__切记不要启动服务__,此时启动服务id会重新生成<br>
6.重新打开`~/.config/rustdesk/RustDesk.toml`,复制其中的enc_id行<br>
7.打开rustdesk gui,启动服务<br>
8.再次关闭rustdesk服务，设置->常规->服务->停止<br>
9.将第6步的enc_id行替换到`~/.config/rustdesk/RustDesk.toml`的enc_id行<br>
10.打开rustdesk gui,启动服务,此时id应该已经改变了<br>


## linux自定义ID(仅root用户)

找到这个文件<br>
`~/.config/rustdesk/RustDesk.toml`<br>
如果没有就新建，内容如下。 如果文件以存在需要把内容清空只保留id行。<br>

```toml
id = "MyNewID123"
```
