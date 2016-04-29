program-sketch-tool
===================

The program-sketch tool is a set of programming tools build on top of Dracket.

### Install

You can install this module quickly using the Package Manager, to this end proceed to the following steps:

* **Note:** make sure you've installed the [image-data-snip](https://github.com/gui-/image-data-snip) class.
* open DrRacket
* then, go to `File > Package Manager...`
* in the field `Package Source` paste the following link

> https://github.com/gui-/program-sketch-tool.git

* finally click on `Install`
* Done!
![image](https://cloud.githubusercontent.com/assets/3803770/14905653/93d5728e-0daa-11e6-983b-4bcc4554c830.png)

### Uninstall

* In the Package Manager go to the Currently Installed tab  
* Find the name program-sketch-tool
* Click on Remove
* Done!

### Utilization

After the installation it is **important** to restart DrRacket, in order to load all plugins.

#### Sketch utilization
* To use the sketches in the program, you must have the following structure:

```racket
#lang racket
(require image-data-snip)

(define (my-function foo bar baz)
  ;image here that illustrates foo,bar, and baz
  ;function body here
  )
```
* The images can be inserted in the menu `Insert > Insert Image ...`
* When the image is inserted all arrows will point to the image center

![image](https://cloud.githubusercontent.com/assets/3803770/14906201/986dfac2-0db0-11e6-9152-0554751fd86a.png) 

* To change an arrow target press <kbd>ctrl</kbd> + right click and point to the desired location where you want the arrow to point. Note: it must be inside the image space. 

![image](https://cloud.githubusercontent.com/assets/3803770/14906124/058ade8c-0db0-11e6-8ccf-ec7f2502c856.png)

* In the UI, write the name of the argument you want to point out, in this case was alpha. **Note** the argument name written in the UI must be exactly the same of to the one written in the function.

* The field x and y of the UI are optional, it defines the place where the arrow starts. That means, if you choose 0,0 an arrow will appear in the upper left corner of your image (but be careful it only accepts number in [0,1])

* Finally, click on Check Syntax button and check if the arrow is correct.

![image](https://cloud.githubusercontent.com/assets/3803770/14906152/4bc0760a-0db0-11e6-8706-3aa92c1de6ff.png)

### Auto run

* Clicking in the button ![alt text](https://cloud.githubusercontent.com/assets/3803770/14906340/4b22a2c0-0db2-11e6-8ac6-9348f694a45b.png) the editor will be constantly running the program.
* If you are editing your program we recommend to disable this feature, it can be annoying sometimes. However, if you want to "play" with it, wirte a function invocation, e.g. as the following, and try to change these input values.

```racket
(arrow (xyz 0 0 0) 1 (/ pi 3) (/ pi 2) 1)
```

* to turn it off, just click on the Auto Run button again.

* Use sliders to change the program inputs interactively.

* Select a number, click and drag the cursor until the number is entirely selected 

![image](https://cloud.githubusercontent.com/assets/3803770/14906704/615a2c8a-0db6-11e6-9438-2a079ab145f0.png)

* Press <kbd>F4</kbd>, then the slider will appear (note make sure that the DrRacket window is maximized, otherwise the slider may appear outside the window)

![image](https://cloud.githubusercontent.com/assets/3803770/14906849/3e37d6b0-0db8-11e6-8543-e25b461aa9e8.png)

* To close the slider just click on the main editor window and it will close automatically.

### Shortcut Summary

| Shortcut                        | Action                         | Resource  |
| ------------------------------  |:------------------------------:| ---------:|
| <kbd>ctrl</kbd> + right click   | sets arrow                     | image     |
| <kbd>shift</kbd> + right click  | dismiss view                   | image     |
| <kbd>shift</kbd> + left click   | show  view                     | image     |
| select a number + <kbd>F4</kbd> | show slider                    | number literal|

### Final Notes

This software is a proof of concept, any issue related with it please open a github issue or contact me.

Thank you.
