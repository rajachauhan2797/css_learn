CSS units are used to specify the measurement of various CSS properties such as length, width, height, margin, padding, font size, and more. There are several types of CSS units, each serving different purposes. Here's an overview of the most commonly used CSS units:

### 1. **Absolute Length Units**:
   - These units are fixed and do not change their value based on other properties or user settings.
   - Examples:
     - `px` (Pixels): Relative to the viewing device.
     - `pt` (Points): 1/72 of an inch. Primarily used for print media.
     - `in` (Inches): Inches.
     - `cm` (Centimeters): Centimeters.
     - `mm` (Millimeters): Millimeters.

### 2. **Relative Length Units**:
   - These units are relative to other property values, either of the element itself or its parent element.
   - Examples:
     - `em`: Relative to the font-size of the element. If used within a CSS property for font-size, it's relative to the parent element's font size.
     - `rem`: Relative to the font-size of the root element (`<html>`), providing a more predictable way to work with relative units.
     - `ex`: Relative to the x-height of the font.
     - `ch`: Relative to the width of the '0' (zero) character in the font.

### 3. **Percentage (%)**:
   - Percentages are relative to the parent element's property to which they are applied.
   - Examples:
     - `width: 50%;`: The element's width will be 50% of its parent element's width.

### 4. **Viewport Percentage Units**:
   - These units are relative to the viewport size (the visible area of the web page).
   - Examples:
     - `vw`: 1% of the viewport's width.
     - `vh`: 1% of the viewport's height.
     - `vmin`: 1% of the smaller dimension (width or height) of the viewport.
     - `vmax`: 1% of the larger dimension (width or height) of the viewport.

### 5. **Font Relative Units**:
   - These units are used in font-related CSS properties and are relative to the font-size of the element itself or its parent.
   - Examples:
     - `em`, `rem`, `ex`, and `ch` are also font relative units.

### 6. **Time Units**:
   - These units are used for time-related CSS properties like animations and transitions.
   - Examples:
     - `s` (Seconds): Represents seconds.
     - `ms` (Milliseconds): Represents milliseconds.

### 7. **Frequency Units**:
   - These units are used for frequency-related CSS properties.
   - Examples:
     - `Hz` (Hertz): Represents cycles per second.
     - `kHz` (Kilohertz): Represents thousands of cycles per second.

### 8. **Resolution Units**:
   - These units are used for resolution-related CSS properties, especially in print media styles.
   - Examples:
     - `dpi` (Dots per Inch): Represents dots per inch.
     - `dpcm` (Dots per Centimeter): Represents dots per centimeter.

Different units serve different purposes, and choosing the right unit for a specific context ensures a responsive and consistent layout across various devices and screen sizes.