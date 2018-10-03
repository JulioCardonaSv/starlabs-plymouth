# Star Labs Plymouth Theme ![alt text](https://cdn.shopify.com/s/files/1/2059/5897/files/Star_50x.png?v=1513954416 "Star Labs Systems")
Star Labs plymouth theme

## How to install
### Ubuntu, Linux Mint, elementaryOS
##### Install
```
sudo add-apt-repository ppa:starlabs/ppa
sudo apt update
sudo apt install starlabs-theme
```
##### Uninstall
```
sudo apt remove starlabs-theme
```


### Other distributions
##### Install
```
sudo cp -r starlabs-logo/ /usr/share/plymouth/themes/
```
##### Uninstall
```
sudo rm -r /usr/share/plymouth/themes/starlabs-logo/
```
##### Enable
```
sudo update-alternatives \
		--install /usr/share/plymouth/themes/default.plymouth default.plymouth \
		/usr/share/plymouth/themes/starlabs-logo/starlabs-logo.plymouth 150 \
		--slave /usr/share/plymouth/themes/default.grub default.plymouth.grub \
		/usr/share/plymouth/themes/starlabs-logo/starlabs-logo.grub
sudo update-initramfs -u
```
##### Disable
```
sudo update-alternatives \
		--remove default.plymouth /usr/share/plymouth/themes/starlabs-logo/starlabs-logo.plymouth
sudo update-initramfs -u
```

Any issues or questions, please contact us at [support@starlabs.systems](mailto:supportstarlabs.systems)

[© Star Labs® / All Rights Reserved.](https://starlabs.systems) 

