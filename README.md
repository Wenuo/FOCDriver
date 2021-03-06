# FOCDriver
![FocDriver](https://github.com/Wenuo/FOCDriver/blob/master/pic/FocDriver.jpg)

`FOCDriver`是一款基于`STM32F405`的无刷矢量控制驱动器系统。其硬件是来源于`ODRIVE`，我在其基础上增加了`OLED`显示屏，用来显示无刷电机的矢量状态，包括但不局限无刷电机的位置、速度信息、电源电压以及设备的温度。

硬件架构与ODRIVE一样，采用`STM32F405`作为主控，控制两路`DRV8301`无刷电机驱动器驱动3路MOS逆变电路。

板载`USB2.0、CAN、UART、SWD、`以及`GPIO`输入输出接口、还留有舵机驱动接口（刹车电路）

通过`AS5047P`、`TLE5012B`获取无刷电机转子位置，为了能更好地获取转子位置信息，我做了`2312S`无刷电机的结构体，用于装配`AS5047P`、`TLE5012B`的PCBA。形态如下：

![0002](https://github.com/Wenuo/FOCDriver/blob/master/pic/0002.png)

使用M3螺丝进行紧固。效果如下图

![0003](https://github.com/Wenuo/FOCDriver/blob/master/pic/0003.jpg)

第一版REV1.0
![REV1.0](https://github.com/Wenuo/FOCDriver/blob/master/pic/REV1.0.jpg)
