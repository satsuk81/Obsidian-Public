(
mkdir -p ~/.ssh
chmod 700 ~/.ssh
echo [publickey] >> ~/.ssh/authorized_keys
chmod 600 ~/.ssh/authorized_keys
cat ~/.ssh/authorized_keys
sudo systemctl restart ssh
)

nano /etc/ssh/sshd_config
PasswordAuthentication no
ChallengeResponseAuthentication no

(
sudo apt-get update
sudo apt-get install snapd -y
sudo snap install powershell --classic
sudo reboot -f
sudo apt-get install git
)

(
git clone https://github.com/Seidlm/PowerShell-Backup-Script.git
cd PowerShell-Backup-Script
pwsh
get-help BackupScript_v2.ps1
)