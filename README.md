# birdcam

A collection of assets for my bird feeder camera.

![Example](capture.png)

## Hardware
* Binoculars & tripod
* Raspberry Pi 2/3/4
* [Pi Camera v2 & cable][1] 
* [Bumper case][2] 
* small screws to attach the camera board to the adapter
* Velcro strap to attach pi to the binoculars
* [Camera eypiece adapter][3] (use OpenScad to customize the size & fit):

        ```
        --- a/camera-case/RPiCam-OBJ2.scad
        +++ b/camera-case/RPiCam-OBJ2.scad
        @@ -56,11 +56,11 @@ KOyo = 1.15; // keepout edge offset
        
        ff = 0.2;  // amount to increase ID due to printer slop
        
        -MOd = 45.2+ff;  // OD of AmScope 4x microscope objective
        -MOz = 10;    // length of constant-OD part of objective barrel
        +MOd = 22.0+ff;  // OD of AmScope 4x microscope objective
        +MOz = 13;    // length of constant-OD part of objective barrel
        MOoff = 7.3;  // height offset of objective
        // MOoff = -10;  // height offset of objective
        -MOda = 45.2+ff;  // OD of 2nd barrel part
        +MOda = 22.5+ff;  // OD of 2nd barrel part
        MOza = 5.0;  // height of 2nd barrel part
        
        BHwt = 2.0;  // wall thickness of objective barrel holder

        ```

## Software
* [MotionEye][4]

## Setup
* Use the [fast network camera][5] back-end for a faster frame-rate


[1]: https://www.raspberrypi.org/products/camera-module-v2/
[2]: https://www.thingiverse.com/thing:629886
[3]: https://www.thingiverse.com/thing:1565909
[4]: https://github.com/ccrisan/motioneyeos/wiki
[5]: https://github.com/ccrisan/motioneyeos/wiki/Fast-Network-Camera
