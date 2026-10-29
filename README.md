<div align="center">

# Janmesh P.

**Robotics · Multi-Robot Coordination · Autonomous Systems · Embedded Engineering**

I build robotic systems and measure how they behave under congestion, timing faults, and imperfect assumptions—from planning and perception to real-time control and hardware interfaces.

`C++17` `ROS 2` `Python` `Multi-Agent Planning` `Embedded Systems`

[Featured project](https://github.com/janmesh-p/multi-robot-fleet-coordination) · [All repositories](https://github.com/janmesh-p?tab=repositories)

</div>

---

## 🚀 Featured project: Multi-Robot Fleet Coordination

**[Warehouse multi-agent pickup and delivery (MAPD)](https://github.com/janmesh-p/multi-robot-fleet-coordination)** — a C++17 fleet coordinator and grid simulator for up to **100 robots**, covering task allocation, multi-agent pathfinding, traffic management, and execution delays.

- **Coordination:** With 25 robots and 360 orders/hour offered, independent A* froze in every benchmark run; coordinated ECBS averaged **359.5 deliveries/hour** over 10 seeds.
- **Late execution:** At a 10% missed-step probability, turning off both traffic rules produced **44,170 simulated safety stops** over 80 one-hour runs. With the rules enabled, the matched experiments recorded **0**.
- **Planner trade-offs:** Under heavy load, ECBS delivered about **40% more orders** than faster-to-compute PIBT (653.3 versus 465.1 deliveries/hour with 25 robots).
- **Stage 7 map experiment:** Adding station-adjacent parking raised simulated throughput **27–34% with 50 robots** across four planners at 1,800 orders/hour offered; each planner improved in all 10 paired seeds. At 100 robots, station wait remained near 62% even on the modified map.
- **Evidence pipeline:** **35 committed CSVs from 2,140 planning runs** rebuild the README tables, with CI table checks and sampled reruns. The separate learning recheck matched **3,480 runs with zero non-timing differences**; this confirms reproducibility, not a throughput improvement.
- **Learning result:** A learned travel-time model improved prediction accuracy but did **not** pass the predefined test for higher delivery throughput against a tuned rule-based allocator.

**Status:** Grid simulation is complete through **Stage 7: benchmarks and evidence**, including communication-fault experiments and fuzz testing. **Next:** Isaac Sim, hardware-in-the-loop, and overhead perception; these stages are **planned, not yet validated**.

[Stage 7 evidence and time budgets](https://github.com/janmesh-p/multi-robot-fleet-coordination/blob/80e56439354cf715f44002435c846e2bd8b95324/README.md#benchmarks-and-evidence-stage-7) · [Learning results and limitations](https://github.com/janmesh-p/multi-robot-fleet-coordination/blob/80e56439354cf715f44002435c846e2bd8b95324/learning/README.md)

[Source, benchmark commands, and results](https://github.com/janmesh-p/multi-robot-fleet-coordination) · [Interactive algorithm atlas](https://janmeshbuilds.dev/fleet-algorithm-atlas)

## 📊 Measured performance highlights

<table>
<tr>
<td align="center" width="33%">
  <b>359.5 deliveries/h</b><br/>
  <sub>25 coordinated robots<br/>360 orders/h offered · 10 seeds</sub>
</td>
<td align="center" width="33%">
  <b>44,170 → 0</b><br/>
  <sub>simulated safety stops<br/>traffic rules off → on · 80 h</sub>
</td>
<td align="center" width="33%">
  <b>+40% throughput</b><br/>
  <sub>ECBS vs faster-to-compute PIBT<br/>25 robots · heavy load</sub>
</td>
</tr>
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
</table>

> All figures above are taken from the linked project documentation and evaluation results in this profile's repositories.

## 🧭 About

My work connects robotics algorithms to running systems: multi-robot planning, navigation, state estimation, motion control, embedded interfaces, and safety mechanisms. I focus on measurable performance, repeatable tests, and fault handling—not just successful demos.

## 🧩 Selected work

| Project | What it does | Documented highlight |
| --- | --- | --- |
| 🤖 **[Multi-robot fleet coordination](https://github.com/janmesh-p/multi-robot-fleet-coordination)**<br/><sub>C++17 · Multi-agent pathfinding · MAPD · Benchmarks</sub> | Reproducible warehouse fleet simulator with coordinated planning, order assignment, execution delays, and traffic safeguards for up to 100 robots. | **359.5 deliveries/hour** with 25 robots at 360 orders/hour offered; **0 simulated safety stops** with traffic rules on in the matched 80-hour delay experiment. |
| 🧭 **[Terrain-aware autonomous navigation](https://github.com/janmesh-p/nav2-terrain-aware-sim)**<br/><sub>ROS 2 · Nav2 · NVIDIA Isaac Sim · C++ · Python · CAN</sub> | Custom Nav2 terrain costmap layer that detects slope, roughness, and height steps from 3D lidar, with evaluation against simulator ground truth, a safety command arbiter, and a simulated drive ECU. | Safety arbiter demo reached standstill in **0.55 s** during an e-stop while turning, with documented takeover and stop behavior. |
| 🦾 **[Robot arm teleoperation](https://github.com/janmesh-p/teleop-ik-stack)**<br/><sub>ROS 2 · C++ · Eigen · Jetson Orin Nano · RealSense · Isaac Sim</sub> | Marker-driven teleoperation of a simulated Franka arm using custom inverse kinematics, a safety supervisor, and network fault testing. | **65 ms** median end-to-end capture-to-motion latency, **100 Hz** control loop, and documented no-overrun sessions. |
| 👁️ **[Stereo visual odometry](https://github.com/janmesh-p/stereo-inertial-odometry)**<br/><sub>C++17 · OpenCV · EuRoC</sub> | Metric stereo visual-odometry frontend with tracking, triangulation, PnP-RANSAC, motion-consistency gating, and trajectory evaluation. | **5.23 cm** APE RMSE, **3.60 ms** mean latency, and **0.0642%** PnP failure rate on EuRoC MH_01_easy. |
| 🔌 **[STM32 real-time sensor logger](https://github.com/janmesh-p/STM-32-Sensor-Interfacing)**<br/><sub>STM32 · FreeRTOS · C · DMA · UART</sub> | Multitasking sensor collection with RTOS queues and synchronization, DMA-backed storage, Bluetooth monitoring, and sensor fault recovery. | Built around concurrency primitives, DMA offload, and trace-based timing checks for reliable real-time behavior. |
| 🌿 **[BeagleBone environmental monitor](https://github.com/janmesh-p/smart-env-monitor)**<br/><sub>BeagleBone Black · C · Linux · GPIO · I²C · PWM · ADC</sub> | Embedded Linux environmental sensing, on-device display, actuator control, and cloud data logging. | Integrates sensing, local display, PWM control, and ThingSpeak logging using plain C on embedded Linux. |

## 🛠️ Technical focus

| Area | Tools and topics |
| --- | --- |
| 🤖 Robotics & autonomy | Multi-agent pathfinding, fleet coordination, ROS 2, Nav2, Isaac Sim, teleoperation, localization, motion control |
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
