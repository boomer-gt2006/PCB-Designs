# PCB Design Standards & Guidelines

**Team Deimos - IIT Mandi**

## 📖 Overview

This document establishes the design standards, guidelines, and best practices for all PCB designs within Team Deimos. Following these standards ensures consistency, quality, and manufacturability across all projects.

## 🎯 Design Philosophy

### Core Principles:
1. **Reliability First**: Designs must be robust and reliable
2. **Cost Effectiveness**: Optimize for cost without compromising quality
3. **Manufacturability**: Designs should be easily manufacturable
4. **Testability**: Include provisions for testing and debugging
5. **Documentation**: Comprehensive documentation for all designs

## 📏 Design Standards

### Schematic Standards

#### Symbol Libraries:
- Use IEEE standard symbols where available
- Maintain consistent symbol styles across projects
- Include part numbers and key specifications
- Use clear, readable text sizes (minimum 0.8mm)

#### Reference Designators:
- **Resistors**: R1, R2, R3...
- **Capacitors**: C1, C2, C3...
- **Inductors**: L1, L2, L3...
- **ICs**: U1, U2, U3...
- **Diodes**: D1, D2, D3...
- **Transistors**: Q1, Q2, Q3...
- **Connectors**: J1, J2, J3...
- **Test Points**: TP1, TP2, TP3...

#### Net Naming:
- Use descriptive names (VCC_3V3, CAN_HIGH, MOTOR_PWM)
- Avoid generic names (NET1, NET2)
- Use consistent naming conventions
- Include voltage levels in power nets

### PCB Layout Standards

#### Layer Stack-up:
- **2-Layer**: Signal + Ground, Signal + Power
- **4-Layer**: Signal, Ground, Power, Signal
- **6-Layer**: Signal, Ground, Signal, Power, Ground, Signal

#### Trace Width Guidelines:
| Current (A) | Trace Width (mm) | Via Size (mm) |
|-------------|------------------|---------------|
| 0.1 | 0.15 | 0.2/0.4 |
| 0.5 | 0.25 | 0.25/0.5 |
| 1.0 | 0.5 | 0.3/0.6 |
| 2.0 | 1.0 | 0.4/0.8 |
| 5.0 | 2.5 | 0.6/1.2 |

#### Spacing Requirements:
- **Minimum trace-to-trace**: 0.1mm
- **Minimum trace-to-pad**: 0.1mm  
- **Minimum via-to-via**: 0.2mm
- **Minimum drill size**: 0.15mm

#### Component Placement:
- Group related components together
- Maintain signal flow from left to right
- Place bypass capacitors close to IC power pins
- Consider thermal management in placement
- Ensure accessibility for testing and rework

#### Routing Guidelines:
- Minimize via usage on high-speed signals
- Use 45-degree angles, avoid 90-degree turns
- Route power and ground with appropriate widths
- Maintain consistent impedance for critical signals
- Separate analog and digital sections

## 🔌 Connector Standards

### Power Connectors:
- **Low Current (<2A)**: JST-PH, JST-XH
- **Medium Current (2-10A)**: XT30, Anderson Powerpole
- **High Current (>10A)**: XT60, XT90, Anderson PP45

### Signal Connectors:
- **General Purpose**: JST-PH, Molex Picoblade
- **CAN Bus**: Phoenix Contact, WAGO
- **USB**: Standard USB-A, USB-C connectors
- **Ethernet**: RJ45 with integrated magnetics

## ⚡ Power Design Guidelines

### Power Distribution:
- Use star grounding topology
- Include bulk and bypass capacitors
- Add power-on indicators (LEDs)
- Consider inrush current limiting
- Include reverse polarity protection

### Voltage Regulation:
- Use linear regulators for low noise applications
- Use switching regulators for efficiency
- Include proper input/output filtering
- Add thermal relief for high-power components

### Protection Circuits:
- **Overvoltage**: TVS diodes, Zener clamps
- **Overcurrent**: Fuses, current limiters
- **ESD**: TVS arrays on external interfaces
- **Reverse Polarity**: Schottky diodes, MOSFETs

## 📡 Signal Integrity

### High-Speed Design:
- Control impedance on critical signals
- Use differential pairs for high-speed data
- Minimize stub lengths
- Add proper termination resistors

### EMI/EMC Considerations:
- Use ground planes extensively
- Filter power supply inputs
- Add ferrite beads on power lines
- Shield sensitive circuits when necessary

## 🌡️ Thermal Management

### Heat Dissipation:
- Use thermal vias under high-power components
- Consider copper pour for heat spreading
- Add mounting holes for heat sinks
- Plan component placement for airflow

### Temperature Monitoring:
- Include temperature sensors on critical circuits
- Plan for thermal shutdown protection
- Consider component derating guidelines

## 🔧 Manufacturing Guidelines

### DFM (Design for Manufacturing):
- Follow manufacturer minimum specifications
- Use standard via sizes and drill diameters
- Maintain adequate solder mask expansion
- Include fiducial markers for assembly

### Assembly Considerations:
- Use standard component packages when possible
- Avoid components on both sides if possible
- Include component orientation markers
- Plan for automated assembly when feasible

### Testing Provisions:
- Include test points on critical nets
- Design for in-circuit testing (ICT)
- Add boundary scan for complex designs
- Include built-in self-test (BIST) where appropriate

## 📄 Documentation Requirements

### Design Files:
- Complete schematic with annotations
- PCB layout with assembly notes
- 3D visualization/rendering
- Gerber files for manufacturing
- Pick and place files for assembly

### Supporting Documentation:
- Bill of Materials (BOM) with supplier info
- Assembly drawings and instructions
- Test procedures and specifications
- Design review checklist
- Revision history and change notes

## ✅ Design Review Process

### Review Stages:
1. **Schematic Review** - Circuit functionality
2. **Layout Review** - PCB routing and placement  
3. **DRC/ERC Check** - Design rule verification
4. **Manufacturing Review** - DFM compliance
5. **Final Approval** - Sign-off for production

### Review Checklist:
- [ ] Schematic follows standards
- [ ] All components have part numbers
- [ ] Power distribution is adequate
- [ ] Signal integrity considerations addressed
- [ ] Thermal management planned
- [ ] Manufacturing requirements met
- [ ] Test provisions included
- [ ] Documentation complete

## 🚀 Advanced Design Techniques

### Multi-Board Systems:
- Use consistent connector pinouts
- Plan for inter-board communication
- Consider mechanical integration
- Standardize mounting methods

### Flexible PCBs:
- Follow bend radius guidelines
- Reinforce connection areas
- Plan for dynamic flexing
- Use appropriate materials

### RF Design:
- Control impedance carefully
- Use proper grounding techniques
- Shield sensitive circuits
- Include calibration provisions

## 📊 Quality Metrics

### Design Quality Indicators:
- DRC/ERC violation count: 0
- Via count minimization
- Layer utilization efficiency
- Component count optimization
- Manufacturing yield targets

### Performance Targets:
- Power efficiency > 85%
- Signal integrity margins > 20%
- Thermal derating > 50%
- MTBF > 10,000 hours

## 🔄 Continuous Improvement

### Feedback Collection:
- Manufacturing feedback integration
- Field failure analysis
- Performance measurement
- Cost optimization studies

### Standard Updates:
- Regular review of guidelines
- Integration of new technologies
- Best practice sharing
- Training and education

---

*Document Version: 1.0*  
*Last Updated: September 2025*  
*Next Review: March 2026*
