# Documentation

## Title
Documentation of Python code to fetch and read top news

## Table of contents
1. Introduction
2. Purpose
3. Dependencies
4. Installation
5. Usages
6. Examples
7. Error Handling
8. Best Practices
9. Troubleshooting
10. Limitations
11. Conclusion

## Introduction
The following code is used to fetch and read top news from the newsapi.org website. This documentation explains the working of the code, its purpose, dependencies, installation steps, usages, examples, error handling, best practices, troubleshooting, and limitations.

## Purpose
The purpose of this code is to fetch and read top news from the newsapi.org website. It takes an integer as an input from the user and returns that number of top news headlines. This code can be used to keep the user updated with the latest news.

## Dependencies
This code has some external dependencies like Python requests and Python win32com modules which can be installed using the pip command.

## Installation 
To install the required modules, run the following command:
``` 
pip install requests
pip install pypiwin32
```

## Usages
This code can be used to fetch and read top news headlines from the newsapi.org website. To use this code, execute the following command:
```
python news.py
```
After running the above command, it will ask for an integer input from the user. Enter the required number of top news headlines to be read. Once entered, the code will fetch the top news headlines and read them out loud using the speakers of the system.

## Examples
### Easy level Example
To fetch and read top two news headlines, execute the following command:

`d = 2`

Output:

```
How many top news you want ?    2
Todays top 2 News are :
News 1 is India logs 37,154 Covid cases, 724 deaths in a day | India News - Times of India
News 2 is India vs Sri Lanka: Indian captain Shikhar Dhawan wins toss, opts to field in first ODI - Times of India
```

### Medium level example
To fetch and read top five news headlines, execute the following command:

`d = 5`

Output:

```
How many top news you want ?    5
Todays top 5 News are :
News 1 is India logs 44,230 Covid cases, 555 deaths | India News - Times of India
News 2 is Look forward to working with new colleagues: S Jaishankar on new Cabinet | India News - Times of India
News 3 is APJ Abdul Kalam death anniversary: Remembering Missile Man of India | India News - Times of India
News 4 is Priyanka Gandhi enters UP poll fray with 4-day visit | India News - Times of India
News 5 is Amazon, Big Basket issued notices for not having ‘country of origin’ details on products - Times of India
```

### Hard level example
To fetch and read top seven news headlines, execute the following command:

`d = 7`

Output:

```
How many top news you want ?    7
Todays top 7 News are :
News 1 is India logs 44,230 Covid cases, 555 deaths | India News - Times of India
News 2 is Look forward to working with new colleagues: S Jaishankar on new Cabinet | India News - Times of India
News 3 is APJ Abdul Kalam death anniversary: Remembering Missile Man of India | India News - Times of India
News 4 is Priyanka Gandhi enters UP poll fray with 4-day visit | India News - Times of India
News 5 is Amazon, Big Basket issued notices for not having ‘country of origin’ details on products - Times of India
News 6 is 23 lions test positive for Covid in Etawah | India News - Times of India
News 7 is Minor girl accuses 14-year-old boy of rape in Delhi, case registered | Delhi News - Times of India
```

## Error Handling
While running this code, some errors may occur. The possible errors and their solutions are provided below:
1. If the internet connection is not properly established, then an error will occur stating `ConnectionError`, in such case, establish proper internet connection and re-run the code. 
2. If the entered value is not an integer, an error will occur stating `Value Error`, in such case, input an integer value and re-run the code. 
3. If the entered value is zero or negative, an error will occur stating `ZeroDivisionError`, in such case, enter a positive integer value more than zero and re-run the code.

## Best Practices
Use the following practices to avoid errors while using this code:
1. Ensure that a proper internet connection is established before running the code.
2. Provide an integer value greater than zero while running the code.
3. Install required modules using pip before running the code.

## Troubleshooting
For further reference and troubleshooting, follow the given link:
- https://newsapi.org/docs/get-started

## Limitations
1. This code can only fetch and read the news in an English language.
2. The user can only input the value of top news headlines to be read; there is no option to select the category of news.
3. This code can only fetch and read the top news headlines of India.

## Conclusion
This code is used to fetch and read top news headlines. It takes an integer as input from the user and returns that number of top news headlines. This documentation explains the working of the code, its purpose, its dependencies, the installation steps, usages, examples, possible errors, best practices, and limitations. This code can be used to keep the user updated with the latest news.
