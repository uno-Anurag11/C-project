Weather Information Retrieval Program Documentation
Overview
This C++ program allows users to retrieve weather information for a specific city using the wttr.in service. Users are prompted to enter a city, and the program fetches the current weather information for that city from wttr.in.

Prerequisites
Before using the program, ensure that the following prerequisites are met:

C++ Compiler: You must have a C++ compiler installed on your system to compile and run the program.
Curl Library: The program uses the libcurl library to perform HTTP requests. Make sure the libcurl development headers are installed on your system.
Usage
Compilation
Compile the program using your preferred C++ compiler. For example, with g++:

sh
Copy code
g++ -o weather weather.cpp -lcurl
Execution
Run the compiled executable:

sh
Copy code
./weather
Input
Follow the prompts to enter the desired city.

Output
The program displays the current weather information for the specified city in the terminal.

Error Handling
The program checks for errors during the execution of the curl request and displays an error message if an error occurs.

Functions
size_t writeCallback(void *ptr, size_t size, size_t nmemb, std::string *data)
Description: Callback function to handle the received data from the HTTP request.
Parameters:
ptr: Pointer to the received data buffer.
size: Size of each data element.
nmemb: Number of data elements.
data: Pointer to a std::string object where the received data will be appended.
Returns:
The total number of bytes written.
int main()
Description: The main function of the program.
Returns:
0 on successful execution.
Dependencies
libcurl: The program depends on the libcurl library for performing HTTP requests.
