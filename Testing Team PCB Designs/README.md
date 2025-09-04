# Testing Team PCB Designs

![Testing Team](https://img.shields.io/badge/Testing-Team-green?style=for-the-badge)
![Validation](https://img.shields.io/badge/Quality-Assurance-orange?style=for-the-badge)

## 🧪 Mission Statement
Validate, test, and optimize PCB designs through rigorous testing protocols and real-world deployment scenarios.

## 🖼️ Current Test Subject

### Rover Motor Control PCB
<div align="center">

![Motor Control 3D](Motor%20Control/PCB_3D_view.png)
*3D view of the Rover Motor Control PCB under testing*

</div>

> **Status**: ✅ Design Complete, 🔄 Testing Phase  
> **Performance**: Exceeding expectations in initial tests

## 🚀 Current Projects

### 1. Rover Motor Control PCB
**Status**: ✅ Design Complete, 🔄 Testing Phase

Advanced motor control PCB designed specifically for rover propulsion systems with integrated sensing and communication capabilities.

#### Design Specifications:
- **Motor Driver**: MD13S high-current motor driver
- **Microcontroller**: ESP32-WROOM-32 (38-pin variant)
- **Power Input**: 22.2V via XT90 connector
- **Current Sensing**: ACS37030LLZATR-020B3 (20A range)
- **Communication**: CAN bus via SN65HVD230 transceiver
- **Power Regulation**: XL4005 step-down converter

#### Key Components:

| Component | Part Number | Quantity | Function |
|-----------|-------------|----------|----------|
| Motor Driver | MD13S | 1 | High-current motor control |
| MCU | ESP32-WROOM-32 | 1 | Main controller |
| Current Sensor | ACS37030LLZATR-020B3 | 1 | Motor current monitoring |
| CAN Transceiver | SN65HVD230 | 1 | CAN bus communication |
| Buck Converter | XL4005 | 1 | Power regulation |
| Filter Capacitor | 2200µF | 1 | Power supply filtering |
| Inductor | 33µH SMMS1770-330M | 1 | Buck converter inductor |

#### Files Available:
- `PCB_PCB_Rover_motor_2_2025-08-20.pdf` - Final PCB layout
- `BOM_Rover_motor_2025-08-16.csv` - Complete Bill of Materials
- `SCH_Rover_motor_2025-08-16.json` - Schematic in JSON format
- `PCB_PCB_PCB_Rover_motor_2_2025-08-16.json` - PCB design files
- `PCB_3D_view.png` - 3D visualization of the PCB

## 📊 Testing Protocols

### 1. Electrical Testing
- **Power-on Testing**: Verify all voltage rails
- **Communication Testing**: CAN bus functionality
- **Motor Control Testing**: PWM signal generation
- **Current Sensing Validation**: Accuracy across load range

### 2. Environmental Testing
- **Temperature Range**: -20°C to +85°C operation
- **Vibration Testing**: Rover operational conditions
- **Humidity Testing**: IP54 equivalent protection

### 3. Performance Metrics
- **Motor Response Time**: < 50ms
- **Current Measurement Accuracy**: ±2%
- **Communication Latency**: < 10ms
- **Power Efficiency**: > 90%

## 🔧 Test Equipment

### Hardware:
- Digital oscilloscope (100MHz+)
- Multimeter with current measurement
- Function generator
- Variable power supply (0-30V, 10A)
- CAN bus analyzer
- Thermal camera

### Software:
- KiCad for design verification
- CAN bus monitoring tools
- Custom test firmware (ESP32)
- Data logging applications

## 📈 Test Results Summary

### Latest Test Session (August 2025):
- ✅ **Power Rails**: All voltages within ±5% specification
- ✅ **Motor Control**: Smooth PWM operation verified
- ✅ **CAN Communication**: Error-free at 250kbps
- ⚠️ **Thermal Performance**: Some components run warm under full load
- ✅ **Current Sensing**: Accuracy within ±1.5%

### Issues Identified:
1. **Thermal Management**: Consider larger ground plane for heat dissipation
2. **Component Placement**: Optimize layout for better thermal distribution
3. **Protection**: Add additional TVS diodes for ESD protection

## 🛠️ Testing Procedures

### Pre-Test Checklist:
- [ ] Visual inspection of PCB assembly
- [ ] Continuity testing of critical nets
- [ ] Power supply verification
- [ ] Component orientation check

### Standard Test Sequence:
1. **Initial Power-up** (no load)
2. **Voltage Rail Verification**
3. **Communication Interface Testing**
4. **Motor Driver Functionality**
5. **Current Sensing Calibration**
6. **Full System Integration Test**

## 📋 Quality Assurance

### Design Review Process:
1. **Schematic Review** - Circuit functionality verification
2. **PCB Layout Review** - Signal integrity and thermal analysis
3. **Component Selection Review** - Availability and specifications
4. **Manufacturing Review** - DFM guidelines compliance

### Acceptance Criteria:
- All functional tests pass
- Thermal limits within safe margins
- EMI/EMC compliance verified
- Reliability testing completed (1000+ hour operation)

## 🚀 Future Testing Plans

### Upcoming Tests:
- [ ] Long-term reliability testing (6 months)
- [ ] EMI/EMC compliance testing
- [ ] Field testing in actual rover deployment
- [ ] Performance optimization studies

### Test Equipment Upgrades:
- [ ] Network analyzer for RF testing
- [ ] Environmental chamber for extended temp testing
- [ ] Automated test setup for regression testing

## 📞 Testing Team Contact

For test data requests, collaboration on testing procedures, or reporting issues with tested designs, please contact the Testing Team leads.

---

*Testing Team - Team Deimos IIT Mandi*  
*Last Updated: September 2025*