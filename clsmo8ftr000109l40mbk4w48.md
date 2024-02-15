---
title: "Top 50 One-Liners JavaScript"
datePublished: Tue Feb 13 2024 14:43:00 GMT+0000 (Coordinated Universal Time)
cuid: clsmo8ftr000109l40mbk4w48
slug: top-50-one-liners-javascript-1-1
canonical: https://codexdindia.blogspot.com/2024/02/top-50-one-liners-javascript.html
cover: https://cdn.hashnode.com/res/hashnode/imageupload/v1707968311082/5430b10a-c948-4712-9a1f-18f806736a68.jpeg

---

**Mastering JavaScript: Top 50 One-Liners Every Developer Should Know**

[![](https://cdn.hashnode.com/res/hashnode/imageupload/v1707968310255/a09cf45b-2414-471d-afd4-6048ef7f1976.jpeg)](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4lvdf9d073oxg32xx08r.jpeg)

**Introduction:**

JavaScript is a versatile and powerful programming language used extensively in web development. Whether you're a seasoned developer or just starting your journey, mastering JavaScript can significantly boost your productivity and efficiency. In this article, we'll explore the top 50 JavaScript one-liners that every developer should know. These concise and elegant solutions cover a wide range of common tasks, from manipulating arrays to working with strings and objects.

**1\. Checking if a Variable is Undefined:**

    const isUndefined = variable => typeof variable === 'undefined';
    

**2\. Checking if a Variable is Null:**

    const isNull = variable => variable === null;
    

**3\. Checking if a Variable is Empty:**

    const isEmpty = variable => !variable;
    

**4\. Checking if a Variable is an Array:**

    const isArray = variable => Array.isArray(variable);
    

**5\. Checking if a Variable is an Object:**

    const isObject = variable => typeof variable === 'object' && variable !== null;
    

**6\. Checking if a Variable is a Function:**

    const isFunction = variable => typeof variable === 'function';
    

**7\. Getting the Last Element of an Array:**

    const lastElement = array => array.slice(-1)[0];
    

**8\. Flattening an Array:**

    const flattenArray = array => array.flat();
    

**9\. Reversing a String:**

    const reverseString = str => str.split('').reverse().join('');
    

**10\. Generating a Random Number:**

    const randomNumber = (min, max) => Math.floor(Math.random() * (max - min + 1)) + min;
    

**11\. Removing Duplicates from an Array:**

    const removeDuplicates = array => [...new Set(array)];
    

**12\. Checking if an Array Contains a Specific Value:**

    const containsValue = (array, value) => array.includes(value);
    

**13\. Checking if a String Contains a Substring:**

    const containsSubstring = (str, substring) => str.includes(substring);
    

**14\. Getting the Current Date and Time:**

    const currentDateTime = () => new Date().toLocaleString();
    

**15\. Checking if a Year is a Leap Year:**

    const isLeapYear = year => (year % 4 === 0 && year % 100 !== 0) || year % 400 === 0;
    

**16\. Truncating a Number to a Specified Decimal Place:**

    const truncateNumber = (num, decimalPlaces) => Math.trunc(num * 10 ** decimalPlaces) / 10 ** decimalPlaces;
    

**17\. Checking if an Object has a Specific Property:**

    const hasProperty = (obj, property) => obj.hasOwnProperty(property);
    

**18\. Converting a String to Title Case:**

    const toTitleCase = str => str.replace(/\b\w/g, char => char.toUpperCase());
    

**19\. Repeating a String N Times:**

    const repeatString = (str, n) => str.repeat(n);
    

**20\. Generating a Range of Numbers:**

    const range = (start, end) => Array.from({ length: end - start + 1 }, (_, i) => start + i);
    

**21\. Summing Numbers in an Array:**

    const sumArray = array => array.reduce((acc, curr) => acc + curr, 0);
    

**22\. Getting the Maximum Value in an Array:**

    const maxArrayValue = array => Math.max(...array);
    

**23\. Getting the Minimum Value in an Array:**

    const minArrayValue = array => Math.min(...array);
    

**24\. Checking if a Number is Even:**

    const isEven = num => num % 2 === 0;
    

**25\. Checking if a Number is Odd:**

    const isOdd = num => num % 2 !== 0;
    

**26\. Checking if a String is Palindrome:**

    const isPalindrome = str => str === str.split('').reverse().join('');
    

**27\. Reversing the Order of Words in a String:**

    const reverseWords = str => str.split(' ').reverse().join(' ');
    

**28\. Checking if a Number is Prime:**

    const isPrime = num => {
     for (let i = 2; i <= Math.sqrt(num); i++) {
     if (num % i === 0) return false;
     }
     return num > 1;
    };
    

**29\. Converting Fahrenheit to Celsius:**

    const fahrenheitToCelsius = f => (f - 32) * 5 / 9;
    

**30\. Converting Celsius to Fahrenheit:**

    const celsiusToFahrenheit = c => (c * 9 / 5) + 32;
    

**31\. Factorial of a Number:**

    const factorial = n => n === 0 ? 1 : n * factorial(n - 1);
    

**32\. Fibonacci Sequence:**

    const fibonacci = n => n <= 1 ? n : fibonacci(n - 1) + fibonacci(n - 2);
    

**33\. Finding the Greatest Common Divisor (GCD) of Two Numbers:**

    const gcd = (a, b) => b === 0 ? a : gcd(b, a % b);
    

**34\. Finding the Least Common Multiple (LCM) of Two Numbers:**

    const lcm = (a, b) => (a * b) / gcd(a, b);
    

**34\. Shuffle an Array:**

    const shuffleArray = array => array.sort(() => Math.random() - 0.5);
    

**35\. Checking if a Number is a Perfect Square:**

    const isPerfectSquare = num => Math.sqrt(num) % 1 === 0;
    

**36\. Checking if a Number is a Power of Two:**

    const isPowerOfTwo = num => (num & (num - 1)) === 0 && num !== 0;
    

**37\. Checking if a Number is a Palindrome:**

    const isPalindromeNumber = num => num.toString() === num.toString().split('').reverse().join('');
    

**38\. Capitalize the First Letter of Each Word in a Sentence:**

    const capitalizeWords = sentence => sentence.replace(/\b\w/g, char => char.toUpperCase());
    

**39\. Counting the Occurrences of Each Element in an Array:**

    const countOccurrences = array => array.reduce((acc, val) => {
     acc[val] = (acc[val] || 0) + 1;
      return acc;
    }, {});
    

**40\. Sum of Squares of Digits of a Number:**

    const sumOfSquareDigits = num => num.toString().split('').reduce((acc, digit) => acc + Math.pow(parseInt(digit), 2), 0);
    

**41\. Converting a Number to Binary:**

    const toBinary = num => num.toString(2);
    

**42\. Converting a Binary Number to Decimal:**

    const binaryToDecimal = binary => parseInt(binary, 2);
    

**43\. Checking if a String is an Anagram of Another String:**

    const isAnagram = (str1, str2) => str1.split('').sort().join('') === str2.split('').sort().join('');
    

**44\. Converting an Object to Query Parameters String:**

    const objectToQueryString = obj => Object.entries(obj).map(([key, value]) => `${encodeURIComponent(key)}=${encodeURIComponent(value)}`).join('&');
    

**45\. Checking if a Year is a Leap Year (Using Ternary Operator):**

    const isLeapYear = year => (year % 4 === 0 && year % 100 !== 0) || year % 400 === 0 ? true : false;
    

**46\. Reversing an Array in Place:**

    const reverseArrayInPlace = array => array.reverse();
    

**47\. Finding the Maximum Value in an Array (Using Spread Operator):**

    const maxArrayValue = array => Math.max(...array);
    

**48\. Finding the Minimum Value in an Array (Using Spread Operator):**

    const minArrayValue = array => Math.min(...array);
    

**49\. Truncating a String to a Maximum Length and Appending Ellipsis:**

    const truncateString = (str, maxLength) => str.length > maxLength ? str.slice(0, maxLength) + '...' : str;
    

**50\. Finding the Longest Word in a Sentence:**

    const longestWord = sentence => sentence.split(' ').reduce((longest, current) => current.length > longest.length ? current : longest, '');
    

**Conclusion:** JavaScript one-liners are concise and powerful solutions to common programming tasks. By mastering these one-liners, you can write cleaner, more efficient code and become a more proficient JavaScript developer. Experiment with these examples and incorporate them into your projects to take your coding skills to the next level. Happy coding!