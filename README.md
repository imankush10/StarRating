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
You can install this component using npm or yarn:
```bash
npm install custom-stars
```
or
```bash
yarn add custom-stars
```
## Usage
Here's a simple example of how to use the StarRating component in your project:
```javascript
import React from 'react';
import StarRating from 'custom-stars';

const App = () => {
  const handleSetRating = (rating) => {
    console.log(`New rating: ${rating}`);
  };

  return (
    <div>
      <h1>Rate our product</h1>
      <StarRating
        maxRating={5}
        defaultRating={3}
        color="#fcc419"
        size={48}
        onSetRating={handleSetRating}
        messages={['Terrible', 'Bad', 'Okay', 'Good', 'Great']}
      />
    </div>
  );
};

export default App;

```
## Props
| Prop           | Type      | Default  | Description                                 |
|----------------|-----------|----------|------------------------------------------------|
| maxRating      | number    | `5`      | Maximum number of stars.                     |
| defaultRating  | number    |  `0`     | Default rating value.                        |
| color          | string    | #fcc419  | Color of the stars.                          |
| size           | number    |  48      | Size of the stars.                           |
| className      | string    | ""       | Additional CSS classes for the component.     |
| onSetRating   | function  | `null`   | Callback function that receives the new rating. |
| messages       | array     | `[]`     | Array of messages for each rating level.     |

## Example
Here's a more detailed example demonstrating various prop configurations:
```javascript
import React from 'react';
import StarRating from 'custom-stars';

const App = () => {
  const handleSetRating = (rating) => {
    console.log(`New rating: ${rating}`);
  };

  return (
    <div>
      <h1>Rate our product</h1>
      <StarRating
        maxRating={10}
        defaultRating={7}
        color="#ff6347"
        size={36}
        className="custom-star-rating"
        onSetRating={handleSetRating}
        messages={['Awful', 'Terrible', 'Bad', 'Poor', 'Meh', 'Okay', 'Good', 'Great', 'Awesome', 'Perfect']}
      />
    </div>
  );
};

export default App;

```
## Customization
You can customize the look and feel of the stars by adjusting the color and size props. Additionally, you can add custom CSS classes using the className prop.

## License
This component is open source and available under the MIT License.

#### Building for source

For production release:
Feel free to contribute or report issues on the [GitHub](https://github.com/imankush10/star-rating-component) repository.