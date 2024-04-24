# ISSUE-RESOLVING-CHATBOT-FOR-BOOKING-AND-RESERVING-HOTEL-ROOMS
The "Issue-Resolving Chatbot for Booking and Reserving Hotel Rooms" project is focused on developing a cutting-edge chatbot system designed to enhance the hotel booking and reservation process while effectively addressing customer issues.

![image](https://github.com/czh001118/ISSUE-RESOLVING-CHATBOT-FOR-BOOKING-AND-RESERVING-HOTEL-ROOMS/assets/64961112/e37b1e3b-5e3e-4ba2-a80c-9a55e5f971b3)

## Chatbot Setup
Imported the necessary libraries, such as NLTK and PyTorch, and are ready to train the chatbot, the process typically involves several key steps. First, collect dataset of conversations, including pairs of queries, user inputs and corresponding responses. Let the intents stored in a JSON file, begin by loading the intents data from the JSON file into the program, typically using a library like JSON in Python. The loaded data contains information about various intents, including examples of user queries, associated questions, and potential responses. After that, start the training process for the chatbot. Starts by loading a set of intents and their associated patterns from a JSON file. It then preprocesses the data, tokenizes the words, and creates a bag-of-words representation for each pattern. Uses the NLTK library for text processing and the PyTorch library to build and train a neural network model. The neural network architecture is defined in the “NeuralNet” class, and the dataset is prepared using the “ChatDataset” class. The training loop involves iterating over epochs and batches, performing forward and backward passes, and optimizing the model using the Adam optimizer. The final trained model's state dictionary, along with essential information such as input size, hidden size, and output size, is saved to a file named "data.pth." This saved file can be later used to load the trained model and associated metadata for making predictions or deploying the chatbot. The training process is monitored by printing the loss at regular intervals, providing insights into the model's convergence.

![image](https://github.com/czh001118/ISSUE-RESOLVING-CHATBOT-FOR-BOOKING-AND-RESERVING-HOTEL-ROOMS/assets/64961112/440f9fcb-9103-4044-b1a0-b13b14eb2c17.png=100x100)
<img src="(https://github.com/czh001118/ISSUE-RESOLVING-CHATBOT-FOR-BOOKING-AND-RESERVING-HOTEL-ROOMS/assets/64961112/440f9fcb-9103-4044-b1a0-b13b14eb2c17)" width="150" height="150">

After the training process along with other necessary information, was saved to a file named "data.pth." In this runtime script, the trained model is loaded, and the chatbot enters a chat loop. The user can input messages, and the chatbot processes them using the trained model to generate responses. The chatbot utilizes a bag-ofwords approach to convert user input into a numerical representation, and the trained neural network predicts the intent of the input. If the predicted intent has a high probability and meets a certain confidence threshold, the chatbot randomly selects a response associated with that intent from the training data. If the confidence is below the threshold or the intent is not recognized well, the chatbot responds with a default message indicating a lack of understanding. The chatbot continues to prompt the user for input until the user types "quit," ending the chat.

![image](https://github.com/czh001118/ISSUE-RESOLVING-CHATBOT-FOR-BOOKING-AND-RESERVING-HOTEL-ROOMS/assets/64961112/67532120-dce0-49ff-8d32-1d681cb73bb6)

## Usability Testing

![image](https://github.com/czh001118/ISSUE-RESOLVING-CHATBOT-FOR-BOOKING-AND-RESERVING-HOTEL-ROOMS/assets/64961112/59d4a32b-e75f-434e-ab2a-2c8d5cc29ff4)
