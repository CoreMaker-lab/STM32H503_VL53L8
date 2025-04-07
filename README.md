# Overview
- **Name**: STM32H503_VL53L8-V1.0
- **MCU**: STM32H503CBT6
- **IDE**: STM32CUBEMX+KEIL

  


# Contact Information

- **Name**: Billy
- **交流群**: 925643491
- **Email**: a845656974@outlook.com
- **Phone**: +86 15622736378
- **CSDN Blog**: [Blog](https://blog.csdn.net/xinzuofang)
- **Video**: [Video](https://space.bilibili.com/3546563710290070)




# Buy Link
[https://shop192352884.taobao.com/](https://shop192352884.taobao.com/)

 
# Image




# Project Introduction

- **STM32H503_VL53L8CX_Project1**:STM32H5开发VL53L8CX(1)----驱动TOF进行区域检测
- **CSDN Blog**:[https://blog.csdn.net/qq_24312945/article/details/146887467](https://blog.csdn.net/qq_24312945/article/details/146887467)
- **Video**:[https://www.bilibili.com/video/BV1VWRiYvEGU/](https://www.bilibili.com/video/BV1VWRiYvEGU/)

VL53L8CX是一款8x8多区域ToF测距传感器，它在环境光下能够在降低功耗的同时增强性能。该传感器基于意法半导体的FlightSense技术设计，能够提供最高400 cm的精确测距，并具有65°对角线视场。
VL53L8CX集成了功能强大的新一代VCSEL，以及两个先进的超表面镜头。硬件封装在创新的“一体化”模块中。这使得它能够适用于更广泛的高性能应用场景，如低功耗系统激活、手势识别、机器人SLAM、液位监控等多种用途。
VL53L8CX采用意法半导体的专利算法，可以检测和跟踪视场内的多个目标，具有64区域深度测量能力。意法半导体的直方图确保盖片玻璃串扰抗扰度超过60 cm。
与所有基于意法半导体FlightSense技术的ToF传感器一样，VL53L8CX能够测量绝对距离，不受目标颜色和反射率的影响。
VL53L8CX支持SPI和I²C接口，确保高频帧率和短启动时间。
VL53L8CX的VCSEL发射940 nm的完全不可见红外光。这种VCSEL具有1级认证，对眼睛是安全的。使用VL53L8CP可以进行场景浏览和多区域检测。这归因于软件可定制的检测阵列。它能快速且低功耗地检测到人体存在。此类检测被称为微深度图。

The VL53L8CX is an 8x8 multi-zone Time-of-Flight (ToF) ranging sensor, offering enhanced performance and reduced power consumption under ambient light conditions. Built on STMicroelectronics' FlightSense™ technology, it delivers accurate distance measurements up to 400 cm, with a 65° diagonal field of view (FoV).

The VL53L8CX integrates a powerful next-generation VCSEL emitter and two advanced metasurface lenses, all enclosed in an innovative "all-in-one" module, making it suitable for a wide range of high-performance applications such as:

Low-power system activation

Gesture recognition

Robotic SLAM

Liquid level monitoring

The sensor leverages ST’s patented algorithms to detect and track multiple targets within its FoV, offering 64-zone depth sensing. Thanks to ST's histogram technology, it provides strong immunity to crosstalk from cover glass, maintaining accuracy beyond 60 cm even with optical obstructions.

As with all ST ToF sensors based on FlightSense, the VL53L8CX measures absolute distance, unaffected by target color or reflectivity.

Key features include:

Interfaces: Supports both SPI and I²C, enabling high frame rates and fast startup times.

Emitter: Uses a 940 nm eye-safe Class 1 VCSEL that is completely invisible to the human eye.

Scene Browsing & Multi-Zone Detection: With the VL53L8CP companion software, users can customize the detection array for quick, low-power human presence detection—also known as a micro depth map.

This makes the VL53L8CX an ideal solution for next-gen applications requiring multi-zone awareness, precision, and low power consumption.



- **STM32H503_VL53L8CX_Project2**:STM32H5开发VL53L8CX(2)----设置自主模式
- **CSDN Blog**:[https://blog.csdn.net/qq_24312945/article/details/146887652](https://blog.csdn.net/qq_24312945/article/details/146887652)
- **Video**:[https://www.bilibili.com/video/BV1amRvYFEu9](https://www.bilibili.com/video/BV1amRvYFEu9)


“自主模式”（Autonomous mode）通常指的是设备或系统能够在没有外部输入的情况下独立完成任务。对于传感器，如VL53L8，自主模式可能意味着传感器可以独立、定期地进行测量，而不需要来自主控制器或主机的每一次单独指令。

选择使用自主模式的原因可能包括：
简化控制：一旦配置完成，传感器可以独立工作，减少主控制器与传感器之间的通信需求。
稳定的测量频率：在自主模式下，传感器可以以固定的频率进行测量，从而确保数据的稳定性和连续性。
减少响应延迟：由于传感器持续地或定期地进行测量，数据可能会更快地准备好，从而减少了从请求到获取数据的延迟。
主控制器工作量减少：主控制器可以被释放出来执行其他任务，而不是持续地向传感器发送测量命令。
低功耗应用：对于某些传感器，自主模式可能更加能效，因为它可以在测量之间进入低功耗状态。
实现预定任务：自主模式允许传感器在特定条件下执行预定的任务，例如当检测到某个特定值时触发警报。
然而，是否使用自主模式取决于特定的应用需求。有些应用可能更倾向于连续模式，其中主控制器更频繁地与传感器交互，以获得实时数据或更高的控制精度。


“Autonomous mode” typically refers to a device or system’s ability to operate independently without external input. For sensors like the VL53L8, autonomous mode means the sensor can perform measurements periodically and independently, without requiring individual commands from the main controller or host.

Reasons to use autonomous mode may include:
Simplified Control: Once configured, the sensor can operate on its own, reducing communication overhead between the main controller and the sensor.

Stable Measurement Frequency: In autonomous mode, the sensor can measure at a fixed frequency, ensuring data stability and continuity.

Reduced Response Latency: Since the sensor is continuously or periodically measuring, the data may be ready more quickly, reducing the delay between request and data retrieval.

Lower Host Workload: The main controller can be freed up to perform other tasks, instead of constantly sending measurement commands to the sensor.

Low-Power Applications: For some sensors, autonomous mode can be more energy-efficient, as the sensor may enter a low-power state between measurements.

Predefined Task Execution: Autonomous mode allows the sensor to carry out predefined actions under certain conditions — for example, triggering an alert when a specific value is detected.

However, whether or not to use autonomous mode depends on the specific application requirements. Some applications may favor continuous mode, where the main controller interacts more frequently with the sensor to obtain real-time data or achieve greater control precision.



































