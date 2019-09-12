# Monopoly

The Mathematics of Monopoly: how likely are you to land on a square? 

This project is inspired by standupmaths' [The Mathematics of Winning Monopoly](https://www.youtube.com/watch?v=ubQXz5RBBtU "Youtube video"). 


[Monopoly](https://monopoly.fandom.com/ "Monopoly Wiki") is a board game of chance in which players go around a board to buy and develop properties and pay rents. However, not all of the squares have equal probability of being landed on because of two main factors: 

Chance and Community Chest cards include a mechanism of sending the player to another square or to jail
Jail: A player goes to jail by rolling three doubles in a row, getting sent there from Chance or Community Chest card, or landing on the Go To Jail square. 

I calculated the probabilities of landing on every square by simulating 500000 games of 100 turns each in this Jupyter notebook. 

### Main Conclusions
1. Squares do not have the same probability of being landed on. 
2. The squares most likely to be landed on are in descending order: 
  * Jail
  * The orange squares (Tennessee Avenue, New York Avenue, St. James Place)
  * The red squares (Illinois Avenue, Kentucky Avenue, Indiana Avenue)
  * The yellow squares (Atlantic Avenue, Ventnor Avenue, Marvin Gardens)

### Figures and Tables

#### Figure 1
Figure 1 below shows the relative probabilities of moving from one square to another. 
<img src=https://github.com/ayoola-babatunde/monopoly/blob/master/monopoly%20screenshot1.png alt="Figure 1" width="1000"/>
As expected, the most likely squares from a given square are those 6, 7, and 8 squares away since these are the numbers that come up the most when rolling two dice (44% of the time). 
We also note that properties 6, 7, and 8 squares away from jail (square 40) have high visit rates since a player ends in jail a lot. .
Other important squares are destinations from chance and community card squares. 
Note the blank row/column 30 (Go To Jail square). This is because no one ends the turn on this square. 

#### Table 1
Table 1 below shows the simulated probabilities of landing on every square

| index | names                  | percentage |
|-------|------------------------|------------|
| 0     | Go                     | 2.885436   |
| 1     | Mediterranean Avenue   | 2.003141   |
| 2     | Community chest        | 1.918602   |
| 3     | Baltic Avenue          | 2.082590   |
| 4     | Income tax             | 2.272565   |
| 5     | Reading railroad       | 2.753477   |
| 6     | Oriental Avenue        | 2.248173   |
| 7     | Chance                 | 2.168054   |
| 8     | Vermont Avenue         | 2.305446   |
| 9     | Connecticut Avenue     | 2.269254   |
| 10    | Jail                   | 2.224882   |
| 11    | St. Charles Place      | 2.629665   |
| 12    | Electric company       | 2.663134   |
| 13    | States Avenue          | 2.251561   |
| 14    | Virginia Avenue        | 2.479692   |
| 15    | Pennysylvania Railroad | 2.609909   |
| 16    | St. James Place        | 2.744481   |
| 17    | Community chest        | 2.572099   |
| 18    | Tennessee Avenue       | 2.869067   |
| 19    | New York Avenue        | 2.867210   |
| 20    | Free parking           | 2.846641   |
| 21    | Kentucky Avenue        | 2.655180   |
| 22    | Chance                 | 2.630511   |
| 23    | Indiana Avenue         | 2.596563   |
| 24    | Illinois Avenue        | 3.023932   |
| 25    | B & O Railroad         | 2.742805   |
| 26    | Atlantic Avenue        | 2.578784   |
| 27    | Ventnor Avenue         | 2.560849   |
| 28    | Water works            | 2.686024   |
| 29    | Marvin Gardens         | 2.480863   |
| 30    | Go to Jail             | 0.000000   |
| 31    | Pacific Avenue         | 2.537292   |
| 32    | North Carolina Avenue  | 2.473935   |
| 33    | Community chest        | 2.389051   |
| 34    | Pennsylvania Avenue    | 2.348941   |
| 35    | Short line             | 2.283079   |
| 36    | Chance                 | 2.034814   |
| 37    | Luxury tax             | 2.050690   |
| 38    | Park Place             | 2.052077   |
| 39    | Boardwalk              | 2.471845   |
| 40    | Actual Jail            | 3.737686   |


### Future Plans

I would like to simulate more games and introduce money, multiple players, and bankruptcy. Feedback greatly appreciated. 
