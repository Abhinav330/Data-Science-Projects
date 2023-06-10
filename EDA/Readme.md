# Title
Documentation on Top News Headlines Reader

## Table of Contents
- Introduction
- Purpose
- Dependencies 
- Installation
- Usages
- Examples
- Error Handling
- Best Practices
- Troubleshooting
- Limitations
- Conclusion

## Introduction
The Top News Headlines Reader is a python-based program that sets out to help users get top news headlines from around the world. With this program, users can get top news headlines from their preferred sources and save their time spent on sorting through a long list of articles. This program uses the newsapi.org API to access current news headlines across the globe. 

## Purpose
The purpose of this documentation is to assist stakeholders in understanding the functioning of the given Python code on Top News Headline Readers. It will provide valuable insight into the code’s functions, its dependencies, installation processes, and examples. 

## Dependencies
The program is dependent on the following modules;
- requests
- win32com.client
- json

## Installation
The following installations are necessary to run the code without any problems:
- Python must be installed
- An API key is needed from newsapi.org to access the latest news headlines.

The following packages could be installed in the command prompt or any Python integrated development environment (IDE) such as Pycharm:

```python
pip install requests
pip install pypiwin32
```

## Usages
The given code is a Python-based program that provides the functionality of accessing top news headlines from around the world and reading them through the computer's speaker. It prompts the user to provide the number of news headlines they need to access and returns a string with the given news headlines. Afterward, the program uses the Dispatch function from the win32com.client module to read the news to the user using the computer's speaker.

## Examples
Here are some examples of the Top News Headlines Reader being utilized:
#### Easy Example
```python
print(getnews(5)) # This prints out the top 5 news headlines.
```
#### Medium Example
```python
speaker(getnews(10)) 
# This accesses the top 10 news headlines and reads them aloud through the computer's speaker.
```
#### Hard Example
```python
while True: 
    print("\nWelcome to the Top News Headlines Reader Menu\n")
    print("1. Get the Latest News Headlines\n")
    print("2. Read News Headlines\n")
    print("3. Exit\n")
    option = input("Choose an option: ")

    if option =="1":
        count = int(input("Enter the number of news headlines you want to access: "))
        print(getnews(count))
    
    elif option=="2":
        count = int(input("Enter the number of news headlines to read: "))
        speaker(getnews(count))
    
    elif option == '3':
        print("\nThank you for using the Top News Headlines Reader. See you again!\n")
        break
```

## Error Handling
In case an error occurs, we can get one of the following error messages: 

1. Authentication Error - this error occurs when the user's API Key is invalid or incomplete.
2. Network Connection Error - this error occurs when there is no connection to the network or unstable network connections. 
3. Invalid User Input - this error will prompt when a user has provided an invalid input.

## Best Practices
Here are some best practices to ensure that the Top News Headlines Reader code is being utilized correctly and to avoid any issues:

1. Ensure that Python and the necessary packages are installed and up-to-date.
2. Always ensure to provide integer inputs to avoid invalid user input errors.
3. Make sure to use valid login credentials to avoid authentication errors.
4. Ensure to use a stable Internet connection while running the code.
5. Always keep track of the number of API calls being made to avoid any unnecessary charges on the API.

## Troubleshooting
For more troubleshooting, users should visit the [newsapi.org](https://newsapi.org/docs/errors) website for any problems associated with errors generated in the code.

## Limitations
There are some limitations that one may encounter while running this code that are beyond the control of the developer. They are:

1. As the API is an external service, sometimes it may not respond correctly or may be unavailable.
2. The free version of the API limits the number of requests to 500 per day, and this may affect the number of top news it can return.
3. It relies on the computer's speaker to deliver the news, and there may be occasional inconsistencies owing to the equipment being used.

## Conclusion
In conclusion, the Top News Headlines Reader is a useful program for accessing top news headlines worldwide. It is a valuable tool for busy individuals who want to stay updated on current events with the ease of running a simple Python code. This documentation should make it more accessible to stakeholders who want to understand its usage, limitations, and advantages.
