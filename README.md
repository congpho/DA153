# DA153
Đây là bản mới tại thời điểm mình đăng, chú ý đây là chỉ là chia sẻ và học hỏi ko nên thương mại hóa

P/s: Chú ý bản này chỉ chạy được trên Centos 7 64bit

Cách cài:

gõ: 

yum -y install nano wget perl


wget https://raw.githubusercontent.com/congpho/DA153/master/setup.sh


chmod +x setup.sh


./setup.sh


nhập ID và lic id con số bất kỳ bạn thích


và rồi cài.

chú ý sau khi cài xong sẽ ko run được thì khai báo port cho nó

lệnh


//////////////////////// centos 7

ewall-cmd --zone=public --add-port=25/tcp --permanent

firewall-cmd --zone=public --add-port=2222/tcp --permanent

firewall-cmd --zone=public --add-port=21/tcp --permanent

firewall-cmd --zone=public --add-port=80/tcp --permanent


firewall-cmd --reload

//////////////////////

-- centos 7 --

systemctl restart directadmin 
