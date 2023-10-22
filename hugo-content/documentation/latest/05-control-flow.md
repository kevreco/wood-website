## Control Flow

### Loop

```wood
// Loop forever
loop {
    // ...
}
```

#### Exit a loop

To break out of a loop we must give a label to the loop and use the `break` keyword.
```wood
label : loop {

	// ...

	if (condition)
	{
		break(label);
	}

	// ...
}
```

Using label allow us to explicitely break from any loop.
```wood
label :
	loop {
		loop {
			loop {
				
				// Some intructions ...
				
				if (condition)
				{
					break(label); // break out of all for loop
				}
			}
		}
	}	
```
> NOTE:\
Using a labeled block would be the only way to break?