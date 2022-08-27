# NanoPi R4S Firmware

> 添加CPU 温度风扇控制脚本(适配r2s 和 r4s)，来源官方仓库  
> 详见 https://github.com/Mr-xn/NanoPi-R4S/blob/main/scripts/lean.sh#L119  
```
# Add cpu temperature
curl -sfL https://github.com/friendlyarm/friendlywrt/raw/master-v22.03/target/linux/rockchip/armv8/base-files/usr/bin/fa-fancontrol-direct.sh --create-dirs -o target/linux/rockchip/armv8/base-files/usr/bin/fa-fancontrol-direct.sh
curl -sfL https://github.com/friendlyarm/friendlywrt/raw/master-v22.03/target/linux/rockchip/armv8/base-files/usr/bin/fa-fancontrol.sh --create-dirs -o target/linux/rockchip/armv8/base-files/usr/bin/fa-fancontrol.sh
curl -sfL https://github.com/friendlyarm/friendlywrt/raw/master-v22.03/target/linux/rockchip/armv8/base-files/etc/init.d/fa-fancontrol --create-dirs -o target/linux/rockchip/armv8/base-files/etc/init.d/fa-fancontrol
chmod +x target/linux/rockchip/armv8/base-files/etc/init.d/fa-fancontrol target/linux/rockchip/armv8/base-files/usr/bin/fa-fancontrol*.sh
```

## Tips
* Default Gateway: 192.168.2.1
* Default Password: password

## Features
* [SuLingGG/OpenWrt-Rpi/README.md](https://github.com/SuLingGG/OpenWrt-Rpi/blob/main/README.md)

## References
* https://github.com/SuLingGG/OpenWrt-Rpi
* https://github.com/coolsnowwolf/lede
* https://github.com/immortalwrt/immortalwrt
* https://github.com/friendlyarm/friendlywrt
* https://github.com/P3TERX/Actions-OpenWrt
