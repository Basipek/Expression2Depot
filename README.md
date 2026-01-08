# Expression2Depot: Personal Script Archive
![E2](https://img.shields.io/badge/Language-Expression_2-blue)

A collection of Garry's Mod Wiremod Expression 2 (E2) scripts developed since 201X. This repository serves as a timeline for my programming

> **Note:** This repository is a "Vault." The code is preserved in its original state and any contributions are, consequently, strictly theoretical.

### License:
Unless stated otherwise in any script, the code in this repository is public domain. Go wild.


## Contact and Contribution

If you have any questions regarding the development of these, or about E2 in general, feel free to contact me at basipekgaming@gmail.com



For contributions; the repo is currently a vault, so no modifications are in order. If there is an optimization or bug, it is going to be a theoretical discussion rather than an applied issue.



Thank you.

## Installation

You can put them in your data folder usually found in a path like so:



`steamapps\common\GarrysMod\garrysmod\data\expression2`



And Wiremod will load them in when you refresh the list or reboot the game.

You can also use folders.

## Documentation
W.I.P
I will be filling this table up with the description, history and usage of each script in the future.

> These scripts were written to solve specific engineering challenges within the Garry's Mod source engine environment.

| File | System | Technical Highlights (For Code Review) |
| :--- | :--- | :--- |
| `aiming_computer_v3.5_egp_chip` | **Integrated UI / ACE** | Custom Action Menu framework. Look for the EGP 3D tracking logic and the range-table interpolation used for ballistic lead. |
| `artillery_calculate-inator_2020` | **Computational Math** | Implements an iterative solver for long-range ballistics. Check the `delta-clamp` logic used to reconcile real distance vs. calculated parabolic arcs. |
| `vehicle_helicopter_control_set_ang` | **Physics / Control** | Advanced flight stabilization. Features altitude-velocity damping and automated vertical throttle compensation based on `BaseEnt` velocity. |
| `vehicle_plane_control_set_ang` | **Aerodynamics** | Translation of user-input (WASD) into local-to-world angle transformations for simulated flight surfaces (Ailerons/Elevators). |
| `firing_range_timing` | **Event Handling** | High-precision timing system. Uses the `entityDamage` event listener to manage state transitions and real-time penalty calculation. |
| `Turret_Friends (+ACF)` | **Entity Networking** | Multi-entity slaving. Uses `wirelink` arrays and string parsing (`explode`) to broadcast target vectors from a single master controller to multiple hardware entities. |
| `Weapon_Shop` | **UX / API Interfacing** | Custom interactive GUI. Utilizes `egpCursor` tracking and coordinate range-checking logic to interface with the DarkRP `moneyRequest` API. |
| `classic_commands` | **String Manipulation** | A lightweight shell for admin tasks. Features nested function calls for string explosion and player-finding by name/partial string. |
| `e2_finder_hud` | **Spatial Scanning** | Optimization-focused entity scanning. Uses `findInSphere` with model-filtering and 3D-parented EGP HUD elements. |
| `vehicle_control_v2_set_ang` | **Prop Motion** | Vehicle logic using `propFreeze` state-management and normalized steering/throttle clamping for ground vehicles. |