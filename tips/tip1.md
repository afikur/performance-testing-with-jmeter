## Add undo/redo in JMeter

By default in jmeter there's no undo or redo options available. But lucky for us we can enable this feature in 3 easy steps.

1. Goto `jmeter/bin` folder. Now open `jmeter.properties` file in your favorite text editor.
2. Search for the text `undo.history.size`. By default it's commented. Uncomment the line (remove the hash in front) 
3. Set the value to 25. By default it's 0

**Important:** You can set any natural numbers like 1,2,3,4...100 etc. But setting high number can slow down the application cause it consumes more memory. Just above the line `undo.history.size` you can see that 25 is recommended by JMeter.