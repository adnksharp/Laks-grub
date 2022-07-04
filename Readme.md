# GRUB

Mi configuración de GRUB.

Dentro del archivo `/etc/default/grub` modifique las siguientes líneas como usuario **root**:
```Shell
GRUB_DEFUALT=saved
GRUB_SAVE_DEFAULT=true
GRUB_TIMEOUT=2
GRUB_THEME=/home/akey/.config/Lgrub
GRUB_DISABLE_SUBMENU=y
GRUB_DISABLE_OS_PROBER=false
```

Para actualizar los cambios, ejecute el comando como **root**:
```Shell
grub-mkconfig -o /boot/grub/grub.cfg
```