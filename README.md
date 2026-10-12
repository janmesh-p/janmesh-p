<div align="center">

# Janmesh P.

**Robotics · Autonomous Systems · Embedded Engineering**

I build and validate robotic systems across perception, navigation, real-time control, and hardware integration.

`ROS 2` `C++` `Python` `Embedded Systems` `Safety-Critical Control`

[Explore projects](https://github.com/janmesh-p?tab=repositories) · [GitHub profile](https://github.com/janmesh-p)

</div>

---

## 📊 Verified performance highlights

<table>
<tr>
<td align="center" width="33%">
  <b>65 ms p50</b><br/>
  <sub>capture → arm motion latency<br/>teleoperation stack</sub>
</td>
<td align="center" width="33%">
  <b>100 Hz</b><br/>
  <sub>control loop rate<br/>p99 period 10.1 ms</sub>
</td>
<td align="center" width="33%">
  <b>5.23 cm</b><br/>
  <sub>APE RMSE on<br/>EuRoC MH_01_easy</sub>
</td>
</tr>
<tr>
<td align="center" width="33%">
  <b>3.60 ms</b><br/>
  <sub>mean stereo-VO frontend latency<br/>release build</sub>
</td>
<td align="center" width="33%">
  <b>0.0642%</b><br/>
  <sub>PnP failure rate<br/>3115 stereo frames</sub>
</td>
<td align="center" width="33%">
  <b>0.55 s</b><br/>
  <sub>e-stop standstill time<br/>safety arbiter demo</sub>
</td>
</tr>
</table>

> All figures above are taken from the linked project documentation and evaluation results in this profile's repositories.

## 🧭 About

My work connects robotics algorithms to running systems: from sensor processing and state estimation to motion commands, embedded interfaces, and safety controls. I focus on measurable performance, repeatable tests, and fault handling—not just successful demos.

## 🧩 Selected work

| Project | What it does | Documented highlight |
| --- | --- | --- |
| 🧭 **[Terrain-aware autonomous navigation](https://github.com/janmesh-p/nav2-terrain-aware-sim)**<br/><sub>ROS 2 · Nav2 · NVIDIA Isaac Sim · C++ · Python · CAN</sub> | Custom Nav2 terrain costmap layer that detects slope, roughness, and height steps from 3D lidar, with evaluation against simulator ground truth, a safety command arbiter, and a simulated drive ECU. | Safety arbiter demo reached standstill in **0.55 s** during an e-stop while turning, with documented takeover and stop behavior. |
| 🦾 **[Robot arm teleoperation](https://github.com/janmesh-p/teleop-ik-stack)**<br/><sub>ROS 2 · C++ · Eigen · Jetson Orin Nano · RealSense · Isaac Sim</sub> | Marker-driven teleoperation of a simulated Franka arm using custom inverse kinematics, a safety supervisor, and network fault testing. | **65 ms** median end-to-end capture-to-motion latency, **100 Hz** control loop, and documented no-overrun sessions. |
| 👁️ **[Stereo visual odometry](https://github.com/janmesh-p/stereo-inertial-odometry)**<br/><sub>C++17 · OpenCV · EuRoC</sub> | Metric stereo visual-odometry frontend with tracking, triangulation, PnP-RANSAC, motion-consistency gating, and trajectory evaluation. | **5.23 cm** APE RMSE, **3.60 ms** mean latency, and **0.0642%** PnP failure rate on EuRoC MH_01_easy. |
| 🔌 **[STM32 real-time sensor logger](https://github.com/janmesh-p/STM-32-Sensor-Interfacing)**<br/><sub>STM32 · FreeRTOS · C · DMA · UART</sub> | Multitasking sensor collection with RTOS queues and synchronization, DMA-backed storage, Bluetooth monitoring, and sensor fault recovery. | Built around concurrency primitives, DMA offload, and trace-based timing checks for reliable real-time behavior. |
| 🌿 **[BeagleBone environmental monitor](https://github.com/janmesh-p/smart-env-monitor)**<br/><sub>BeagleBone Black · C · Linux · GPIO · I²C · PWM · ADC</sub> | Embedded Linux environmental sensing, on-device display, actuator control, and cloud data logging. | Integrates sensing, local display, PWM control, and ThingSpeak logging using plain C on embedded Linux. |

## 🛠️ Technical focus

| Area | Tools and topics |
| --- | --- |
| 🤖 Robotics & autonomy | ROS 2, Nav2, Isaac Sim, teleoperation, localization, motion control |
| 👁️ Perception & estimation | stereo visual odometry, lidar terrain analysis, tracking, pose estimation |
| 🔧 Systems software | C, C++, Python, Linux, instrumentation, testing, fault handling |
| ⚙️ Embedded & hardware | STM32, FreeRTOS, Jetson, BeagleBone Black, CAN, UART, I²C, DMA |

## 📈 GitHub activity

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=janmesh-p&show_icons=true&hide_border=true&include_all_commits=true&rank_icon=github&theme=transparent" alt="GitHub activity statistics for janmesh-p" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=janmesh-p&layout=compact&hide_border=true&theme=transparent" alt="Top languages for janmesh-p" />

[View contribution history on GitHub →](https://github.com/janmesh-p?tab=overview)

</div>

---

<div align="center">

[All repositories →](https://github.com/janmesh-p?tab=repositories)

</div>
