# Acs-ku

INSTALL GENIEACS OTOMATIS
This is autoinstall GenieACS


apt install git curl -y

git clone https://github.com/sahabatmandiri/Acs-ku.git

cd genieacs

chmod +x install.sh

bash install.sh

#=== Script update GenieACS ====#

Config sebelumnya akan terhapus dan tergantikan oleh config baru

Yang akan diupdate, yaitu:

• Admin >> Preset
• Admin >> Provosions
• Admin >> Virtual Parameter
• Admin >> Config

#===Script/config tersebut akan terganti dengan yang baru ====#

Jika anda memiliki config/script custom buatan anda sendiri,
silahkan backup terlebih dahulu, kemudian setelah update lakukan config manual lagi sesuai config custom anda.

Device, user, permisions, tidak akan terpengaruh
Bagi yang confignya error, akan ter-repair dengan script ini
Anda masih bisa kembali ke konfigurasi sebelumnya dengan memilih restore
======= CARA RESTORE ========

cd
sudo mongorestore --db=genieacs --drop genieacs-backup/genieacs
