### Custom Stars Component

A highly customizable React component for star rating, allowing users to easily rate items with a star-based system. This component is flexible and can be integrated into any project with minimal setup.

## Features

- Adjustable maximum rating
- Customizable default rating
- Changeable star color and size
- Callback function for rating updates
- Optional messages for different rating levels
- Installation
- You can install this component using npm or yarn
  :

## Installation

Just download this file and put it inside your src (or components) folder and then import it

```bash
git clone https://github.com/imankush10/star-rating-component
```

## Usage

Here's a simple example of how to use the StarRating component in your project:

```javascript
import StarRating from "./StarRating";

const App = () => {
  return (
    <StarRating
      maxRating={5}
      defaultRating={3}
      color="#fcc419"
      size={48}
      onSetRating={handleSetRating}
      messages={["Terrible", "Bad", "Okay", "Good", "Great"]}
    />
  );
};

export default App;
```

## Props

| Prop          | Type     | Default | Description                                     |
| ------------- | -------- | ------- | ----------------------------------------------- |
| maxRating     | number   | `5`     | Maximum number of stars.                        |
| defaultRating | number   | `0`     | Default rating value.                           |
| color         | string   | #fcc419 | Color of the stars.                             |
| size          | number   | 48      | Size of the stars.                              |
| className     | string   | ""      | Additional CSS classes for the component.       |
| onSetRating   | function | `null`  | Callback function that receives the new rating. |
| messages      | array    | `[]`    | Array of messages for each rating level.        |

## Customization

You can customize the look and feel of the stars by adjusting the color and size props. Additionally, you can add custom CSS classes using the className prop.

## License

This component is open source and available under the MIT License.

#### Building for source

For production release:
Feel free to contribute or report issues on the [GitHub](https://github.com/imankush10/star-rating-component) repository.
