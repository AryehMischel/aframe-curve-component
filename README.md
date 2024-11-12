# aframe-curve-component ?(v0.1.3)

> **Note**: I am **NOT** the original author of this component. This repository includes a working version of the component based on the original work by [protyze](https://github.com/protyze) and [AdaRoseCannon](https://github.com/AdaRoseCannon).

For more details, check the original [npmjs page](https://www.npmjs.com/package/aframe-curve-component/v/0.1.3).

## Changes & Updates

The component needed a few modifications to be compatible with A-Frame 1.6.0. 
<br/> The changes are as follows...

1. **Fix for `getworldposition-target-is-now-required-error-message`**:
   - I added an empty `Vector3` to the `getWorldPosition` call to resolve the issue.
   - The fix involved adding the following line:  
     ```javascript
     point.object3D.getWorldPosition(position);
     ```

2. **Updated Rotation and Scale Syntax for `clone-along-curve`**:
   - In the original implementation, `vec3` properties were declared as strings (e.g., `'0 0 0'`).
   - In this update, the proper format for `vec3` properties is now the object syntax:  
     ```javascript
     { x: 1, y: 1, z: 1 }
     ```
   - This change ensures compatibility with the latest A-Frame versions.

## Credits

- **Original Author**: [protyze](https://github.com/protyze)
- **Based On**: [AdaRoseCannon's aframe-curvez component](https://github.com/AdaRoseCannon/aframe-curves)
  
### Important Notes

- The repository for the original component seems to have been deleted or set to private. All that remains here is a working version of the component as a plain JavaScript file.
- This repository only includes the modified component. Please refer to the original [A-Frame Curve Component](https://github.com/AdaRoseCannon/aframe-curves) for more context on how the component was initially designed.

## Installation

Currently the component only exists as a plane javascript file in the repo. I am not sure how to go about updating the npm package, but if anyone wants to take it and host it somewhere I'm sure it would be appreaciated!

