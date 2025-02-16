## sudo - Super User Do
Thực thi lệnh với quyền cao nhất

## chmod - Change Mode
Thay đổi quyền hạn của Mode

#### systax
Dùng ký tự:
```
sudo chmod u=rwx,g=rwx,o-rwx filename/folder
```

Dùng bát phân:
```
sudo chmod 765 filename/folder
```

```
lrwxrwxrwx  1 root root       7 Apr 22  2024 bin -> usr/bin
drwxr-xr-x  1 root root     512 Feb 26  2024 bin.usr-is-merged
drwxr-xr-x  1 root root     512 Apr 22  2024 boot
drwxr-xr-x  1 root root     512 Feb 16 17:19 dev
drwxr-xr-x  1 root root     512 Feb 16 17:19 etc
drwxr-xr-x  1 root root     512 Feb 16 11:05 home
-rwxr-xr-x  1 root root 2127224 Apr 25  2024 init
```
- l: link shortcut
- d: directory
- -: file
- 3 ký tự tiếp theo: quyền hạn của Own
- 3 ký tự tiếp theo: quyền hạn cho Group
- 3 ký tự tiếp theo: Other

  + w: write
  + r: red
  + x: execute


 ## chown - Change Owner
Thay đổi người sở hữu

##### Systax
```
sudo chown [owner]:[group] filename/folder
```

## groups
Xem các group

xem đang ở groups nào:
```
groups
```

xem user đang ở groups nào:
```
groups <username>
```

```
id
```
```
id <username>
```

hiển thị tất cả groups
```
cat /etc/group
```

#### add User in a Group
```
sudo usermod -aG <groupname> <username>
```

#### remove User from a Group
```
sudo gpasswd  -d <username> <groupname>
```













 
 
