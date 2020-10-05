## OpenCV: Open Source Computer Vision Library

### Resources

* Homepage: <http://opencv.org>
* Docs: <http://docs.opencv.org/master/>
* Q&A forum: <http://answers.opencv.org>
* Issue tracking: <https://github.com/opencv/opencv/issues>

### Contributing

Please read the [contribution guidelines](https://github.com/opencv/opencv/wiki/How_to_contribute) before starting work on a pull request.

#### Summary of the guidelines:

* One pull request per issue;
* Choose the right base branch;
* Include tests and documentation;
* Clean up "oops" commits before submitting;
* Follow the [coding style guide](https://github.com/opencv/opencv/wiki/Coding_Style_Guide).

### OpenCV rebuild

* Replace *<OPENCV_SOURCE_DIR>/modules* to *OpenCV-3.3.1/modules/*.
```
$ mv OpenCV-3.3.1/modules/ <OPENCV_SOURCE_DIR>/modules
```
* Rebuild
```
$ cd <OPENCV_SOURCE_DIR>/build && sudo make install
```

### Image capture

```
# Original capture 
$ export OPENCV_QLEN = Queue size (Queue size = 1,2,3,4)

# On-demand capture
$ export OPENCV_QLEN = 0

# Set permanently 
$ vi ~/.bashrc (add "export OPENCV_QLEN = Queue size")
$ source ~/.bashrc
```
