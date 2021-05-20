# Traveller's Bingo

## Introduction

This is a fun Bingo app for travellers. It generates name of different places in the world randomly and the players can mark the places they have visited.

## Visual Preview

Home Screen: For Computers
Inline-style: 
![alt text] (https://github.com/Sanjalee22/Bingo/blob/main/sampleScreens/home.png?raw=true)

## Requirements

### User Flow

 * User loads the web page in the browser.
 * Arrives at the home screen which has the following components:
   + The app name on the top
   + An input control for the user to enter the total number of players. By default, it is one.
   + A 5 X 5 bingo ticket with names of cities in each cell and a Bingo image in center.
   + A button with the text 'Next City'.
 * When user changes the number of players, that many different tickets are shown on the screen. 
 * When user clicks on the button 'Next City'
   + A randomly picked city name is shown on the screen. 
   + If in any of the tickets, that city name is present, that cell gets highlighted.
   + A list of the cities which have been called, is displayed.
 * When user click on the highlighted cell:
   + Colour of the cell changes indicating that the corresponding city name has been called out.
   + If all the names which are vertically, horizontally or diagonally adjacent to this cell have been called out, it is a Bingo.
   + If the user is just one name call away from Bingo, that city name is highlighted in the ticket.
 * When there is a Bingo, all the cells which are part of the bingo combination, are highlighted with some animation to indicate the win.

### Validations
   
   * User can only enter numeric value greater than one in the 'Number Of Players' input box.
   * User can mark only those city name(s) in the ticket which is being called or have been called.

## Technology

* ReactJS 17.0.2
* React Hooks
* React Testing Library for Unit Tests
* Git with a commit history
* Followed standard coding guidelines

## Package Structure

The repo has following code folders:
   * public: Boilerplate code generated by create-react-app
   * src: Application specific code
      + components: react components 
      + styles: a common stylessheet and other component specific stylesheets
      + tests: component specific unit tests
      + utils: utility methods, constants, images etc.

## Running The Application:

Following are the steps to load the application in browser:
   1. Clone the repository.
   2. Open command prompt and change working directory to 'bingo' from the cloned folder.
   3. run "npm install". This will install all the dependencies needed for this application to run.
   4. run "npm start". This will open a new tab in browser. Default URL is localhost:3000.

## Future Enhancements:

1. The animations and effects, when the player is one name call away from bingo and on finally getting a bingo, can be made more appealing.
2. For smaller screens, the UI layout can be improved. 
   * Current layout: The list of cities which have been called is taking a lot of screen space. 
   * Suggested layout: It can be converted to an on-demand component or pop-up.
3. Properly handle the change in number of players during the game. 
   * Current flow: If user adds/ removes players (hence tickets) during the game, new tickets are rendered with incorrectly highlighted names.  
   * Suggested flow: User should not be allowed to add/remove players during the game.
   
   
  
      
