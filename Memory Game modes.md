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
### Tasks
- play a sound when losing or winning
- Background music
- For the main menu i can play barber beats
- make the mute music button work
- make the mute game sounds button work 
- Play a sound on block match
- On opening one sound will play
- If its a match play a positive sound, otherwise negative


## in game counters
- create and style the container #DONE 
- turns
- correct guesses
- misses
- accuracy percentage
- speed drop down selector
- show number checkbox to use numbers instead of images
- cancel button to go back #DONE 

## Slim down
- Start with optimizing the code in start.ts
- Slim down as much as possible in main.ts afterwards
- Refactor the css as I am sure there is a lot of repetition now








