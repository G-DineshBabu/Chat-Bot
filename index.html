// Require the Dialogflow and MongoDB packages
const dialogflow = require('dialogflow');
const { MongoClient } = require('mongodb');

// Set up Dialogflow client
const projectId = 'js-chatbot-urng'; // Replace with your own Dialogflow project ID
const sessionId = '9b515732-e11b-451d-9478-4fd56da1d180'; // Replace with a unique session ID for your user
const sessionClient = new dialogflow.SessionsClient();
const sessionPath = sessionClient.projectAgentSessionPath(projectId, sessionId);

// Define function to send user input to Dialogflow and retrieve a response
async function getChatbotResponse(userInput) {
  const request = {
    session: sessionPath,
    queryInput: {
      text: {
        text: userInput,
        languageCode: 'en-US'
      }
    }
  }

  const responses = await sessionClient.detectIntent(request);
  const result = responses[0].queryResult;
  return result.fulfillmentText;
}

// Connect to the MongoDB database
const url = 'mongodb://localhost:27017'; // Replace with your own MongoDB connection string
const dbName = 'Gurju'; // Replace with your own database name

async function connectToMongoDB() {
  const client = await MongoClient.connect(url);
  const db = client.db(Gurju);
  console.log('Connected to MongoDB');
  return db;
}

// Handle user input and display chatbot response
async function handleUserInput() {
  const userInput = document.getElementById('user-input').value; // Get the user's input from a form input field
  const chatbotResponse = await getChatbotResponse(userInput); // Call the getChatbotResponse function with the user's input
  const db = await connectToMongoDB(); // Connect to the MongoDB database
  // Save the user's input and chatbot response to the database
  const collection = db.collection('Dinesh');
  const result = await collection.insertOne({
    user: userInput,
    chatbot: chatbotResponse,
    timestamp: new Date()
  });
 } // Display the chatbot's response in the chatbot interface
 const chatbotInterface = document.getElementById('chatbot-interface'); // Replace with the ID of your chatbot interface
 const chatbotMessage = document.createElement('div');
 chatbotMessage.classList.add('chat-message');
 chatbotMessage.innerHTML = `<p>${chatbotResponse}</p>`;
 chatbotInterface.appendChild(chatbotMessage);



// Add event listener to form submit button
const form = document.getElementById('chat-form'); // Replace with the ID of your chat form
form.addEventListener('submit', (event) => {
  event.preventDefault(); // Prevent the form from submitting
  handleUserInput(); // Call the handleUserInput function to handle the user's input
});

const express = require('express')
const app = express()

app.get('/', (req, res) => {
  res.sendFile(__dirname + '/index.html')
})

app.listen(3000, () => {
  console.log('Server started on port 3000')
})
console.log('User input:', userInput)
console.log('Chatbot response:', result.fulfillmentText)


