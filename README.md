# addswap

为openvz或kvm架构的linux服务器增加swap分区，请确保在root权限下使用

```bash
sudo -i 
curl -L https://raw.githubusercontent.com/spiritLHLS/addswap/main/addswap.sh -o addswap.sh && chmod +x addswap.sh && bash addswap.sh 
```

已增加openvz架构重启swap自动添加的，务必要在root根目录运行此脚本并保证脚本一直在root根目录下。

(有bug未修复，重启时swap自动删除了)

### 单位换算：输入 1024 产生 1G SWAP内存

# 致谢

kvm分区原版脚本源自 https://www.moerats.com/

```bash
curl -L https://www.moerats.com/usr/shell/swap.sh -o swap.sh && chmod +x swap.sh && bash swap.sh
```

openVZ分区原版脚本源自互联网 (作者无从考究，如有出处麻烦告知)

由 @fscarmen 指导修改优化
