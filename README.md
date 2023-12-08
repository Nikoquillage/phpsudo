# phpsudo

Source code of an online Sudoku game, programmed in PHP and JavaScript

The application allows the generation of grids of any type, always ensuring a unique solution. It offers grids in various formats, ranging from 4×4 to 16×16, providing the option to use letters, numbers, or even a combination of both.

The application integrates real-time correction and includes a timer to allow you to attempt to beat your best score.

This version does not rely on a database. The grids are generated each time the application is used. It would be beneficial to consider storing the grids to significantly improve the performance of the application. 
The computation of a grid can sometimes take a significant amount of time, ranging from 5 seconds to 1 minute, depending on the selected size and difficulty. 

Integration :

head>
<script src="js/jquery-3.7.1.min.js" type="text/javascript"></script>
<script src="js/phpsudo.js.php" type="text/javascript"></script>

...
/head>

body>
div id="grille">/div>

<script type="text/javascript">
$(function() {
    $('#grille').PhpSudo({
        'TailleCasePX': '35',
        'Dimension': '9*3',
        'AfficheSelectionGrilles': true,
        'AfficherLaGrille': true,
        'TailleTexte': '22',
        'GenererNouvelleGrille': true
    });
});
</script>

...
/body>

TailleCasePX : size of a box in pixels
Dimension : you can default to displaying a grid type  (9*3, 6*2, …)
AfficheSelectionGrilles : displays dropdown lists for grid selection (true or false)
AfficherLaGrille : yhe grid is displayed directly when the page is loaded
TailleTexte : size of the text in the boxes

The grid uses a "template," so you can easily change colors, fonts, and the layout of the game.

Demo : http://phpsudo.free.fr
