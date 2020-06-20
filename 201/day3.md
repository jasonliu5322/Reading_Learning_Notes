# Day 3
- Chapter 3: "List" p62-73
    - Ordered lists
    ```
    <ol>
    ```

    - Unordered lists
    ```
    <ul>
    ```

    - Definition lists
    - Nested lists

- Chapter 13: "Boxes" p300-329
    - Box dimensions: width, height
    - Limiting width: min-width, max-width
        - Some page designs expand and shrink to fit the size of the user's screen. In such designs, the min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide.
    - Limiting height: min-height, max-height
    - Overflowing content: hidden, scroll

    - Border, Margin, Padding p307
        - border-width
        - border-style
        - border-color
        - shorthand: border

        - padding: The padding property allows you to specify how much space should appear between the content of an element and its border.
        
        - margin: The margin property controls the gap between boxes. Its value is commonly given in pixels, If one box sits on top of another, margins are collapsed , which means the larger of the two margins will be used and the smaller will be disregarded.
        

     - centering content
       In order to center a box on the page, you need to set a width for the box (otherwise it will take up the full width of the page). Once you have specified the width of the box, setting the left and right margins to auto will make the browser put an equal gap on each side of the box. 

     - change inline/block
       display: inline/block/inlin-block/none p317
       If you use this property, it is important to note that inline boxes are not supposed to create block-level elements.

     - hiding boxes
       The visibility property allows you to hide boxes from users but It leaves a space where the element would have been.
       visibility: hidden/visible

     - border imgages CSS3 p319
       The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces.

     - box shadows CSS3

     - rounded corners CSS3
       CSS3 introduces the ability to create rounded corners on any box, using a property called border-radius. The value indicates the size of the radius in pixels.

     - elliptical shapes

- Javascript Chapter 4: 
   “Decisions and Loops” from switch statements on (pp.162-182)

   -  TYPE COERCION & WEAK TYPING
       avaScript can convert data types behind the scenes to complete an operation. This is known as type coercion. For example, a string ' l ' could be converted to a number 1 in the following expression:(' 1' > 0). As a result, the above expression would evaluate to true.

        JavaScript is said to use weak typing because the data type for a value can change. Some other languages require that you specify what data type
        each variable will be. They are said to use strong typing.

        Type coercion can lead to unexpected values in your
        code (and also cause errors). Therefore, when checking if two values are equal, it is considered better to use strict equals operators ===and ! ==
        rather than == and != as these strict operators check that the value and data types match.

   - Loop
      - for loop
      - while loop
      - do-while loop
      