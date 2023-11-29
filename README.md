# Train Control System

Welcome to the Train Control System repository! This JavaScript implementation allows you to manage and control trains, including basic trains and high-speed trains.

## Classes

### `Train`

The `Train` class is the base class for all train instances. It is initialized with parameters for color and lights status. The class provides methods for toggling lights, checking lights status, obtaining the object itself, and retrieving its prototype.

#### Methods

- **`toggleLights()`**: Toggles the lights on or off.
- **`lightsStatus()`**: Logs the current lights status to the console.
- **`getSelf()`**: Logs the current train instance to the console.
- **`getPrototype()`**: Logs the prototype of the current train instance to the console.

### `HighSpeedTrain`

The `HighSpeedTrain` class extends the `Train` class and introduces additional features specific to high-speed trains. It includes parameters for the number of passengers and the high-speed mode status. This class overrides the `toggleLights` method to include a custom message specific to high-speed trains.

#### Methods

- **`toggleHighSpeed()`**: Toggles the high-speed mode on or off.
- **`toggleLights()`**: Overrides the base class method to include a custom message for high-speed trains.

## Usage

To use the Train Control System, instantiate train objects and high-speed train objects using the provided classes. You can then manipulate their properties using the provided methods.

### Example

```javascript
var myFirstTrain = new Train('red', false);
console.log(myFirstTrain); // Train {color: 'red', lightsOn: false}

var highSpeed1 = new HighSpeedTrain(200, false, 'green', false);
highSpeed1.toggleLights(); // Lights on? true, Lights are 100% operational.
