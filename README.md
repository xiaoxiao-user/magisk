##                         安装步骤



下载并解压至目录/data/local/tmp

cd /data/local/tmp

`tar -xf magisk-template.tar`

### 安装步骤1

安装

```
sh install.sh install
```

卸载

```
sh install.sh uninstall
```

安装按成之后重启

### 安装步骤2

a、安装Magisk APP

```
pm install -r -g /data/local/tmp/modules/magisk.apk
```

完成安装之后重启

b、安装RIRU

```
magisk --install-module /data/local/tmp/modules/riru-v26.1.7.r533.2d513afd5f-debug.zip
```

完成安装之后重启

c、安装LSP

```
magisk --install-module /data/local/tmp/modules/LSPosed-v1.9.2-7024-riru-release.zip
```

当然也可通过Maigsk APP安装

完成安装之后重启



### 测试

安装测试APP 

```
pm install -r -g /data/local/tmp/AIDA64_2.02_APKPure.apk
pm install -r -g /data/local/tmp/com.test.lsp.apk
```

APP上激活的lsp测试模块,选择Hook的APP

启动APP查看Hook结果`logcat |grep -i lsp`
