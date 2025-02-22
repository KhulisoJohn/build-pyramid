# Inverted Pyramid Pattern Generator

This JavaScript program generates a pyramid pattern using the `#` character. The pyramid can be inverted or normal based on the `inverted` variable. The program constructs the pattern by calculating appropriate padding and character repetition, then logs the result to the console.

## Overview

The script consists of:

- **Defining a Character (`#`) and Count (`8`)**
  - The `character` variable holds the symbol used for building the pyramid.
  - The `count` variable specifies the number of rows.

- **Padding Function (`padRow`)**
  - Calculates the correct spacing on both sides of each row to align the pyramid properly.
  - Uses `repeat` to append spaces and `#` characters dynamically.

- **Building the Rows**
  - The loop constructs rows based on the `inverted` flag.
  - If `inverted` is `true`, rows are added at the beginning (`unshift`), creating an inverted pyramid.
  - Otherwise, rows are added at the end (`push`), creating a normal pyramid.

- **Generating the Final Output**
  - The script iterates over the `rows` array and concatenates them into a single formatted string.
  - The final result is logged to the console.

## Running the Code

To execute this script, follow these steps:

1. Save the JavaScript code in a file (e.g., `pyramid.js`).
2. Open a terminal and navigate to the file's directory.
3. Run the script using:
   ```bash
   node pyramid.js
   ```
4. The pyramid pattern will be displayed in the console.

## Example Output

For `inverted = true` and `count = 8`, the console will display:

```
       #       
      ###      
     #####     
    #######    
   #########   
  ###########  
 #############
###############
```

For `inverted = false`, it prints the normal pyramid:

```
###############
 #############
  ###########  
   #########   
    #######    
     #####     
      ###      
       #       
```

## Future Improvements

### Custom Character Selection:
Allow users to specify a different character instead of `#`.

### User Input:
Implement user prompts to dynamically adjust the number of rows and inversion setting.

### Visual Enhancements:
Improve formatting with color or animation when running in a browser environment.

## Conclusion

This script provides an elegant approach to dynamically constructing symmetrical pyramid patterns. It showcases JavaScript fundamentals like loops, string manipulation, and conditional logic. Future enhancements can make it more interactive and customizable.

