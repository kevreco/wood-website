## Control Flow

### For Loop

```wood
// Loop forever
for() {
    // Some intructions...
}

// Exit loop

// we give the for loop a label, then
loop : for() {
	break(loop);
}

// A label is givent the for loop, then we can break from the for loop using the label.
loop2 : for() {
	for() {
		for() {
			// Some intructions...
			break(loop2); // all for loops
		}
	}
}
```
Using a labeled block would be the only way to break?