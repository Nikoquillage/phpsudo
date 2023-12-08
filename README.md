# phpsudo

Source code of an online Sudoku game, programmed in PHP and JavaScript

The application allows the generation of grids of any type, always ensuring a unique solution. It offers grids in various formats, ranging from 4×4 to 16×16, providing the option to use letters, numbers, or even a combination of both.

The application integrates real-time correction and includes a timer to allow you to attempt to beat your best score.

This version does not rely on a database. The grids are generated each time the application is used. It would be beneficial to consider storing the grids to significantly improve the performance of the application. 
The computation of a grid can sometimes take a significant amount of time, ranging from 5 seconds to 1 minute, depending on the selected size and difficulty. 

Demo : http://phpsudo.free.fr
