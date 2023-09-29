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

// W give the for loop a label, then we can break from the loop using the label.
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


