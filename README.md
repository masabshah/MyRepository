# MyRepository
This is my first repository
<br>
Author - Masab Shah
#include <iostream>
#include <string>
using namespace std;
string getResponse(const string& input) {
// Convert the input to lowercase to handle case-insensitive matching
string lowerInput=input;
for (char &c:lowerInput) {
c=tolower(c);
}
// Simple responses based on input
if (lowerInput=="hello"||lowerInput=="hi") {
return "Hello! How can I help you today?";
} else if (lowerInput=="how are you?") {
return "I'm a bot, so I'm always good! How about you?";
} else if (lowerInput=="what is your name?") {
return "I'm a simple chatbot created in C++ by Masab Shah.";
} else if (lowerInput=="bye" || lowerInput=="goodbye") {
return "Goodbye! Have a great day!";
} else {
return "I'm not sure how to respond to that.";
}
}
int main() {
string input;
cout<<"Chatbot:Hello! Type 'bye' to end the conversation."<< endl;
// Chat loop
while (true) {
cout<<"You:";
getline(cin, input);
// Check for termination condition
if (input=="bye" || input=="goodbye") {
cout << "Chatbot: " << getResponse(input) << endl;
break;
}
// Get response from the bot and print it
string response=getResponse(input);
cout<<"Chatbot:"<< response<<endl;
  }
return 0;
}
