# ED3D: Transparent 3D Printer Display Concept

**ED3D** is a custom 3D printer project that integrates a transparent LCD screen in front of the build plate, allowing you to view a live 3D rendering of the print in progress. By hacking an old monitor and combining it with a Klipper-based setup, this project aims to bridge physical and digital printing with real-time visualization.

---

## Hardware

- **Display:**  
  Repurposing an old LG LCD monitor by removing its lcd thing and polarizing film to create a see-through screen effect. This enables the overlay of a virtual 3D model aligned with the physical print.  
  *Reference:* [YouTube Guide](https://www.youtube.com/watch?v=IhldXT7yxXo)

- **Controller + Computer:**  
  - **skr mini e3v3**   
  - **rpi4** running Klipper

---

##  FIRMWARE AND STUFF

- **firmware:** [Klipper](https://www.klipper3d.org/)
- **web ui:** [Mainsail](https://docs.mainsail.xyz/)

### TITLEHERE

Klipper exposes a web API endpoint(moonraker):
http://<raspberrypi-ip>/printer/objects/query?print_stats

This provides details on the current print, including the `filename` of the G-code in progress.

You can access this file at:
/home/pi/print_data/gcodes/xyz.gcode

Use this path to visualize the G-code.

---

## IDEA

Goal: Real-time display of the currently printing 3D model using `three.js` or a browser-based G-code visualizer, rendered directly on the transparent screen.

---

## MATERIALS
- **Linear Rails**: MGN12C  
- **Z Axis Drive**: Lead screw  
- **Mainboard**: BTT SKR Mini E3 V3  
- **Display**: FYSTEC Mini12864 RGB LCD  
- **Stepper Motors**: NEMA 17, 48mm  
- **Power Supply**: 24V 16.7A 400W  
- **Extruder**: Dual Gear Drive Extruder (Clone)  
- **PTFE Tube**: Capricorn PTFE Tube (Set)  
- **Heatbed**: Ender 3 Heatbed  
- **Heatbed Knobs**: Heatbed Knob Set  
- **Hotend**: V6 Hotend Set (E3D Clone)  
- **Hotend Mount**: V6 Hotend Aluminum Bracket  
- **Nozzle**: CHT 0.4mm Nozzle (Clone)  
- **Endstops**: Limit Switches  
- **Cooling Fans**: 4010 24V Cooling Fan & Blower  
- **Timing Belt**: GT2 Timing Belt (Set)  
- **Stepper Pulley**: 20T (GT2)  
- **Idler Pulley**: 16T (GT2)  
- **Smooth Idler Pulley**: 16T (GT2)  
- **Coupler**: 5mm  
- **Threaded Inserts**: M3 Threaded Heat Insert Set  
- **Washers**: M3 Washer Set  
- **Frame Material**:  
  - 1x1" Steel Tubular  
  - 1" Steel Flatbar  
  - 2020 Aluminum Profile  
- **Fasteners**:  
  - 2020 M3 T-Slot Nuts (Set)  
  - Screws  
- **Filament**:  
  - Generic ABS Filament  
  - Filament Detector  
  - Filament Detector Cable  
- **Motion Components**:  
  - Linear Shafts  
  - Linear Bearing Block  
- **Electronics**:  
  - Raspberry Pi  
  - Monitor (LCD)  
- **Tools**:  
  - Hand Tap Set  
  - Wire Spool  

##  Project Files

- [CAD](https://a360.co/3Rony1E)
- [BOM](https://docs.google.com/spreadsheets/d/178BAEs7F_joBAkZX4WfwpVy1w5ChVrZ6aIprLqq8BNg/edit?usp=sharing)
- [LOG](https://infill.hackclub.com/printers/ed3d/)

---
