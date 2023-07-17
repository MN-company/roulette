![Brand Image](brand-image-no-no.png)

# Automated Roulette System (ARS) 🎰

The ARS project is a Google Sheets file that provides a simulation of a live casino, allowing players to place bets on a physical roulette wheel. The file uses formulas and a script to calculate players' bets, potential winnings and remaining balance. The goal of the project is to create an interactive and realistic gaming experience through the spreadsheet, allowing players to experience the thrill of gambling without having to physically travel to a casino. By using Google Sheets as the platform, the file can be easily shared with other players, allowing for virtual competition or just having fun with friends.

## Installation

1. Go to the  and make a copy of the file.
To use ARS, follow the steps below:

Click on the [ARS spreadsheet link](https://docs.google.com/spreadsheets/d/14G8uvZQG2EfwmBMk9HPM--t2D0ymGmPYAxfy_NaDtZI/edit#gid=255657849) to access the spreadsheet.
Once the sheet is open, make a copy of the file by selecting 'File' from the menu bar and selecting 'Make a copy'.
When the spreadsheet opens, you will be asked for the dealer's email address. Enter the desired email address. (If you wish to disable this option, see the wiki for further instructions).
You will see a new menu appear. Select 'Spin' from the menu and sign in to your Google Account when prompted.
The dealer will now be able to run the script directly from the menu.
What if the menu does not generate?
Sometimes Google requires authentication in order to generate the menu. If the authorisation pop-up does not appear, follow these alternative steps:

Open the 'Extensions' menu.
Select 'Apps Script'.
Run the 'onOpen' function.

## How to use

Here are the steps to follow once you have authenticated yourself and set up your merchant email:

From the "ARS" menu at the top, select "Settings".
The settings menu allows you to set the deposit amounts for each player. Enter the desired deposit amount for each player and save the settings.
Once the deposits have been set, the players can begin to place their bets. They can enter their bet amounts in the designated cells or areas.
When all players have placed their bets and are ready to proceed, the dealer should select "Spin" from the "ARS" menu.
The script will then perform the necessary calculations using a simplified B-B+R (Balance, Bet, Return) formula.
B (Balance): The script will deduct the bet amount from each player's balance.
B+ (Bet+): The script will calculate the potential winnings based on the bet amount and the roulette outcome.
R (Return): The script will update each player's balance by adding any winnings to their balance.

# Little explenation 

## Dealer sheet

### Roulette table
![Roulette table](roulette_1.png)

The Dealer will be looking at the Roulette numbers to see where the winning number is located. The cells corresponding to its characteristics will turn green and "TRUE" will be written if the number is valid.

### History and winning number
![History of extracted numbers](history_1.png) 

The dealer should enter the number that came out of the roulette wheel in the "Winning Number" column and enter it in the history of previous numbers.

### Information about players
![players info](tabs_1.png)

The Dealer will keep an eye on the default values in the upper table, which must be changed according to his needs. The table below shows values such as the bet, balance and winnings for each player. These should not be changed as they are handled by formulas and scripts that work independently.

## Player sheet

### Bet, return and balance
![Bet, return and balance](RBB.png)

These cells delegate the calculation of bet, win/loss and balance to formulas.

### Simple betting 
![outside bet](regularplayer.png)

In all grey cells the player must enter the amount of money to be allocated to this bet.

### Other type of betting
![Other bet](otherbet.png)

As before, the player must enter the amount of money to bet in the grey cells and the correct number to bet on in the blue cells. 

## Licence

ARS is released under the terms of the GNU licence.

## Project Status

ARS is currently in beta stage and can be used without any problems. Some values in the script can be changed to customise player names, but this also involves changing references. See FAQ.

## Future goals --> THIS SECTION IS MOVED INTO THE GITHUB PROJECTS

# FAQ --> THIS SECTION IS MOVED INTO THE WIKI

# Contacts
If you want collaborate or you have any question you can open an issue

