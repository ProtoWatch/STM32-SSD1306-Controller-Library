# STM32 SSD1306 Controller Library
Provides abstract methods for controlling 128x32 OLED screens with the SSD1306 chip via I2C.

Capabilities include the following:
- Writing text to screen
- Displaying images in the form of bitmaps
- Drawing various shapes (lines, rectangles, circles)
- Illuminating and darkening individual pixels & arrays of pixels

## Delivables / Overview of Functions
| Title | Description | State |
| ----- | ----------- | --------- |
| Initialize Screen | Runs initializer code. | Done |
| Test Screen | Briefly illuminates and darkens screen. | Done |
| Erase Screen | Darkens entire screen (removes data stored on RAM). | *Testing |
| Erase Area | Clears an area on the screen specified by a matrix (n long, m wide) and the coordinates of the top left pixel of the matrix. | Not Started |
| Draw Text | Draws message onto screen. Drawing is based on font size and the coordinates of top left pixel of the text. | Developing |
| Draw Bitmap | Draws an area on the screen specified by a matrix (n long, m wide) and the coordinates of the top left pixel of the matrix. | Not Started |
| Draw Line | Draws a line on the screen between the coordinates of two pixels. | Not Started |
| Draw Polygon | **Draws a polygon based on location of n coordinates. | Not Started |


\* Review implementation to see if for loop at end of function is necessary or if setting page range to 0 to 7 is sufficient.
<br>\** Implementation Note: Write algorithm to maximize area inside bounded lines.