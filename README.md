
## 添加方法

导入公钥：

```
sudo pacman-key --keyserver hkp://keyserver.ubuntu.com --recv-keys 8ED9ABE61CDBAABAC4B6A694C9218E60C13B4BA8
sudo pacman-key --lsign-key 8ED9ABE61CDBAABAC4B6A694C9218E60C13B4BA8
```
编辑`/etc/pacman.conf`
```
[shorin-arch]
Server = https://repo.shorin.xyz/archlinux/$arch
```

或者使用自动脚本：

```
curl -L repo.shorin.xyz/archlinux/gpgsetup | bash 
```