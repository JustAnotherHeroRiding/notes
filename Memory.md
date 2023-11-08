

## Block class
Only one method for getting and setting #DONE 
Delete method for the image in the block class #DONE 

## Board Class
Move timeout image into another function in the board class #DONE 

## If blocks match
- Remove the blocks if they match #DONE 

#### Making them stay open
make logic if two blocks are the same, remain open #DONE 
disable click listener on the two blocks #DONE 

## CSS
further improvements css
flip animation for blocks #DONE 

## Images folder parse

read images from images folder and put into array #Impossible
Create a new file and import the array from it #DONE 

## My changes
- Shuffle the images #DONE 
- Add a win condition #DONE 
- Add a timer that will mean that the user lost
- The gameOver function should display an animation upon winning #DONE 
- And display a message #DONE 
- When there is a match add a sound and animation

## Element creation
- Move creation logic of elements into another class called elementCreator class #DONE 
- Create div using the class instead of manually #DONE 
- Create the images using the class #DONE 
- Add support for multiple styles and classes when creating elements
## Cleanup 

remove console.logs



# ONLY ONE EMPTY LINE BETWEEN

## Check click on 2 blocks
- Currently when two blocks are clicked nothing will happen until a third click is made which will clear the opened blocks array  #DONE 
- What should happen is that a function should be called if the two blocks match, and if they do they should remain open #DONE 
- If the same block is clicked twice, it should not call any function, we can perhaps use a set here #DONE 
- There should a timeout function again while the blocks are being compared #DONE 
- We can again check the image and see if it is the same #DONE 
- Use the flip class again for the animation #DONE 

### This might be a little weird as the callback function needs access to the block element again
- Define the callback in the constructor, perhaps in the board itself so it does not have to be defined for each block separately

#### Where should the check match function be?
`openBlock` inside of board already checks the counter for number of opened blocks
I put it inside of the Board class as here we have the array of opened blocks that we can check

## Shuffle blocks
- Use the same function it should work as the new block object array is similar to the previous one #DONE 
##### This worked by simply using the shuffle function when creating the array


## Win condition
- Create a win condition to trigger the game over screen and animation #DONE 
- Previously i used the number of blocks remaining unopened, but there must be another way as the condition was triggered too early sometimes #DONE 

## Improve animation - abstract or new confetti animation
- Perhaps we can create a base Animation class, and the extend with the confetti class for confetti, and then be able to add a start game animation #DONE 
- when creating the confetti elements, there is a lot of code for the element being created that could be done by passing params to the element creator

## Opening a third block bug
- Currently if i have 2 blocks open, while the timeout is still not over if i click on a third block it will bug out and the correctly matched pair will close as if it does not match
##### For now i have added a property to track if the timer is running or not. If it is running under no case should any code run


## Learn how bind works and binding this(the context)
- In two places, angel used .bind(this) on a function so that we can use the context in the function itself
- Otherwise this would refer to the function being called, but we need a way to access the object where the function is called
- Here we pass the reference to the board object down to the block
- See how the binding was used in the block class

## Callback function in openBlock
- There was some magic used here as we needed a way to access the board object from inside the blocks


## Create element creator
- There is already an element creator but it needs to be improved
- Right now it creates the element and returns a reference but we add styles and properties


#### Flipping images animation code

```
const animationEndCallback = () => {
div.appendChild(img);
div.classList.remove("flip");
div.removeEventListener("animationend", animationEndCallback);
};
div.classList.add("flip");
div.addEventListener("animationend", animationEndCallback);
```


#### Start animation code
```
const gameoverMessage = document.querySelector("h2") as HTMLHeadingElement;
const confettiAnimation = new ConfettiAnimation(gameoverMessage);

confettiAnimation.start();
setTimeout(() => confettiAnimation.stop(), 5000);

```