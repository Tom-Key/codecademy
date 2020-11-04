### CSS Transitions
- After a website is displayed, the visual appearances of various elements can change for many reasons. 
    ``` css
    a {
      transition-property: background-color;
      transition-duration: 750ms;
    }

    a:hover {
      background-color: LimeGreen;
    }
    ```
- `transition-delay: 250ms;` Delay specifies the time to wait before starting the transition. 
- `transition-timing-function`The timing function describes the pace of the transition.
    - `ease-in` — starts slow, accelerates quickly, stops abruptly
    - `ease-out` — begins abruptly, slows down, and ends slowly
    - `ease-in-out` — starts slow, gets fast in the middle, and ends slowly
    - `linear` — constant speed throughout
- **Shorthand:**`transition: color 1.5s(duration) linear 0.5s(delay);`
- **Combinations** `transition: color 1s linear,font-size 750ms ease-in 100ms;`
- **All**：`transition: all 1.5s linear 0.5s;`