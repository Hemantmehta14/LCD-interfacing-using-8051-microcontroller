Mt this project demonstrates how to interface an LCD with an 8051 microcontroller to display messages on the screen. The code initializes the LCD, sends commands, writes data, and displays strings on the LCD.

Hardware Connections
Pin	Function	Microcontroller Pin
RS	Register Select	P2.5
RW	Read/Write	P2.6
E	Enable	P2.7
D0-D7	Data Lines	P1.0 - P1.7

Main Program:
Set initial values for P1 and P2.
Call LCD_INIT to initialize the LCD.
Call LCD_DELAY_LONG to ensure the LCD is ready.
Display MSG1 on the first line.
Move to the second line and display MSG2.

Subroutines
LCD_INIT:
Initialize the LCD with the necessary commands.

LCD_CMD:
Send a command to the LCD.

LCD_DATA_WRITE:
Write data to the LCD.

LCD_SEND_STRING:
Send a string of characters to the LCD.


LCD_DELAY:
Generate a small delay.

LCD_DELAY_LONG:
Generate a longer delay for initialization.

Data
MSG1: First line message.
MSG2: Second line message.
