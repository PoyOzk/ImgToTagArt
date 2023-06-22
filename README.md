# ImgToTagArt
Originally made this in a day to be able to place images using no quotes at all, which still works, but the result is too long to be useful for much, so I just decided to post it.

This gets an image using the upload file button, (and also a resolution slider to lower result text) and once the user clicks the "Process Image" button, does a few things:

- For each row of pixels, an <acornym> tag is made.
    - Realistically any tag could be used here but <acornym> is very rarely used and it could mess up the :nth-child selector if placed on already existing code.
    - Every <acornym> tag has css applied to it using an nth-child() selector, which is in <style> tags.
         - each acornym is set to the height of one pixel, the width of the inputted image, and given a gradient that starts and stops exactly where the next color does to completely remove the actual gradient effect and effectively load in pixels.
  
Once all of that is done, it returns the result to the user in a text box. 
  
Keep in mind the end result text can be extremely long, so this will probably cause lag, but very interesting to mess around with this nonetheless.
  
Feel free to use any code in this project for your own, provided that proper credit is given.
