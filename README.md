def chatbot_response(user_input):
    user_input = user_input.lower()

    if "hello" in user_input or "hi" in user_input:
        return "Hello! How can I assist you today?"
    
    elif "how are you" in user_input:
        return "I'm just a chatbot, but thanks for asking! How about you?"
        
    elif "what are you" in user_input:
        return "I am a simple chatbot!"
        
    elif "can i meet you" in user_input:
        return "I can not meet you beacuse i am an application!"
        
    elif "what do you like most" in user_input:
        return "I do not like anything!"
        
    elif "which language do you know" in user_input:
        return "I know all languages!"

    elif "weather" in user_input:
        return "I can't check the weather, but it's always a good idea to carry an umbrella!"

    elif "help" in user_input:
        return "Sure! What do you need help with?"
        
    elif "ok" in user_input:
        return "ok,chat you again!"
        
    elif "bye" in user_input or "goodbye" in user_input:
        return "Goodbye! Have a great day!"    

    else:
        return "I'm sorry, I didn't understand that. Can you ask something else?"

# Example interaction
while True:
    user_input = input("You: ")
    if user_input.lower() in ["bye", "goodbye"]:
        print("Chatbot: Goodbye! Have a great day!")
        break
    response = chatbot_response(user_input)
    print("Chatbot:", response)
