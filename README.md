# Candy Cursh Example

Candy Crush game like made in Godot, available for Android and HTML5.

## Rules

You must connect 3 pieces of the same type.

![blue](/art/Pieces/Blue%20Piece.png)![green](/art/Pieces/Green%20Piece.png)![yellow](/art/Pieces/Yellow%20Piece.png)![pink](/art/Pieces/Pink%20Piece.png)![orange](/art/Pieces/Orange%20Piece.png)![lightGreen](/art/Pieces/Light%20Green%20Piece.png)

### Blank Spaces

In the grid there are some blank spaces that will prevent or difficult connections.

### Jelly

Certain pieces will have a jelly that can be used to gain more points, you must perform certain number of connections with the pieces contained in the jelly in order to remove it.

![jelly](/art/Obstacles/Ice.png)

### Lock

Some pieces will be locked and cannot be moved, you must perform certain number of connections with the pieces contained to remove it.

![lock](/art/Obstacles/Locks.png)

### Concrete

In the grid there are some concrete pieces that will prevent or difficult connections, you can remove it by performing connections near to the concrete.

![concrete](/art/Obstacles/Concrete.png)

### Slime

Some pieces will be replaced in the grid by slime pieces, this pieces can be destroyed if a near combo is made near them. If in one turn you don't detroy any slime piece, a new slime piece will be spawned in the grid.

![slime](/art/Obstacles/Slime.png)

### Bombs

Combination of pieces can generate different bomb types:

#### Column Bomb

If four pieces combinate performing a column move (swaping vertically) a column bomb with the color of the combination will be generated. When the bomb is envolved in a combo, will destroy the entire column at his current position.

![column_bomb](/art/Pieces/Blue%20Column.png)

#### Row Bomb

If four pieces combinate performing a row move (swaping horizontally) a row bomb with the color of the combination will be generated. When the bomb is envolved in a combo, will destroy the entire row at his current position.

![row_bomb](/art/Pieces/Blue%20Row.png)

#### Adjacent Bomb

If a combination envolves at the same time tree column pieces and tree row pieces an adjacent bomb with the color of the combination will be generated. When te bomb is envolved in a combo, will destroy the surround pieces at his position no matter the color they have.

![adjacent_bomb](/art/Pieces/Blue%20Adjacent.png)

#### Color Bomb

If a combination (column, row or adjacent) has five pieces a color bomb is created. When the color bomb is swaped with another piece, all pieces of that color will be destroyed. If the piece swaped is another color bomb, all board will be cleared.

![color_bomb](/art/Pieces/Rainbow.png)

### Sinker

Sinker pieces will spawn at the first row of the board and only will be deleted when reaching the last row, sinker pieces can not be used for combinations.

![sinker](/art/Sinnker/Sinker.png)

## Game Win Conditions

Game win conditions can be configured by the designer. Number of piece combinations, eliminate an special piece like concretes, slimes, etc. The game win conditions will be displayed on the top ui.

## Game Over Conditions

Game over conditions can be by number of movements or by time, that is configured by the designer.

## Deadlock

If there are no possible combinations, the board will be remade.