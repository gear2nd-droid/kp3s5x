# BC axis adjustment

## Platform adjustment
Align the plane of the platform and bearing.
1. Place a ruler on the front and back ribs of the B-axis carriage with the edges facing each other.
2. Align the edge of the ruler with the height of the platform.
3. Place the nozzle on the platform, and with the nozzle fixed, adjust the distance between the nozzle and the platform while rotating the C-axis manually.
4. Again, apply the ruler and adjust it so that the edge of the platform and the edge of the ruler are in contact.

## A-axis rotational deflection compensation
The weight of the B-axis motor causes the platform to deflect in the A-axis direction and tilt. This is the correction.
1. Measure the distance between the nozzle and the platform when the nozzle is operated with X=0, Y=Change, Z=Fixed.
2. Adjust "offset_a" in the [printer] section to keep the spacing constant.

# XYZ axis adjustment
The intersection of the rotation axes of the B and C axes must be the XYZ origin.

## Z home position adjustment
1. Adjust the "position_endstop" in the [stepper_z] section so that z=0 on the platform.
2. Deflection compensation results in a larger change than the change in "position_endstop". Please pay attention to this.

## X/Y home position adjustment
1. While dispensing, rotate the C-axis and adjust it so that it becomes a single point instead of a circle.
2. Adjust "position_endstop" in [stepper_x] and [stepper_y] for adjustment parameters.
