# PCB Checklist

This checklist is designed to guide you through the complete process of designing a PCB. It includes critical steps, ensuring that your design is accurate and ready for manufacturing. Follow each item, confirming your progress with initials and date.

> [!IMPORTANT]
The procedure needs to be executed in order as defined here. Start from number 1

## 1.ERC (Validation PCB)
- [ ] Run Electrical Rule Check (ERC) and resolve all violations
- [ ] Check for unconnected pins or nets
- [ ] Verify power, ground, and signal connections
- [ ] Check component parameters, values, and tolerances
- [ ] Confirm net labels are consistent and correctly applied
- [ ] Validate component pinouts match datasheets

## 2.Update PCB from Schematic
- [ ] Ensure schematic and PCB are synchronized
- [ ] Update PCB from schematic and verify component and net transfer
- [ ] Confirm no outdated components and Check footprint
- [ ] Validate critical component placements and component orientations
- [ ] Set and verify origin point

## 3. Repour All Polygons
- [ ] Repour all polygons on all layers
- [ ] Check polygon pour settings (clearance, thermal relief, etc.)
- [ ] Check for polygon islands and remove if necessary
- [ ] Verify thermal connections to pads
- [ ] Ensure proper clearance around vias and pads
- [ ] Ensure correct connections to ground and power planes
- [ ] Open Stack Manager and define PCB layer stack and core thickness

## 4. Design Rule Check (DRC)
- [ ] Run DRC and verify no errors
- [ ] Verify clearance constraints for all object types
- [ ] Verify minimum drill size requirements
- [ ] Check hole-to-hole spacing
- [ ] Check short circuit constraints
- [ ] Verify annular ring size meets manufacturer specs
- [ ] Check copper to board edge clearance
- [ ] Verify via sizes and types are within manufacturer capabilities
- [ ] Validate differential pair routing (if applicable)
- [ ] Check high-voltage clearance requirements

## 5. Silkscreen Preparation
- [ ] Check silkscreen text size meets manufacturer requirements
- [ ] Confirm component designators are visible and correctly placed
- [ ] Check polarity indicators for diodes, capacitors, etc.
- [ ] Include board revision number
- [ ] Add manufacturer name or logo if required
- [ ] Check for silkscreen overlapping exposed copper
- [ ] Verify text readability and orientation
- [ ] Add any necessary assembly or testing notes
- [ ] Run Silkscreen Preparation

## 6. Bill of Materials (BOM) Generation
- [ ] Generate complete BOM with all components
- [ ] Verify component parameters and values are correct
- [ ] Check part numbers and manufacturer details

## 7. Gerber Files (Check, Validate, and Final Review)
- [ ] Select appropriate Gerber format
- [ ] Include all necessary layers in Gerber output:
  - [ ] Top and bottom copper layers
  - [ ] Inner copper layers (if any)
  - [ ] Top and bottom solder mask
  - [ ] Top and bottom silkscreen
  - [ ] Board outline (mechanical layer)
  - [ ] Paste mask layers (for SMT assembly)
  - [ ] Generate NC Drill files with proper format
- [ ] Create pick-and-place files for assembly
- [ ] Check Gerber output settings (units, precision, etc.)
- [ ] Verify generated files using a Gerber viewer
- [ ] Confirm drill file matches component requirements
- [ ] Verify board dimensions in output files
- [ ] Check for proper solder mask openings
- [ ] Validate paste mask layer for SMT components
- [ ] Confirm all text is readable and not mirrored

## 8. Remove 3D on PCB (for reducing PCBdoc file size)
- [ ] Backup original file with 3D models before removal
- [ ] Remove or disable 3D models to reduce file size
- [ ] Check that file opens correctly after 3D removal
- [ ] Verify file size is appropriate for sending to manufacturer
- [ ] Create backup of original file with 3D models intact

## 9. Output Jobs and Document Files
- [ ] Create output job file with all necessary outputs
- [ ] Include special instructions for manufacturer
- [ ] Package all files according to manufacturer requirements
- [ ] Organize files in logical folder structure


# 🌟 Support Me
If you found this repository useful:
- Subscribe to my [YouTube Channel](https://www.youtube.com/@aKaReZa75).
- Share this repository with others.
- Give this repository and my other repositories a star.
- Follow my [GitHub account](https://github.com/aKaReZa75).

# ✉️ Contact Me
Feel free to reach out to me through any of the following platforms:
- 📧 [Email: aKaReZa75@gmail.com](mailto:aKaReZa75@gmail.com)
- 🎥 [YouTube: @aKaReZa75](https://www.youtube.com/@aKaReZa75)
- 💼 [LinkedIn: @akareza75](https://www.linkedin.com/in/akareza75)
