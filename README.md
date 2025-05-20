This is a repo of standard code examples and other standards not considered standard by us but required to make certain packages work. Strictly examples.

## Standard Code

When standard programs or packages are executed, they are zipped up and executed by the standard compiler (closed-source). That folder can be organized as you'd like but standards are `.stds` and executable code is `.std`. A full manual can be found here. You can execute .std files by themselves if they do not require standards.

Let's start with 'hello world'.

```
print "Hello World!"
```

We can go 0 to 100...
This example prints the vin of every car in the vehicle table.
```
cars [VHL] #Selects all cars
for: cars {
    print .vin
}
```

Make a window
```
^window: "Title", windowVar {
    view {
        label: "Hello World!"
    }
    view {
        maxheight 100
        scrollable true
        cars [VHL] #Selects all cars
        for: cars {
            label: .vin
        }
    }
}
```