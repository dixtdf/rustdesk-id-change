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

## linux自定义ID

找到这个文件<br>
`~/.config/rustdesk/RustDesk.toml`<br>
如果没有就新建，内容如下。 如果文件以存在需要把内容清空只保留id行。<br>

```toml
id = "MyNewID123"
```

## webtop容器 lscr.io/linuxserver/webtop:latest自定义ID
找到docker映射目录`/config`的这个文件<br>
`.config/rustdesk/RustDesk.toml`<br>
如果没有就新建，内容如下。 如果文件以存在需要把内容清空只保留id行。<br>

```toml
id = "MyNewID123"
```
