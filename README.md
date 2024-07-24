# Codsoft-ai-task-1
def chatbot_response(message):
    message = message.lower() 
    if message == 'hi' or message == 'hello':
        return 'Hello! How can I help you today?'
    elif message == 'bye':
        return 'Goodbye!'
    elif 'how are you' in message:
        return 'I am good, thank you!'
    else:
        return "I'm sorry, I don't have knowledge aboout that."

print("ChatBot: Hi there! How can I assist you today?")
while True:
    user_input = input("You: ")
    if user_input.lower() == 'exit':
        print("ChatBot: Goodbye!")
        break
    
    response = chatbot_response(user_input)
    print("ChatBot:", response)
