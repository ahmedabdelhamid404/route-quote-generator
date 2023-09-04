# Quote Generator Project

## Introduction

Welcome to the Quote Generator project, developed during my time at Route Academy! This simple yet powerful application aims to inspire and motivate users by displaying quotes along with their respective author images and names.

## Technologies Used

The Quote Generator project was built using the following technologies:

- HTML5
- CSS
- Bootstrap
- Vanilla JavaScript

## Project Details

At the heart of this application is an array of quote objects. Each object contains:

- Author's name
- The quote itself
- Source URL of the author's image
- An alternate description for the image

The quotes' data is manually entered into a JavaScript file, ensuring a dynamic and ever-expanding collection of inspiring quotes.

## How it Works

The JavaScript code behind the Quote Generator includes the following key components:

### Getting Random Index

The `gettingIndex()` function generates a random number between 0 and 10, which corresponds to the indexes of the quotes array. It returns this index for further use.

### Displaying Quotes

The `newQuote()` function is where the magic happens! It calls `gettingIndex()` to obtain a random index. To prevent repeating quotes, it checks whether the quote has been previewed before by consulting the `usedIndexes` array. If the quote has already been shown, it generates a new index until it finds an unused one. Once it has a fresh index, it adds it to the `usedIndexes` array and displays the corresponding quote, author image, and name.

### Continuous Fresh Quotes

To ensure a continuous stream of unique quotes, the code includes a condition that resets the `usedIndexes` array when all quotes have been displayed at least once. It keeps only the last index to prevent repetition, providing a fresh and inspiring experience with every use.

## Try it Out

Give the Quote Generator a try and let us know what you think! It's a simple yet effective way to start your day with wisdom and insight. Enjoy the inspiration!
