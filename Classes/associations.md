| Assoziation   | Zwischen Klasse | und Klasse         | Multiplizität  |
|---------------|-----------------|---------------------|-----------------|
| Vererbung     | Knight          | Piece               | -               |
| Vererbung     | Queen           | Piece               | -               |
| Vererbung     | Rook            | Piece               | -               |
| Vererbung     | Bishop          | Piece               | -               |
| Vererbung     | King            | Piece               | -               |
| Vererbung     | Pawn            | Piece               | -               |
| Komposition   | Account         | Player              | 1 -- 1          |
| Assoziation   | Board           | Player              | 1 -- 2          |
| Aggregation   | Board           | Field               | 1 -- 64         |
| Aggregation   | Player          | Piece               | 1 -- 0...16     |
| Assoziation   | Piece           | Field               | 1 -- 1          |
| Assoziation   | Piece           | MovementHandler      | * -- 1          |
| Komposition   | Piece           | Move                | 1 -- *          |
| Komposition   | Play            | Board               | 1 -- 1          |
| Assoziation   | Play            | GameSettings        | * -- 1          |
| Assoziation   | Play            | Account             | * -- 2          |
| Komposition   | Play            | MovementHandler      | 1 -- 1          |
| Komposition   | Play            | GameStatus          | 1 -- 1          |
| Komposition   | Play            | GameTimer           | 1 -- 1          |
