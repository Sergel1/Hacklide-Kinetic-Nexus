# Hacklide-Kinetic-Nexus

assets/hero-j1-assembly.png

Kinetic Nexus is a parametric telescoping support system designed in SolidWorks for FDM printing in PETG. The current CAD milestone includes a complete four-stage hexagonal tube set and a modeled J1 locking-joint prototype.

## Current progress

### Completed

- T1-T4 telescoping tube configurations
- Configuration-specific tube lengths, outside AF and bore AF
- T1 closed 2 mm bottom floor
- T2-T4 guide bands and pull-out stop bands
- Relieved tube bodies
- Guide-band crush ribs
- Print-oriented chamfers and corner fillets
- J1 external threaded boss on T1
- Custom 3 mm-pitch trapezoidal external thread
- Six-finger J1 collet
- J1 locking nut with matching internal thread
- Matching 8-degree collet and nut cones
- 24 external nut grip flutes
- J1 test assembly
- Interference verification between the T1 and nut threads

### Not completed yet

- J2 locking joint
- J3 locking joint
- Detents and ruler markings
- T1 grip and tripod mechanism
- Phone mount, tilt head and clamp
- Full top-level product assembly
- Printed C1 and C2 validation coupons

## Tube dimensions

| Tube | Full AF | Bore AF | Length | Relieved AF |
|---|---:|---:|---:|---:|
| T1 | 32.00 mm | 28.00 mm | 145 mm | N/A |
| T2 | 27.55 mm | 23.55 mm | 165 mm | 26.35 mm |
| T3 | 23.10 mm | 19.10 mm | 187 mm | 21.90 mm |
| T4 | 18.65 mm | 14.65 mm | 201 mm | 17.45 mm |

assets/tubes-t1-t4.png

## J1 locking joint

J1 connects T1 and T2 and contains three modeled components:

1. An external threaded boss integrated into the upper 8 mm of T1
2. A one-piece six-finger tapered collet
3. A fluted locking nut with a matching internal thread and internal cone

### J1 thread

- Pitch: 3.00 mm
- Thread depth: 1.40 mm
- Thread height: 8.00 mm
- Approximate turns: 2.667
- Flank angle: 20 degrees
- T1 thread major diameter: 38.10 mm
- T1 thread root diameter: 35.30 mm
- Nut thread crest diameter: 35.90 mm
- Nut thread root diameter: 38.70 mm

### J1 collet

- Base OD: 35.60 mm
- Top OD: 32.23 mm
- Height: 14.00 mm
- Straight lip ring: 2.00 mm
- Flexible finger length: 12.00 mm
- Hex bore AF: 26.65 mm
- Slits: six, each 0.80 mm wide
- Cone half-angle: 8 degrees

### J1 locking nut

- Outside diameter: 44.00 mm
- Height: 22.00 mm
- Thread region: 8.00 mm
- Straight cone land: 2.00 mm
- Cone region: 12.00 mm
- Cone base ID: 35.80 mm
- Cone top ID: 32.43 mm
- Grip flutes: 24

assets/j1-collet.png

assets/j1-locking-nut.png

## Verification

SolidWorks Interference Detection reported no interference between the T1 external thread and the J1 nut internal thread at the tested phase.

The rigid CAD collet can intersect the nut cone in a clamped position because the assembly does not simulate elastic PETG finger deflection. Actual thread fit, locking torque, collet flexibility, cracking resistance and holding force remain subject to physical coupon C2 testing.

assets/thread-clearance-test.png

## Repository contents

- `cad/native-solidworks/` contains native SolidWorks source files
- `cad/step/` contains neutral editable STEP exports
- `printable/` contains STL exports for printing
- `assets/` contains project screenshots
- `docs/` contains the project handoff and build specification
- `JOURNAL.md` records development progress
- `BOM.csv` contains the current bill of materials

## Opening the project

### SolidWorks

Open:

`cad/native-solidworks/Kinetic_Nexus_J1_Test_Assembly.SLDASM`

Keep the associated `.SLDPRT` files in the same folder so SolidWorks can resolve the assembly references.

### Other CAD software

Use the models in:

`cad/step/`

STEP files can be opened in applications such as FreeCAD, Fusion, Onshape and many other CAD systems.

## Manufacturing status

The CAD files are an engineering prototype and have not yet completed physical validation.

Before relying on the locking mechanism:

- Print clearance coupon C1
- Print thread-and-collet coupon C2
- Verify thread fit and nut torque
- Check the collet for cracking
- Verify pull-out-stop strength
- Perform repeated lock/unlock testing

## Documentation

Detailed dimensions, feature naming, solved errors and remaining work are documented in:

`docs/Kinetic_Nexus_Updated_Handoff_2026-10-19.docx`

## Author

Designed and modeled by Sergel Hasabella.
