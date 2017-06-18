# 恢复 MI 6 的 NFC-SIM 功能
恢复小米 MI 6 的 NFC-SIM 功能。

## 更新日志
v1

    - 第一版 （First Attempt）

## 恢复说明
1. 修改 `\system\build.prop` 中
```
ro.se.type=eSE,HCE,UICC
```
2. 修改 `\system\etc\libnfc-nxp.conf` 中
```
NXP_NFCC_STANDBY_TIMEOUT=20000
```
   （此处需要替换整个文件）

3. 替换 `\system\vendor\lib64\hw\nfc_nci.nqx.default.so`