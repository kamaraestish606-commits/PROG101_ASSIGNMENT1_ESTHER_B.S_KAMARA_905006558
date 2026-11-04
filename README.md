# PROG101_ASSIGNMENT1_ESTHER_B.S_KAMARA_905006558

## Project Title
Asthma Inhaler Stock Alert System 

## Problem Context
A simple, offline stock alert system that: 
1. Allows nurses to input the current number of inhalers in a ward.
2. Compares the stock to a minimum safe level (15 inhalers).
3. Displays a warning if stock is low.
4. Displays a confirmation if stockis safe.
5. Allows the nurse to check another ward without restarting.

## SDG Alignment
**SDG 3: Good Health and Well-being** - Ensuring life-saving inhalers are always available in hospitals. 

## Open Source Justification
- Free to use, saving hospitals money.
- Local IT students can fix and improve the system.
- No expensive license fees for the Sierra Leone government.

## Digital Public Goods Justification
- Designed for public benefit.
- Accessible to all clinics, even in rural areas.
- Runs offline on basic computers.

## Pseudocode
START 
              // DECLARE CONSTANTS AND VARIABLES
    CONSTANT MIN_SAFE_STOCK = 15
    VARIABLE currentStock AS INTEGER
    VARIABLE checkAnother AS STRING

    // WELCOME MESSAGE
    PRINT "Welcome to the Asthma Inhaler Stock Alert System"
    PRINT "------------------------------------------------"

    // REPETITION STRUCTURE - WHILE LOOP
    SET checkAnother = "YES"

    WHILE checkAnother == "YES" DO

        // INPUT
        PRINT "Enter the number of inhalers currently in the ward:"
        INPUT currentStock

        // DECISION STRUCTURE - IF/ELSE
        IF currentStock < MIN_SAFE_STOCK THEN
            PRINT "WARNING: Low Stock! Reorder immediately."
        ELSE
            PRINT "Stock is safe. You have ", currentStock, " inhalers."
        ENDIF

        // ASK TO REPEAT
        PRINT "Do you want to check another ward? (YES or NO)"
        INPUT checkAnother

    ENDWHILE

    // CALL FUNCTION
    CALL PrintGoodbyeMessage()

END
// FUNCTION DEFINITION
FUNCTION PrintGoodbyeMessage()

    PRINT "Thank you for keeping patients safe. System closing."

END FUNCTION

## Flowchart
<img width="680" height="1492" alt="Untitled Diagram-Page-1 drawio" src="https://github.com/user-attachments/assets/d863cd3d-075d-415b-a904-04c183b5028f" />

## Expected Output
- If stock < 15: **WARNING : Low Stock! Reorder immediately.**
- If stock >= 15: **Stock is safe.**

## Author
- Esther B. S. Kamara
- 905006558
