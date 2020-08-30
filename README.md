# vuejs-slider
A simple range slider component used to increment/decrement values within a range.

## Usage
The slider component exports only a slider component. The width of the component defaults to 100% of the parent element.

### `slider` Component
There are props available for interaction and styling:

- `min`: Number: minimum value for slider. Defaults to 0.
- `max`: Number: maximum value for slider. Defaults to 100.
- `rounded`: Boolean: determines if a border radius is applied to the slide bar and control. Defaults to false.
- `slideSize`:  String: the size of the slide bar ('10px', '1em', etc.). Defaults to 10px.
- `slideColor`: String: the color of the slide bar ('red', '#aaccee', etc.). Defaults to #ccc.
- `controlSize`: String: the size of the control on the slide ('10px', '1em', etc.). Defaults to 16px.
- `controlColor`: String: the color for the control on the slide ('red', '#aaccee', etc.). Defaults to #444.
