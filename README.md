```                                                          
                                                                                
                                     @@@@@@@@                                    
                                       #@@@@@@@                                 
                                          @@@@@@                               
      @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@                 %&&&&         
      @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@                 &@@@@         
                                           @@@@@                  &@@@@         
                                         @@@@@@                   &@@@@         
      @@@@@             @@@@@         @@@@@@@             @@@@@@@@@@@@@         
      @@@@@             @@@@@       @@@@@@@            @@@@@@@@@@@@@@@@         
      @@@@@            @@@@@        @@@@@@@@@        @@@@@@       @@@@@         
       @@@@@@         @@@@@              @@@@@@    &@@@@@         @@@@@         
         @@@@@      @@@@@@                 @@@@@@  &@@@@          @@@@@         
          @@@@@@   @@@@@                    @@@@@  &@@@@          @@@@@         
            @@@@@@@@@@@      @@           @@@@@@@   @@@@@@@       @@@@@         
             @@@@@@@@      @@@@@@@@@@@@@@@@@@@         @@@@@@@@@@@@@@@@         
               @@@@@         @@@@@@@@@@@@@@@             @@@@@@@@@@@@@@         
```

# V3D Vector Library #
This library provides a collection of utilities designed to aid in the manipulation and calculation of 3D vectors. The set of functions are useful in graphics rendering, physics simulations, and any other context where 3D vectors play a critical role.

Some useful resources to understand maths behind this library:

* https://people.eecs.ku.edu/~jrmiller/Courses/VectorGeometry/VectorOperations.html *
* https://docs.unity3d.com/2019.3/Documentation/Manual/UnderstandingVectorArithmetic.html *
* https://www.youtube.com/watch?v=cyZYHGqQ_Ug *
* https://www.youtube.com/watch?v=PYBkPBCmdwo *

### Core Functions ###
Vector Creation and Identity

- `ft_new_v3d(double x, double y, double z)`: Create a new 3D vector with specified components.
- `ft_v3d_identity(int axis)`: Return a unit vector along one of the principal axes (X, Y, Z).

### Vector Normalization ###

- `ft_normalize_v3d(t_v3d \*vec)`: Normalize a given 3D vector in-place.
- `ft_normal_v3d(t_v3d vec)`: Return a normalized version of a 3D vector.

### Vector Operations ###

- `ft_plus_v3d(t_v3d a, t_v3d b)`: Add two vectors.
- `ft_minus_v3d(t_v3d a, t_v3d b)`: Subtract one vector from another.
- `ft_dot_v3d(t_v3d a, t_v3d b)`: Calculate the dot product of two vectors.
- `ft_cross_v3d(t_v3d a, t_v3d b)`: Compute the cross product of two vectors.
- `ft_distance_v3d(t_v3d a, t_v3d b)`: Compute the distance between two vectors.
- `ft_length_v3d(t_v3d vec)`: Calculate the square length of a given vector.
- `ft_mag_v3d(t_v3d vec)`: Calculate the length (magnitude) of a given vector.

### Scalar Operations ###

- `ft_scalar_v3d(double scalar, t_v3d vec)`: Multiply a vector by a scalar.
- `ft_div_v3d(t_v3d vec, double real)`: Divide a vector by a real number.
- `ft_subs_real(t_v3d vec, double real)`: Subtract a real number from each component of a vector.
- `ft_plus_real(t_v3d vec, double real)`: Add a real number to each component of a vector.

### Utility Functions ###

- `ft_is_normal_v3d(t_v3d \*v)`: Check if a vector is normalized.
- `ft_copy_v3d(t_v3d \*vec)`: Create a copy of a 3D vector.
- `ft_perp_v3d(t_v3d vec`: Return the perpendicular vector of a given one.
- `ft_rot_v3d(t_v3d vec, int axis, double angle)`: Rotate a vector using 3D angle (Norm direction vector)
- `ft_is_idt_v3d(t_v3d vec)`: Check if a vector is an identity vector.

### Note ###

- `t_dec`: if you need more precision you can adjust t_dec definition to bigger numerical types (e.g long double, etc.)


### Usage ###

Simply include the header file and link the library to your project to start leveraging the power of this 3D Vector utility.
