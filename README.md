### 导出pacman软件列表
``` bash
pacman -Qqe > pacman_pkglist.txt
```
### 导出aur软件列
``` bash
yay -Qqe --aur > yay_pkglist.txt
```
### 使用
 
#### 先安装yay 

在 **/etc/pacman.conf**中添加
```txt
[archlinuxcn]
Server = https://repo.archlinuxcn.org/$arch
```
- 然后用pacman安装就行
``` bash
sudo pacman -S yay
```
#### 用yay 导入
```bash
yay -S --needed - < pacman_pkglist.txt
```
#### chrome输入法
- 需要配置虚拟输入法