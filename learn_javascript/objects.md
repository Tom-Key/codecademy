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