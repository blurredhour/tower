Tags: [[learning]] [[maths]] [[programming]]

Written on 2025-10-22

Status as of 2025-10-22:
### TEMPORARILY        SUSPENDED.

These documentations are based on the file *learn.py* on the *crymson@Atreidies* system placed in *~/note/python/grid*
The tools used for this experiment are as follows:

1. The [[Atreidies Computer System]]
2. The [[pygame graphics library]]
3. The [[Python Programming Language]]

The goal of this experiment was to draw a grid using the [[pygame graphics library]] to be used for other projects. The initial goal of this experiment has been fulfilled but the goal was further expanded to rendering vector fields. The rendering of the vectors have also been completed but lack customizability. The issues will be further expanded upon in the vectors section. The current goal is to be able to make customizable vector fields.

There are 5 main components namely:

1. constants and parameters
2. draw_grid()
3. draw_vectors()
4. render()
5. Main loop

## constants and parameters 

This component is used to create all the required constants and parameters in order to easily be able to modify the inputs going into the functions.

## draw_grid()

This function handles the drawing of a simple grid using the **pygame.draw.line()** function. It takes in four inputs namely:
1. **lnum**
2. **pos**
3. **surface**
4. **colour**

**lnum** is the counter used the satisfy the while loop. The function uses only a sigle while loop causing the resulting grid to be a square grid which is cut off by the window. This might lead to inefficiencies later on so this has to be checked.

## draw_vectors()

This is the largest function in the file and the purpose is to be able to draw vectors on all of the points of intersection of the grid. Currently they all track towards the mouse and change their length according to their distance from the mouse. The function takes in 6 inputs being:

1. **surface**
2. **colour**
3. **start_pos**
4. **end_pos**
5. **x_counter**
6. **y_counter**

the function uses 2 nested while loops to draw the vectors with the variables to satisfy the while loops being **x_counter** and **y_counter**. This function does not get cut off by the screen and maps efficiently to only the intersections visible.

There is also some proto functionality for changing colours based on length of the vector which has to be expanded upon.

There are various problems which have to be addressed. The tracking of the vectors to the mouse creates a strange optical illusion using the negative space. I suspect this is due to the linear nature of the lengths of the vectors. Maybe this can be addressed using a [[Gaussian Distribution]] to smooth out the vectors. This optical illusion is much more prevalent when mapping the length of the vectors to their brightness it creates a pattern that shouldn't be present.

Other matters include not being able to easily change the orientation of the vectors. If this is resolved it may lead to the creation of vector fields.

## render()

the render function is used to simplify the main loop so as not to introduce clutter. it only calls on the aforementioned functions and is the only function present in the main loop

## main loop

The main loop calls on the **render()** function and handles the functionality to close the running application.

