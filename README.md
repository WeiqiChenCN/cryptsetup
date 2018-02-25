# cryptsetup
unlocking an rootfs encrypted with luks through a usb drive when booting

**Please try it in a virtual machine before you deploy it in a real machine.**

# Usage
- Put this file to:
`/lib/cryptsetup/scripts/decrypt_usb`
- With permission:
-rwxr-xr-x 1 root root 
- Modify `/etc/crypttab`, example:

> sda3_crypt UUID=7aa5541d-4ea2-481c-9b89-234fcadbe049 7aa5541d-4ea2-481c-9b89-234fcadbe049.luks luks,discard,keyscript=decrypt_usb
