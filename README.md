Cracked trial acunetix for linux

Install Ubuntu or Kali Linux

```
apt install git && rm -rf /tmp/acun*
cd /tmp && git clone https://github.com/neolead/acunetix-linux.git
cd acunetix-linux && cat acupatch* > acupatch.tgz
tar -zxvf acupatch.tgz
chmod +x ./acunetix_trial.sh
sudo ./acunetix_trial.sh
cd /home/acunetix/.acunetix_trial/ && bash change_credentials.sh 
su - acunetix
bash
cp /tmp/acunetix-linux/patch_awvs /home/acunetix/.acunetix_trial/v_190515149/scanner/
cd /home/acunetix/.acunetix_trial/v_190515149/scanner/
chmod +x patch_awvs 
./patch_awvs
rm -rf /tmp/acu*
service acunetix_trial restart
curl -k https://127.0.0.1:13443
```
