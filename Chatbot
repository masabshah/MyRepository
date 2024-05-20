#include <iostream>
#include <string>
using namespace std;
string getResponse(const string& input) {
// Convert the input to lowercase to handle case-insensitive matching
string Input=input;
for (char &c:Input) {
c=tolower(c);
}
// Simple responses based on input
if (Input=="hello"||Input=="hi") {
return "Hello! How can I help you today?";
} else if (Input=="how are you?") {
return "I'm a bot, so I'm always good! How about you?";
} else if (Input=="what is your name?") {
return "I'm a simple chatbot created in C++ by Masab Shah.";
} else if (Input=="bye" ||Input=="goodbye") {
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
