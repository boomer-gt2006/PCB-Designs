# Contributing to PCB-Designs

Thank you for your interest in contributing to Team Deimos PCB designs! This document provides guidelines for contributing to this repository.

## 🚀 Getting Started

1. **Fork the repository** to your GitHub account
2. **Clone your fork** locally
3. **Create a new branch** for your feature/design
4. **Make your changes** following our guidelines
5. **Submit a pull request** with a detailed description

## 📋 Design Contribution Guidelines

### File Organization
- Place files in the appropriate team folder (R&D or Testing)
- Use clear, descriptive filenames with dates
- Include version numbers for iterative designs

### Required Documentation
For each PCB design, please include:
- [ ] Complete schematic (PDF export)
- [ ] PCB layout documentation
- [ ] 3D visualization/rendering
- [ ] Bill of Materials (BOM) in CSV format
- [ ] Design specifications document
- [ ] Test results (if applicable)

### File Naming Convention
```
[ProjectName]_[Version]_[Date].extension

Examples:
- MotorController_v1.2_2025-09-05.pdf
- PowerDistribution_v2.0_2025-09-05.sch
- BOM_RoverMotor_v1.1_2025-09-05.csv
```

### Design Standards

#### Schematic Requirements:
- Use standard IEEE symbols
- Include part numbers and values
- Add design notes and explanations
- Properly annotate reference designators
- Include revision history

#### PCB Layout Requirements:
- Follow IPC standards for trace width and spacing
- Include proper ground planes
- Consider thermal management
- Add fiducials for assembly
- Include version and date on silkscreen

#### Documentation Requirements:
- Clear, professional schematics
- Assembly drawings with dimensions
- Component placement guidelines
- Manufacturing notes
- Test procedures

## 🔍 Code Review Process

### Pull Request Requirements:
1. **Clear Description**: Explain what the design does and why
2. **Design Rationale**: Justify component choices and design decisions
3. **Test Results**: Include any testing performed
4. **Manufacturing Considerations**: Note any special requirements

### Review Criteria:
- **Functionality**: Does the design meet requirements?
- **Standards Compliance**: Follows team design guidelines?
- **Documentation**: Complete and clear documentation?
- **Manufacturability**: Can it be built cost-effectively?
- **Testability**: Can the design be properly validated?

## 🛠️ Tools and Software

### Recommended Software:
- **Primary**: KiCad 7.x (open source, standardized)
- **Secondary**: Altium Designer (for complex designs)
- **3D Modeling**: FreeCAD, Fusion 360
- **Documentation**: Markdown for README files

### Design Rule Check:
- Run DRC before submitting
- Verify electrical rules (ERC)
- Check for minimum trace widths
- Validate drill sizes and via specifications

## 📊 Quality Standards

### Before Submitting:
- [ ] Schematic review completed
- [ ] PCB layout passes DRC
- [ ] BOM verified for availability
- [ ] Documentation is complete
- [ ] Files properly organized

### Testing Requirements:
- Functional testing (if prototype available)
- Design simulation results
- Thermal analysis (for power circuits)
- Signal integrity verification (for high-speed designs)

## 🚫 What Not to Submit

- Incomplete designs without documentation
- Files with DRC/ERC errors
- Proprietary designs without permission
- Designs without clear licensing
- Binary files without source files

## 🏷️ Versioning

Use semantic versioning for designs:
- **v1.0**: Initial working design
- **v1.1**: Minor improvements/bug fixes  
- **v2.0**: Major design changes

## 📞 Getting Help

### For Design Questions:
- Create an issue in the repository
- Tag appropriate team members (@r-d-team or @testing-team)
- Include relevant design files and context

### For Process Questions:
- Check existing documentation
- Ask in team discussions
- Contact repository maintainers

## 🎯 Recognition

Contributors will be:
- Listed in project documentation
- Credited in design files
- Recognized in team communications
- Invited to design review sessions

## 📄 License

By contributing to this repository, you agree that your contributions will be licensed under the same license as the project.

---

*Thank you for contributing to Team Deimos PCB designs!*
