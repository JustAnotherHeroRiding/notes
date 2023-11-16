# Home screen


# Theme 
- Shipyard bringing in animals
- Each block is a container
- Our task is to find the pairs of each animal
- Perhaps also a Noah's ark? Let's try the container theme

## Remove animation if it is a match
- Perhaps make the blocks flash green #DONE 
#### I have added a border, lets do more
- Make them grow and decrease, add new animation

## Flip animation
- Add a flip animation with 2 sides #DONE 
- image only gets removed after it gets unflipped #DONE 

## Back button
- Let us think how to use a back button here as the path is file path based currently and will be different on each device #DONE 
#### Currently just checking if the path ends in the folder name

## Match styling and extras

- Give feedback if it is a match #DONE 
- Mute sounds button #DONE 
- If no match make them red and close them #DONE 
- could also be removed from screen
- If it is a match end the timer quicker, else keep them open as long as before #DONE  

## Start Screen

- Quit will remove the screen #NotPossible
- Difficulties #DONE 
- Put quit on the bottom of the container with margin top auto from the difficulties #DONE 
- Header on start page #DONE 


## Background

- Background Image on start screen #DONE
- And on game screen #DONE 
- For the game I can play maybe another mix
- Mute music button #DONE 
## Difficulties
- Try to use queries for difficulties #DONE 
- Do hard difficulty #DONE 
#### generate more images
- For hard we will need more images, if the size is 6 we need 18 #DONE 
- Timer for each difficulties #DONE 
- Board accepts an object of 3 settings #DONE 
- If timer is under 1 min it should be yellow #DONE 
- If timer is under 30 it should be red #DONE 

## Block styling

- More interesting blocks #DONE 
- We can give them a background color #DONE 
- hover animation but nothing too crazy, main animation should be saved for opening #DONE 
- new images for the blocks #DONE 
- Move the width and height to the block class inside of manually setting it #DONE 

## Mobile friendliness

- Test the initial version to see where we need media queries #DONE 
- Mobile friendly
- First we need to find out what it feels like on phones and see what the biggest issues are
- avoid all side scrolling and make sure the blocks are easy to click
- Blocks should be smaller when the screen size decreases
- The header and it's contents should also shrink

## Game Over
- Move the timer into a separate class #DONE 
- New animation for game over if timer is finished #DONE 
- If game is over stop all game logic #DONE 
- Try again button on game over screen #DONE 
- turn the game over message container into a modal #DONE 
- should be closed with X and have more options to try again or quit #DONE 
- quit button with bring us back to the home page #DONE 


## Sounds
You can find free sound effects on various websites. Here are a few suggestions:

1. **Freesound:** A collaborative database of Creative Commons Licensed sounds. You can search for specific sounds like "success chime" or "error buzz".
    
2. **Zapsplat:** Offers a wide range of sound effects. You might find suitable sounds for a successful match or an unsuccessful attempt.
    
3. **Free Music Archive:** While primarily for music, they also have sound effects that could be useful.

#### Let's try recording a major lick for success, minor lick for failure
### Tasks
- play a sound when losing or winning
- Background music
- For the main menu i can play barber beats

### Ui sound settings
- make the mute music button work
- make the mute game sounds button work  #DONE 
- Add a tooltip on hover on both buttons

### Matching Sounds 
- Play a sound on block match #DONE 
- On opening one sound will play #DONE 
- If its a match play a positive sound, otherwise negative #DONE 


## in game counters
- create and style the container #DONE 
- Create a GameStats class that will be used to manage the stats and updating them #DONE 
- Create a class that will update the UI #DONE 
- Figure out the best way to use the two new classes, perhaps create an object in the board class #DONE 
- Update the UI once the stats are updated #DONE 
- turns #DONE 
- correct guesses #DONE 
- misses #DONE 
### Let's update also the percentage
- accuracy percentage #DONE 
- Encapsulate the logic behind updating the counters #DONE 
- speed drop down selector #DONE 
- cancel button to go back #DONE 

## Bug alert
- If i try to match two blocks and they are not a pair, and then quickly open one of the two blocks that i just tried to match they will have no image #DONE 


## Next steps
- Corrected the header logo home page link #DONE 
- Start game sound #DONE 
- Music is muted by default #DONE 
- start stop in animation #DONE 
- Trim the code down
- improve images 
- finish mobile friendly design #DONE 
- compress high quality assets
- tooltips for buttons #DONE 
- Send components and helper functions to third file
- show number checkbox to use numbers instead of images #DONE 
- remove the background images and replace them with a big number
- check if an image should be added in the logic
#### Think about how we can replace the backgrounds and where

- show the timer on the  right or left #DONE 
- Stats can be on the other side #DONE 
- On mobile screens keep them on bottom #DONE 








