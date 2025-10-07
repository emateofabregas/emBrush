# emBrush v1.1
![grapes_010_comp_rrss_01](https://github.com/user-attachments/assets/49cff519-e9d1-404d-9289-d57386d5c71e)
A gizmo that makes a brush effect following the luminance of the same input
![emBrush_gizmo](https://github.com/user-attachments/assets/49639b82-bcc4-4b0d-a7b3-346a957c838e)
My main idea was to retain the brush while incorporating some elements from the original render. You can obtain it using a Keyer as a mask and experimenting with the maximum merge operation, primarily. This gizmo is using another gizmo from Michael Levin (https://github.com/michaellevin/kuwahara-filter-nuke).
## Features:
* Pulldown choice for switching the view: Final output, Mask Preview, and Effect Preview + Mask in the Alpha.
* Using as a Mask the Luminance of the effect or the Luminance of the image.
* You can make this effect only affect a specific region using a Mask input. 
* You can choose the merge operation you want to use with the effect. I highly recommend the *max* ones and playing the grading knobs. 
* I included the Kuwahara Filter effect in the gizmo, and you can play with it as well.
* Grading, saturation, and exposure knobs. You can adjust the effect. For example, if you use the *max* operation, you can adjust it to make it more visible by adjusting the gain or exposure.
* You can adjust the Mix of the effect; it follows the mix of the merge node that you play with the operation as well. 
![emBrush_Knobs](https://github.com/user-attachments/assets/af4e7773-9a07-489e-bdf0-b8ff0a447163)
## Updates v1.1:
* Replaced vanilla nodes with a Blinkscript code inside the saturation, exposure, and grading knobs. 
