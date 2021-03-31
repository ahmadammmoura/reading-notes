# Transforms

**One of the new properties in CSS3 is `transform` property.  
This new property allows for new ways to position, size, and change elements.**

**The `transform` property can either be :**

- **two dimensional**
**or**

- **three dimensional**

**Because the browser support for the `transform` property is still not great, _vendor prefixes_ are used for best support.**

**Syntax:**

```
-vendor_prefix-transform: transform_type(amount);
transform: transform_type(amount);
```

the un-prefixed declaration comes last to overwrite the prefixed versions

## 2D Transforms

**define the length and width of the element to be distorted or transformed on the xy-plane.**

- **2D Rotate**
    - to rotate an element from 0 to 360 degrees
    - +ve value : rotate cw
    - -ve value : rotate ccw

```
transform: rotate(amount);
```
- **2D Scale**
   - to change the appearant size of an element
   - the default value is 1 , which represents the element's original size

```
transform: scale(amount);
```
    
## 3D Transforms

**define the length, width, and height of the element to be distorted or transformed on the xyz-space.**


# Transitions & Animations

**Another new CSS3 properties are the `transition` and `aniamation` which allow to write the behaviors for transitions and animations without using JS.**