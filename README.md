# Ai Chatbot API

Ai Chatbot API is a simple API powered by Google's Generative AI (Gemini) for generating conversational responses. It remembers conversation history and provides responses based on it.

## Installation

* ** Clone this repository to your local machine:  ''' git clone https://github.com/korede456/Ai-Chatbot '''
* ** Navigate into the project directory: ''' cd Ai-Chatbot '''
* ** Install dependencies using npm: ''' npm install '''
* ** Create a .env file in the root directory with the following content: ''' PORT=5000
API_KEY=YOUR_GOOGLE_API_KEY ''' Replace YOUR_GOOGLE_API_KEY with your actual Google API key.

## Usage

* ** Start the server: ''' npm start ''' or run the app.js file
* ** Use an HTTP client like Postman to interact with the API.
* ** Send a POST request to http://localhost:5000/ask with the following JSON body: ''' {
  "message": "Your message here"
} '''  Replace "Your message here" with the message you want to send to the chatbot.
* ** The API will respond with a JSON object containing the chatbot's response: ''' {
  "response": "Chatbot response here"
} """

## Additional Notes
By default, the API listens on port 5000. You can change this by modifying the PORT variable in the .env file.
The API currently only supports a single model (gemini-pro). If you want to use a different model, you'll need to modify the model parameter in the getGenerativeModel function call in app.js.
Handle errors appropriately based on your application's requirements.