currently in development
## Overview

This project is a React application that interacts with a WordPress CMS using Axios for API calls.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/IliaZolas/dmc-frontend-main.git
    ```
2. Navigate to the project directory:
    ```bash
    cd dmc-frontend-main
    ```
3. Install dependencies:
    ```bash
    npm install
    ```

## Usage

1. Start the development server:
    ```bash
    npm start
    ```
2. Open your browser and navigate to `http://localhost:3000`.

## API Calls

This project uses Axios to make API calls to a WordPress CMS. Below is an example of how to make a GET request:

```javascript
import axios from 'axios';

const fetchPosts = async () => {
  try {
     const response = await axios.get('https://your-wordpress-site.com/wp-json/wp/v2/posts');
     console.log(response.data);
  } catch (error) {
     console.error('Error fetching posts:', error);
  }
};

fetchPosts();
```

## Contributing

Feel free to submit issues and pull requests.

## License

This project is licensed under the MIT License.