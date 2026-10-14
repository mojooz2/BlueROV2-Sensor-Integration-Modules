# BlueROV2 Sensor Integration Modules

**Underwater robotics · Mechanical design · CAD · Rapid prototyping · Sensor integration**

Two mechanical sensor-mounting projects developed during a research internship at **POSTECH Hazardous and Extreme Environment Robotics (HERO) Lab**. Both modules were designed for integration with the **BlueROV2** remotely operated underwater vehicle.

![Full BlueROV2 CAD assembly](assets/renders/bluerov2_full_assembly_cad_1.png)

## Overview

| Project | Purpose | CAD models |
|---|---|---|
| [Two-Axis Laser Camera Pan–Tilt Mount](#1-two-axis-underwater-laser-camera-pan-tilt-mount) | Support and orient an underwater laser camera beneath the ROV | 6 STEP parts |
| [Modular Oculus M1200d Imaging Sonar Mount](#2-modular-oculus-m1200d-imaging-sonar-mount) | Integrate an imaging sonar with reconfigurable mounting geometry | 7 STEP parts |

**My work:** Mechanical CAD design, fabrication/prototyping, physical assembly, and integration of the sensor mounts with the BlueROV2 platform. The existing ROV and commercial sensors are not presented as my designs.

## 1. Two-Axis Underwater Laser Camera Pan–Tilt Mount

A mechanical mounting assembly for positioning an underwater laser camera with two rotational degrees of freedom. The assembly is suspended below the BlueROV2 frame and incorporates a circular mounting plate, supports, and links around the camera housing.

### CAD design

| Complete module | Alternate view |
|---|---|
| ![Laser camera module CAD](assets/renders/bluerov2_laser_module_cad_1.png) | ![Laser camera module CAD alternate](assets/renders/bluerov2_laser_module_cad_2.png) |

![Laser camera module CAD underside](assets/renders/bluerov2_laser_module_cad_3.png)

### Fabricated assembly

| Physical installation | Underside view |
|---|---|
| ![Laser camera mount installed](assets/photos/bluerov2_laser_module_1.png) | ![Laser camera mount underside](assets/photos/bluerov2_laser_module_2.png) |

### Underwater operation

![Underwater demonstration](assets/media/bluerov2_lasermodule_video1_gif_version.gif)

[Underwater operation (MP4)](assets/media/bluerove2_lasermodule_video1.mp4) · [Full assembly video (MOV)](assets/media/bluerov2_full_assembly_video.mov)

**CAD:** [6 STEP components](modules/laser-camera-pan-tilt/CAD/STEP/)

| File | Component |
|---|---|
| `laser_module_bearing_link.step` | Bearing link |
| `laser_module_ceiling.step` | Upper attachment |
| `laser_module_disc_link.step` | Disc link |
| `laser_module_disk.step` | Circular disc |
| `laser_module_left_part.step` | Left component |
| `laser_module_right_part.step` | Right component |

## 2. Modular Oculus M1200d Imaging Sonar Mount

A modular, truss-supported mounting structure for the **Oculus M1200d imaging sonar**. The design uses separate left and right support components and accommodates reconfiguration between **45° and 90° sonar beam orientations**.

### CAD design

| Sonar mounting assembly | Truss and interface details |
|---|---|
| ![Sonar mount CAD](assets/renders/bluerov2_sonar_module_cad_1.png) | ![Sonar truss CAD](assets/renders/bluerov2_sonar_module_cad_2.png) |

![Additional sonar mount CAD view](assets/renders/bluerov2_sonar_module_cad_3.png)

### Fabricated assembly

| Installed sonar mount | Alternate integration view |
|---|---|
| ![Sonar mount installed](assets/photos/bluerov2_sonar_module_1.png) | ![Sonar mount integration](assets/photos/bluerov2_sonar_module_2.png) |

**CAD:** [7 STEP components](modules/sonar-mount/CAD/STEP/)

| File | Component |
|---|---|
| `sonar_module_left_disc.step` | Left disc |
| `sonar_module_left_support.step` | Left support |
| `sonar_module_left_truss.step` | Left truss |
| `sonar_module_right_disc.step` | Right disc |
| `sonar_module_right_support.step` | Right support |
| `sonar_module_right_truss.step` | Right truss |
| `sonar_module_sonar_cover.step` | Sonar cover |

## Integrated BlueROV2 Assembly

| Front CAD view | Rear CAD view |
|---|---|
| ![Integrated BlueROV2 front](assets/renders/bluerov2_full_assembly_cad_1.png) | ![Integrated BlueROV2 rear](assets/renders/bluerov2_full_assembly_cad_2.png) |

The two modules are documented together because they share the BlueROV2 integration platform. The provided STEP models represent individual parts; no verified native, constrained CAD assembly is included.

## Repository contents

- `modules/laser-camera-pan-tilt/CAD/STEP/` — six laser camera mount component models
- `modules/sonar-mount/CAD/STEP/` — seven sonar mount component models
- `assets/renders/` — module and integrated-platform CAD images
- `assets/photos/` — fabricated hardware and integration photographs
- `assets/media/` — underwater GIF and video demonstrations

## Engineering notes

The images and footage document fabrication, installation, and underwater operation. They do **not** establish quantitative positioning accuracy, structural strength, environmental rating, sonar performance, or full validation of every configuration. Actuator specifications, material selections, and test measurements should only be added when verified.

## Attribution and permissions

Developed during a research internship at **POSTECH HERO Lab**. BlueROV2 and Oculus M1200d are third-party platforms/products. Publication and reuse of the CAD and research media are subject to permission from the appropriate rights holders; see [LICENSE-NOTICE.md](LICENSE-NOTICE.md). No open-source license is granted by this repository.
