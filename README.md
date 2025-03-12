# Lab 1: AVR Microcontroller Programming and Assembly Language

## Objective
The purpose of this lab is to introduce AVR microcontroller programming and assembly language. The task involves modifying the provided assembly program to ensure precise timing for LED toggling.

## Pre-Lab Requirements
Before beginning the lab, ensure you have completed the following:
- Read and follow the [ECE Lab Safety Guidelines](https://engineering.uiowa.edu/ece-graduate-program-overview/lab-safety-guidelines).
- (Optional) Install Atmel Studio 7.
- Review hardware and software documentation on ICON.
- Attend the mandatory 1.5-hour Lab 1 tutorial session.
- Obtain the Embedded Systems Kit during the tutorial session.

## Lab Activity
1. **Setup**: Connect two LEDs to the microcontroller using appropriate current-limiting resistors. Refer to `blinky_v5_lab01.txt` for pin selection.
2. **Testing**: Upload the provided assembly program to test LED blinking.
3. **Modify Delay Routine**: Update the `delay_long` subroutine to achieve exactly **0.3402 seconds ON** and **0.3402 seconds OFF** for each LED. Consider:
   - Counting clock cycles to determine appropriate adjustments.
   - Modifying loop counters or inserting `nop` (no operation) instructions.
   - Accounting for overhead from function calls and main loop instructions.
4. **Verification**:
   - Ensure precise timing using an oscilloscope.
   - Simulate the program to confirm expected behavior.
   - Demonstrate functionality to a TA before the deadline.

## Timing Accuracy Requirement
- 20% of the lab grade depends on achieving the exact timing requirements.
- A timing error greater than **±40 clock cycles** will result in zero credit for timing accuracy.
- Even an error of 0.0001s (100μs) translates to **1600 clock cycles**, which must be carefully accounted for.

## Submission Guidelines
- Submit your modified `main.asm` file to ICON before the deadline.
- Meet with a TA to demonstrate the correct operation, including:
  - Successfully programming the microcontroller.
  - Measuring timing accuracy using an oscilloscope.
  - Simulating the assembly program for verification.

## Notes
- Late submissions may require sign-up for a TA check-off session.
- Additional details will be provided during the lecture.

---
**Author:** Alexis Crossen  
**Course:** ECE:3360 - Embedded Systems  
**University:** University of Iowa

