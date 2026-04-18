# luci-app-diskman

一个简单的磁盘管理 LuCI 插件，支持在网页上进行分区、格式化、挂载等基本操作，支持 BTRFS RAID 以及查看硬盘状态、SMART 信息。

## 运行环境

由于插件底层的接口脚本依赖 ucode，因此需要 OpenWrt 24.10 或以上版本。

## 支持的文件系统

- ext4（及 ext2/3）
- btrfs
- xfs
- f2fs
- ntfs
- vfat（fat16/fat32）
- exfat
- swap (交换分区)

注意：格式化 ntfs 文件系统需要安装 ntfs-3g-utils 工具包。

## 编译

直接把源码拉到 OpenWrt 源码的 package 目录下，然后 `make menuconfig` 选中编译即可。

## 谢致

- https://github.com/lisaac/luci-app-diskman
