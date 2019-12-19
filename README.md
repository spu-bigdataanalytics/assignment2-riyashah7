# ASSIGNMENT 2
The goal is to achieve concurrent programming using Python. This project shows you the two ways of parallelising tasks, in which you have to improve the speed of the serial-programming application by using threading and/ or multiprocessing.


There are many options for multithreading and multiprocessing.

Some of these packages are, but not limited to:

Ray

Numba

Modin

Dask

multiprocessing

threading

concurrent.futures


In my project I used threading for multi-threading the task of downloading images and used multi-processing for the resizing images task. 

In Multi-Threading the task of image downloads, I created two threads: t1 and t2, we can use more and try which one gives the best results. For me, 2 threads perfomed the task in least amount of time. We can also, automate the number of threads where python will select the best number of threads and perform the task, but for learning purposes, I wanted to check the timings for each change in the number of threads, hence using the tradiotional way. 

For Multi-processing the task of resizing the images, I used pool method in the multiprocessing library. Pool distributes the tasks to availabe processors in FIFO scheduling. The starmap function maps the function to its arguments. This is used when we have multiple inputs for the function, for a single input function we can use pool.map.

To display the results, I used python's prettytable library. This gives a nice tabular representation of the content. It is easy to use this library and we get many in-built functions, which makes it time-effecient.

