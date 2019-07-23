# Custom Grub Theme For Dual Boot - Ubuntu/Windows
Grub theme costumization from tela. For dual boot (ubuntu and windows)


 ### Notes:
 1. Edit **_"boot/grub/grub.cfg"_** (find and add classname):
    - Windows:
    ```
    menuentry "Windows" --class windows**{
    .....................
    }
    ```
    -Ubuntu:
    ```
    menuentry "Ubuntu" --class ubuntu --class gnu-linux [Other Flags] { ..................
    ...............
    }
    ```
    -Bios:
    ```
    menuentry "System Setup" --class driver $menuentry_id_option 'uefi-firmware' {
		fwsetup
    }
    ```
    
  2. Add theme archive **_(Custom_tela_grubtheme.tar.gz)_** with grub-customizer.
  
  3. Save and exit.
  
  ### Screenshots
  
![Grub Menu](ScreenShots/Screenshot.png?raw=true "Title")

![Grub Menu](ScreenShots/Screenshot2.png?raw=true "Title")
  
  

