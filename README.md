# Define the chatbot's responses based on interests
career_paths = {
    "technology": "Based on your interest in technology, you might consider a career in software development, data science, cybersecurity, or IT management.",
    "science": "If you're interested in science, careers such as research scientist, biotechnologist, or environmental scientist might be a good fit.",
    "arts": "For those passionate about the arts, consider careers in graphic design, illustration, music production, or fine arts.",
    "business": "With an interest in business, you could explore roles in management, entrepreneurship, marketing, or finance.",
    "healthcare": "If you're drawn to healthcare, consider becoming a doctor, nurse, pharmacist, or healthcare administrator.",
    "education": "Those interested in education might pursue teaching, educational administration, or curriculum design."
}

# Function to handle user input and provide career guidance
def career_guidance_chatbot():
    print("Welcome to the Career Guidance Chatbot!")
    print("Please tell me about your interests (e.g., technology, science, arts, business, healthcare, education): ")
    
    while True:
        # Get user input
        user_input = input("Your interest: ").strip().lower()

        # Check if the user wants to exit
        if user_input in ["exit", "quit", "bye"]:
            print("Thank you for using the Career Guidance Chatbot. Goodbye!")
            break

        # Provide career guidance based on the input
        if user_input in career_paths:
            print(career_paths[user_input])
        else:
            print("Sorry, I don't have information on that interest. Please try another or type 'exit' to quit.")

# Run the chatbot
if __name__ == "__main__":
    career_guidance_chatbot()
