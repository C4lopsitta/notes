# Desktop application
A Desktop Application is a program. Java has **AWT** as a standard graphics library to draw on screen. Over AWT there is **Swing**.
All Swing widgets are *jsomething* (*jbutton*, *jradio*, ...) that are simply defined as **JComponent**.

# Layouts
## BorderedLayout
Default layout, it's a box with two rows spanning on the top and bottom marked "north" and "south" with two side columns called "east" and "west", plus a "center" zone.
If a part is empty, the nearby elements will span in and fill it.
## Panels
Panels are elements that contain layouts with their own layout.
## FlowLayout
FlowLayout positions elements one after the other in a linear manner.
# Widgets
## JFrame
A *jframe* simply is a Frame with window decorations that then contains other widgets.

# Threads
A thread in java is managed through the `Thread` object
## Runnable
Runnable is an interface that simplifies the uses of threads. It's essentially a thread reduced to minimum terms.