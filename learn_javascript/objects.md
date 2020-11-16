### Objects
![](https://content.codecademy.com/courses/learn-javascript-objects/objectliteraldiagram.svg)
- Accessing Properties
    - dot notation `.`
    ![](https://content.codecademy.com/courses/learn-javascript-objects/object%20dot%20notation.svg)
    
    - Bracket Notation 
    ![](https://content.codecademy.com/courses/learn-javascript-objects/object%20access%20bracket.svg)
       - We must use bracket notation when accessing keys that have numbers, spaces, or special characters in them
       - With bracket notation you can also use a variable inside the brackets to select the keys of an object. This can be especially helpful when working with functions:
        ``` js
        /* If we tried to write our returnAnyProp() function with dot notation (objectName.propName) the computer would look for a key of 'propName' on our object and not the value of the propName parameter.*/
        let returnAnyProp = (objectName, propName) => objectName[propName]; 
        returnAnyProp(spaceship, 'homePlanet'); // Returns 'Earth'
        ```
- Property Asssignment
![](https://content.codecademy.com/courses/learn-javascript-objects/object%20update%20property.svg)
    - If there was no property with that name, a new property will be added to the object.
    - You can delete a property from an object with the `delete` operator.`delete spaceship.mission; `
- Methods , what an object does.
    - Object methods are invoked by appending the object’s name with the dot operator followed by the method name and parentheses:
    ``` js 
    const alienShip = {
      invade () { 
        console.log('Hello! We have come to dominate your planet. Instead of Earth, it shall be called New Xaculon.')
      }
    };
    ```
- Nested Objects
- Pass By **Reference**
    - Functions which change object properties actually mutate the object permanently
    
- Looping Through Objects
    ``` js
    for (let crewMember in spaceship.crew) {
      console.log(`${crewMember}: ${spaceship.crew[crewMember].name}`);
    }
    ```

### Advanced Objects
- The this Keyword
    - *(self in python objects)*
    - Inside the scope of the .diet() method, we don’t automatically have access to other properties of the goat object.
    - avoid using arrow functions when using this in a method!
- Privacy
    - One common convention is to place an underscore `_` before the name of a property to mean that the property should not be altered.
    - In the example above, the _amount is not intended to be directly manipulated.Even so, it is still possible to reassign _amount:
- **Getters** are methods that get and return the internal properties of an object.
- **setter** methods which reassign values of existing properties within an object.
    ```js
    const robot = {
      _model: '1E78V2',
      _energyLevel: 100,
      _numOfSensors: 15,
      get numOfSensors(){
        if(typeof this._numOfSensors === 'number'){
          return this._numOfSensors;
        } else {
          return 'Sensors are currently down.'
        }
      },
      set numOfSensors (num) {
        if(typeof num === 'number' && num >=0){
          this._numOfSensors = num;
        } else {
          console.log( 'Pass in a number that is greater than or equal to 0');
        }
      },

    };
    ```
---
- Factory Functions
    ``` js
    const monsterFactory = (name, age, energySource, catchPhrase) => {
      return { 
        name: name,
        age: age, 
        energySource: energySource,
        scare() {
          console.log(catchPhrase);
        } 
      }
    };
    const ghost = monsterFactory('Ghouly', 251, 'ectoplasm', 'BOO!');
    ghost.scare(); // 'BOO!'
    ```
- Property Value Shorthand
    ```js
    const monsterFactory = (name, age) => {
      return { 
        name: name,
        age: age
      }
    };
    /* The example below works exactly like the example above */
    const monsterFactory = (name, age) => {
      return { 
        name,
        age 
      }
    };
    ```
- Destructured Assignment
    ```js
    const vampire = {
      name: 'Dracula',
      residence: 'Transylvania',
      preferences: {
        day: 'stay inside',
        night: 'satisfy appetite'
      }
    };
    const { residence } = vampire; // 'Transylvania'
    const { day } = vampire.preferences;  // 'stay inside'

    console.log(typeof residence) // object
    ```
     
- Built-in Object Methods
    ``` js
    // grab the property names, otherwise known as keys, 
    const robotKeys = Object.keys(robot);
    // array will contain more arrays that have both the key and value of the properties 
    const robotEntries = Object.entries(robot)
    // want another object that has the properties of robot but with a few additional properties.
    const newRobot = Object.assign({laserBlaster: true, voiceRecognition: true}, robot);
    ```
    - [MDN’s object instance documentation.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object#Methods)