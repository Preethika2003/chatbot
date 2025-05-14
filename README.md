# chatbot
#chatbot
def chatbot_response(user_input):
    user_input = user_input.lower()
    responses = {
        "hi": "Hello! How can I assist you today?",
        "hello": "Hi there! What can I do for you?",
        "hey": "Hey! How can I help?",
        "good morning": "Good morning! How’s your day going?",
        "good evening": "Good evening! How can I assist you?",
        "bye": "Goodbye! Have a great day!",
        "goodbye": "See you soon! Take care!",
        "what is your name": "I'm a chatbot! You can call me ChatBuddy.",
        "who are you": "I'm your friendly chatbot here to assist you.",
        "where are you from": "I live in the cloud! ☁️",
        "what can you do": "I can chat with you, answer simple questions, and keep you entertained!",
        "how are you": "I'm just a chatbot, but I'm always good! How about you?"
    }

    return responses.get(user_input, "I'm sorry, I didn't understand that. Can you rephrase?")
while True:
    user_message = input("You: ")

    if user_message.lower() == "exit":
        print("Chatbot: Exiting... Have a nice day!")
        break

    response = chatbot_response(user_message)
    print("Chatbot:", response)
