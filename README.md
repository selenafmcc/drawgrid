# drawgrid
A drawgrid for primitives! Mostly for my own convenience.
Made in Gamemaker (lol)

FUTURE UPDATES

6.2.2019
 - HEY! okay. So. Origin at 0,0, or Origin at the center, so the primitives and drawing can wrap around it? I like the second option more. Sleep on it.
 - Right now, the below stuff plans for LINE DRAWING. Controlling primitives will have to come a bit later.
 - IMPORTANT: Decide if, when HORSPC  and VERSPC are changed, the drawing while SCALE to that change, or their values will simply be UPDATED. IF A: Their X and Y is based on calculations from the POV of the origin. IF B: Their X and Y is seperate from their grid-based coordinates and only the coords depend on the origin.
 - Origin is obj_CONTROL (consider renaming lol). Room will scroll (eventually) but Origin cannot be moved further onto screen than the top left. Consider adding a border/buffer so that the top left of the grid is not the true top left of the programme screen, but lines still cannot be drawn past that desu ;)
 - Default colours (personal palette) and also a colour picker (inputting RGB would be the best way to do that)
 - Just occured to me, since we'll be using lines and primitives and stuff this is technically a vector drawing program?? Sexy.
 - Don't make this too complicated, yet. Focus on getting lines, nodes, etc. down. Then cosmetics like line width and colour can be done.
 - A layer system! Each layer is an object (consider a layer cap)
 - Each layer object stores the nodes (points) as an array. Array structure should allow each entry to have an x, y, a colour, and up to 2 (for now) connections.
 - Node connections will simply list the index of the node they are connected to!
 - Deleting a node deletes all of its connections and all references to it. This is fine because:
 - When a new node is made, its index is simply the next empty slot in this layer's array.
 - Feature: Arrow colour changes based on the layer it's on..
 - Node displays its coords when you mous over it???? How would we do this without making every node an obj tho.....
 - Consider the possibility of makeing every node an obj so that it can display its coords when you mouse over it.
 - Side menu (draggable) shows:
     - Undo, Clear Screen (and clear layer?), and (MAYBE IF I CAN SWING IT!!!!!) Export buttons
     - Snap to grid toggle
     - Show nodes toggle?
     - X and Y of mouse (based on snap)
     - Horizontal spacing (type to change)
     - Vertical spacing (type to change)
     - Colour bar (grid of preselected colours with rgb input at the side) (can collapse)
     - Layer select (can collapse)
     - Fullscreen toggle
 - Zoom control (oh god) using the scroll wheel or using a zoom bar.
 - Scroll control using either arrow keys or a space+clickdrag
 - Feature: Consider settings menu to account for misc stuff
 - Feature: Make side menu minimisable????? FUck...... shit......
 - Make background grid colours variable, maybe, unlikely, actually, fuck that.
