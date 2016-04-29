program-sketch-tool
===================

The program-sketch tool is a set of programming tools build on top of Dracket.

### Install

You can install this module quickly using the Package Manager, to this end proceed to the following steps:

* **Note:** make sure you've installed the [image-data-snip](https://github.com/gui-/program-sketch-tool) class.
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

#### Scketch utilization
* To use the sketches in the program, the funtions must have the following structure:

```racket
(define (foo bar baz)
  ;image here
  ;funtion body here
  )
```
* The images can be inserted in the menu `Insert > Insert Image ...`
* When the image is inserted all arrows will point to the image center

![image](https://cloud.githubusercontent.com/assets/3803770/14906201/986dfac2-0db0-11e6-9152-0554751fd86a.png) 

* To change an arrow target press <kbd>ctrl</kbd> + right click on the desired target symbol 

![image](https://cloud.githubusercontent.com/assets/3803770/14906124/058ade8c-0db0-11e6-8ccf-ec7f2502c856.png)

* In the UI, write the name of the argument you want to correct, in this case was alpha. **Note** the name argument name written in the UI must be exactally the same to the one written in the function.

* The field x and y of the UI are optional, it defines the place where the arrow starts. That means, if you choose 0,0 an arrow will apper in the upper left coner of your image (but becareful it only accepts number in [0,1])

* Finally, click on Check Syntax button and check if the arrow is correct.

![image](https://cloud.githubusercontent.com/assets/3803770/14906152/4bc0760a-0db0-11e6-8706-3aa92c1de6ff.png)

### Auto run

* Clicking in the button ![alt text](https://cloud.githubusercontent.com/assets/3803770/14906340/4b22a2c0-0db2-11e6-8ac6-9348f694a45b.png) the editor will be constantly running the program.
* If you are editing your program we recommend to disable this feature, it can be annoying. However if you want to "play" with it, wirte a function invocation, e.g. as the following, and try to change these input values.

```racket
(arrow (xyz 0 0 0) 1 (/ pi 3) (/ pi 2) 1)
```

* to turn it off just click on the Auto Run button again.
* Another way to test program inouts is by sliders. So you can 

| Shortcut         | Action                         | Resource  |
| ---------------  |:------------------------------:| ---------:|
| <kbd>ctrl</kbd> + right click   |   | image |
| <kbd>shift</kbd> + right click  | centered      |   image |
| <kbd>shift</kbd> + left click   |        | image |
| select a number + <kbd>F4</kbd> | | number|

### Final Notes

This software is a proof of concept, any issue related with it please open a github issue or contact me.

Thank you.


