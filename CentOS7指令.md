# Centos
firewall-cmd --list-all ##檢查是否有防火牆 

netstat -tunlp ##檢測網路相關

rpm -qa

rpm ##套件管理員 相依性問題

yum ##自動安裝 套件版本較舊，無須檢查相依性 

more,cat ##觀看

systemctl ##系統執行

man XXX ##指令目錄 

ls -a ##可顯示hidden檔案

find -readable -size 1033c ! -executable ##size為字節 ##readable可讀性

yumdownloder 套件下載器

iptables 轉port command
-A PREROUTING -p tcp -m tcp --dport 443 -j REDIRECT --to-ports 8443
-A OUTPUT -d 127.0.0.1/32 -p tcp -m tcp --dport 443 -j REDIRECT --to-ports 8443
-A OUTPUT -d 127.0.0.1/32 -p tcp -m tcp --dport 443 -j REDIRECT --to-ports 8443
