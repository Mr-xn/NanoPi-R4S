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

PS：
如果想手动调节风扇转速和温度匹配可以参考官方的文档-[5.13PWM风扇调节](https://wiki.friendlyelec.com/wiki/index.php/NanoPi_R4S/zh#PWM.E9.A3.8E.E6.89.87.E7.9A.84.E8.B0.83.E8.8A.82)，文件位置如下:  
<img width="547" alt="image" src="https://user-images.githubusercontent.com/18260135/187009723-b2d7ed45-9c4f-4a8e-a38f-48ee7f586300.png">


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
