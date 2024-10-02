# DTB_Armbian-5.3.0_Mod_HG680P

How to mod DTB

    wget https://github.com/andri-cyber/DTB_Armbian-5.3.0_Mod_HG680P/raw/refs/heads/main/hg680p_mod.dtb
    
    sudo cp hg680p_mod.dtb /boot/dtb/
    cd /boot/
    
    sudo nano boot.ini
      change boot.ini = setenv dtb_name "/dtb/hg680p_mod.dtb"

    sudo nano uEnv.ini 
      change = dtb_name=/dtb/hg680p_mod.dtb

    sudo nano /boot/extlinux/extlinux.conf
      change extlinux.conf = FDT /dtb/hg680p_mod.dtb

    reboot now

    ./done
