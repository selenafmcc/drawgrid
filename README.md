# drawgrid
A drawgrid for primitives! Mostly for my own convenience.
Made in Gamemaker (lol)

CHANGELOG
6.3.2019
 - Set origin to the center of a 2000x2000 canvas
 - Added canvas scrolling
 - Set scroll limits so user can't scroll outside of room boundaries
 - Added cursors for layer scrolling and layer identification. (Not implemented yet!)
 - Fullscreen didn't work so Maximise and manuall screen resize are in instead!
 - Side menu added.
 - Side menu is both draggable and minimisable (and maximisable, lol)
 - Side menu cannot be dragged outside of boundaries.
 - Layer Bar and Colour bar can now be hidden and unhidden.

FUTURE UPDATES

6.2.2019
 - Right now, the below stuff plans for LINE DRAWING. Controlling primitives will have to come a bit later.
 - IMPORTANT: Decide if, when HORSPC  and VERSPC are changed, the drawing while SCALE to that change, or their values will simply be UPDATED. IF A: Their X and Y is based on calculations from the POV of the origin. IF B: Their X and Y is seperate from their grid-based coordinates and only the coords depend on the origin.
 - Default colours (personal palette) and also a colour picker (inputting RGB would be the best way to do that)
 - Just occured to me, since we'll be using lines and primitives and stuff this is technically a vector drawing program?? Sexy.
 - Don't make this too complicated, yet. Focus on getting lines, nodes, etc. down. Then cosmetics like line width and colour can be done later.
 - A layer system! Each layer is an object (consider a layer cap)
 - Each layer object stores the nodes (points) as an array. Array structure should allow each entry to have an x, y, a colour, and up to 2 (for now) connections.
 - Node connections will simply list the index of the node they are connected to!
 - Deleting a node deletes all of its connections and all references to it. This is fine because:
 - When a new node is made, its index is simply the next empty slot in this layer's array.
 - Feature: Arrow colour changes based on the layer it's on..
 - Node displays its coords when you mous over it???? How would we do this without making every node an obj tho.....
 - Consider the possibility of making every node an obj so that it can display its coords when you mouse over it.
 - Side menu (draggable) shows:
     - Undo, Clear Screen (and clear layer?), and (MAYBE IF I CAN SWING IT!!!!!) Export buttons
     - Snap to grid toggle
     - Show/Hide nodes toggle?
     - X and Y of mouse (based on snap)
     - Horizontal spacing (type to change)
     - Vertical spacing (type to change)
     - Colour bar (grid of preselected colours with rgb input at the side) (can collapse)
     - Layer select (can collapse)
 - Zoom control (oh god) using the scroll wheel or using a zoom bar.
 - Feature: Consider settings menu to account for misc stuff (like GUI scaling for later monitors)
 - Make background grid colours variable, maybe, unlikely, actually, fuck that.
