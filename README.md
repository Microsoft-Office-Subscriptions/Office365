# Office365.ps1
## 查看 Office365 全局信息, 许可证信息等.(无需管理员权限)
```
Office365.ps1 -u <用户名> -p <密码> -l <许可证全名> -cn
        -u <用户名>
        // (可选) 用户登录的邮箱.
        -p <密码>
        // (可选) 用户登录的密码.
        -l <许可证全名>
        // (可选) 选择需要查看的许可证
        -cn 
        // *如果托管于世纪互联,则需要使用此参数.
```

## 示例
```
# 国际版
./Office365.ps1 -u moeclub@github.onmicrosoft.com -p PASSWORD

# 中国版(世纪互联)
./Office365.ps1 -u moeclub@github.partner.onmschina.cn -p PASSWORD -cn
```

# Office365_OneDrive.ps1
## 设置 OneDrive 预设网盘容量和已存在用户的网盘容量.(需要全局管理员账户)
```
Office365_OneDrive.ps1 -u <用户名> -p <密码> -q <容量> -cn
        -u <用户名>
        // (可选) 用户登录的邮箱.
        -p <密码>
        // (可选) 用户登录的密码.
        -q <容量>
        // (可选) 设置容量大小,默认:5,单位TB.
        -cn 
        // *如果托管于世纪互联,则需要使用此参数.
```

## 示例
```
# 国际版
./Office365_OneDrive.ps1 -u moeclub@github.onmicrosoft.com -p PASSWORD -q 5

# 中国版(世纪互联)
./Office365_OneDrive.ps1 -u moeclub@github.partner.onmschina.cn -p PASSWORD -q 5 -cn
```

# 报错处理
```
Set-ExecutionPolicy -ExecutionPolicy Bypass -Force
```

# 官方设置入口
```
https://<OrgName>-admin.sharepoint.com/#/settings/OneDriveStorageQuota

```

# 新手教程 [点此查看](https://github.com/MoeClub/Office365/blob/master/New.MD)

# 许可证名称-产品名称-SKU [对照表](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/licensing-service-plan-reference)
