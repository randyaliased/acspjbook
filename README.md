(intro)=
### An interactive playground for audio analysis, processing, and synthesis

<!-- _This is the first page the student will see when opening the url._ -->

Welcome to this book on audio analysis, processing, and synthesis. Over the past few years of teaching audio digital signal processing (audio DSP) concepts, I've found that students being exposed to the material for the first time have a difficult time developing intuition for what may sometimes feel like very abstract concepts. Particularly, those with a weaker mathematical background have a hard time connecting with the equations and static depictions of formulae. I have been [experimenting](https://pubs.aip.org/asa/jasa/article/153/3_supplement/A214/2885917/Interactive-demonstrations-in-acoustic-signal) in the classroom more and more with [Jupyter notebooks](https://github.com/randyaliased/acs-sp-demos), where I make use of animations, interactive plots and demonstrations, and real-time manipulation of sounds to create a more accessible and "tangible" connection to audio DSP. The main idea is that with short snippets of code, you get to take control of an equation or concept by dissecting it such that you can modify signals/parameters to produce immediate sonic and visual outputs. In my opinion, this transforms our learning of audio DSP into a creative and enjoyable process. For instance, one thing I personally like to do is modify things until I "break" something, i.e., testing the limits of equations and concepts and understanding under what conditions reasonable outputs are produced. 

One challenge I've had with the Jupyter notebooks though is that they have not always been straightforward to share, especially for those who are not familiar with Python or the concept of [virtual environments](https://docs.python.org/3/library/venv.html). On top of that, things would sometimes only work on specific versions of Python and admittedly I've not been very great with keeping track of this. This is where the brilliance of [Teachbooks](https://teachbooks.io) comes in! With teachbooks, we can now make a Jupyter book (a collection of Jupyter notebooks) where we can directly run and modify Python snippets online without the need to worry about specific Python versions. There are a few tricks to get this all to work, particularly for audio, but that's my headache! 

This approach to learning audio DSP is what I'm calling "Tangible audio analysis, processing, and synthesis", where we more physically interact with equations to create deeper connections, understanding, and intuition of mathematical concepts in this field. This book is, however, not meant to be comprehensive in terms of going into all of the fine details of audio DSP (for this, we have classic texts such as {cite:p}`Oppenheim2009` {cite:p}`zolzer2011dafx`), but rather to be treated as a complementary companion to audio DSP studies. I'm certain there are many more topics to be included, but I've started with a focus on certain concepts where I thought this approach to learning could be beneficial.

In case you have any thoughts, ideas, or spot some errors (most likely), feel free to write me - r.ali@surrey.ac.uk


#### Organization of this book

This book is still in its early stages of organization and I'll update things over time. So far my idea has been to organize it into 3 sections (but this may probably change):

1. Fundamental Audio Analysis - the basic concepts/techniques we need to do anything in audio DSP (a draft of this is complete). This part of the book has been largely based on the material I teach for one of my modules at the University of Surrey, UK on [Audio Signal Analysis](https://catalogue.surrey.ac.uk/2025-6/module/TON1023)
2. Audio processing - Concepts relating to the manipulation of audio. Planning to put several of the notebooks from (https://github.com/randyaliased/acs-sp-demos), so you can have a look at those already if you are curious.
3. Audio synthesis - There are a few notebooks I have that do some interactive synthesis for musical instruments and other objects, but they need some work. I think they would tie together nicely some of the concepts in the previous two sections.


#### How to use this book

Each notebook or chapter consists of two sections (i) an area of text (written in Markdown) which will explain the mathematical concept, and (ii) a code snippet where you can modify and execute the code to see the result.

At the start of each notebook, here's what you need to do:

1. There is a rocket ship button in the top-right hand corner. Hovering your cursor over this brings up a button which says "Live Code". Click this so that all the background Python stuff gets loaded. You will also see that all of the code snippets in the notebook have 4 buttons - "run", "run all", "add cell", and "clear".  Click "run" to execute a cell. 

2. Execute the very first cell of the notebook as this includes all of the necessary packages (various libraries) to be imported in order for following code snippets to work. 

3. Run the various code snippets in the notebook. The majority of these notebooks are interactive, in that a plot is generated where you can vary sliders and see/hear the output. This means that you do not even need to understand what all of the code is doing. Sometimes, I will highlight areas in the code where you can change the values of certain variables and you should then re-run the snippet to see the result. Although snippets of code may seem long at times, the majority of it is actually for rendering the plots.

4. If you want to add a cell and code up something of your own, click "add cell" and experiment! Note that once you leave a notebook though, any modifications you make get lost, so be sure to copy and paste them somewhere!

5. Have fun!

For the more Python-oriented folks: You'll probably realize that some of the Python code is not that efficient and it can certianly use cleaning up. My immediate goal was to get the interactive plots working and then worry about efficiency. For interactive plots, I've made use of the [Jupyter Widgets](https://ipywidgets.readthedocs.io/en/latest/examples/Using%20Interact.html) and [animations with Matplotlib](https://matplotlib.org/stable/users/explain/animations/animations.html).

This should be all you need to get started! I've made the [first notebook](https://randyaliased.github.io/acspjbook/main/fundamental/01_Sinusoidal_Model.html#) purposefully short and simple to demonstrate the idea behind this book, but then go into more detail in the following books. Hope you enjoy the journey!




