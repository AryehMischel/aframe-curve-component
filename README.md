All the information on this component can be found here [npmjs page](https://www.npmjs.com/package/aframe-curve-component/v/0.1.3)
 <br /> I AM NOT THE ORIGINAL AUTHOR.  
 ➡️ [protyze](https://github.com/protyze) is the Original Author and his component is based on [Ada's](https://github.com/AdaRoseCannon) aframe-curvez [component](https://github.com/AdaRoseCannon/aframe-curves). <br />
I am not sure why the repository for the original component has been deleted/privated.  <br />All there is on this repo is a working version of the component as a plane javascript file.
I changed only two things.
1) to fix the "getworldposition-target-is-now-required-error-message" I passed an empty vector 3 to point.object3D.getWorldPosition(position);
2) I had to update the Rotation and Scale Properties of the 'clone-along-curve' component. Previously, in A-Frame you declared a 'vec3' properties in the following format "'0 0 0'", but now you would format a 'vec3' property like this  "{ x: 1, y: 1, z: 1 }".
