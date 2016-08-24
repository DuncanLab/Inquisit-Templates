IMPORTANT TAGS:

- INCLUDE: Includes other inquisit code to your experiment. Equivalent to importing the code.
- EXPT: The experiment tag that holds ordering for the experiment. Contains a sequence of blocks.
- BLOCK: Holds a specified number of trials
- TRIAL: Displays stimulusframes
- ITEM: Holds one or more string values. Ex. It can hold stim values for a column for a block.

All experiments must have one EXPT tag, which contains 1 or more block tag. The block tag must contain 1 or more trial tags. A trial Must contain 1 or more Stimulus Frames.


Possible Stimulus Frames:

	- text: Displays text on screen
	- picture: Displays image on screen
	- shape: Displays shape (rectangle, circle, triangle)


Stimulus Frames all have an items attribute. The items attribute must be given an item tag. The item tag contains one or more items. Every time the stimulus frame gets called within the trial (I.E. every time a trial that uses the stimulus frame gets called), it will iterate to another item in the items tag. You specify the ordering through the 'select' tag in the stimulus frame. Possible options available in: http://www.millisecond.com/support/docs/v5/html/language/attributes/select.htm. Ex. setting it to 'sequence' will iterate through the items values in the set order.