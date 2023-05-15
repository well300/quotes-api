# Quotes API

📜 This is a simple Express.js API that provides a collection of quotes. The quotes are fetched from a JSON file named "quotes.json". The API has two endpoints: `/quote` and `/quote` (HTTP GET and POST, respectively).

## Installation

1. Clone this repository:
 ```
git clone https://github.com/well300/quotes-api.git
```
2. Install the dependencies:
```
cd quotes-api
npm install
```
3.Start the server:
```
npm start
```
## API Endpoints
### GET /quote
Fetches a random quote from the "quotes.json" file and returns it as a JSON response.
For example, in your client-side JavaScript code, you can use the `fetch` function to make a GET request to the `/quote` endpoint on your server:
```
fetch('https://your-server-url/quote')
  .then(response => response.json())
  .then(data => {
    // Handle the retrieved quote
    console.log(data);
  })
  .catch(error => {
    // Handle any errors
    console.error(error);
  });

```

Example response:
```
{
  "quote": "Be the change you wish to see in the world.",
  "author": "Mahatma Gandhi"
}
```
## POST /quote
Adds a new quote to the "quotes.json" file. The request body should contain the quote and author in JSON format.

Example request:
```
{
  "quote": "It always seems impossible until it's done.",
  "author": "Nelson Mandela"
}
```
Example response:
```
{
  "quote": "It always seems impossible until it's done.",
  "author": "Nelson Mandela"
}
```
## Error handling
If an error occurs while fetching or adding a quote, the API will return a JSON response with an "error" property:
```
{
  "error": "Unable to fetch a quote."
}
```
## License
This project is licensed under the [MIT License](LICENSE). 📄⚖️

Enjoy the adorable cat memes and have a fantastic time with Meme Kitty Express! 😸🌟
