
[SSHの設定手順(Ubuntu20.04)とWindowsからのアクセス確認手順](https://aquarius-train.hatenablog.com/entry/SSH%E3%81%AE%E8%A8%AD%E5%AE%9A%E6%89%8B%E9%A0%86%28Ubuntu18_04%29%E3%81%A8Windows%E3%81%8B%E3%82%89%E3%81%AE%E3%82%A2%E3%82%AF%E3%82%BB%E3%82%B9%E7%A2%BA%E8%AA%8D%E6%89%8B%E9%A0%86)

```bash
sudo apt install -y openssh-server
dpkg -l | grep ssh
```


[ssh鍵交換](https://qiita.com/niceland/items/94499734fead10abb193)

```bash
ssh-keygen -t rsa
```

```bash
ssh-copy-id -i ~/.ssh/id_rsa nakamura@192.168.0.150
```

```bash
ssh -l nakamura 192.168.0.150 ls
```

```bash
scp -p nakamura@192.168.0.150:/home/nakamura/project/kubernetes-kanzen-nyumon-material/work/configmap.yaml ./
```
