# Independent Learning Project - Insertion Sort

## Introduction

Insertion sort is a sorting algorithm that sorts an array by inserting each element in it's correct position in a sorted sub-list. It works by comparing each element with the previous elements and then moving the elements to its correct position by shifting it to the right. 

## Algorithm Description

Step 1. 
    ``` for (let i = 1; i < arr.length; i++) {  //Here we use a traditional for loop to iterate over an array with i initialized to index 1 instead of 0. ```

Step 2.
    ``` let currentValue = arr[i]; //Here we assign arr[i] to the variable currentValue. This is an important step because when we find the number before our current index is greater than our current index the previous index becomes the current index (as seen on line 7), so we initialize a variable and set it to the value of our current index so that it's saved and we can use it later. ```

Step 3.
    ``` let j = i - 1; //j is initialized to i - 1 here to have the index that we are comparing our currentValue too. ```

Step 4.
    ``` while (j >= 0 && arr[j] > currentValue) { //We start a while loop here to implement our logic that once our index j is a valid index and our value at index j is greater than our current value, we want to replace the value at the index in front of j with the value of j. ```

Step 5.
    ``` arr[j + 1] = arr[j]; //The update of values if our while loop is true happens here. ```

Step 6.
    ``` j--; //We decrement j here to continue checking through our already sorted elements to make sure our currentValue is in the correct place. } ```

Step 7.
    ``` arr[j + 1] = currentValue; //Once our while loop is completed we take our currentValue that is "floating" in our saved variable and assign it to the index in front of j. } ```

    ![The Reassigning of our floating currentValue](insertionCode.png)

Step 8.
    ``` return arr; //Here we return our newly sorted arr. }; ```


## Big O Evaluation



### Time Complexity



### Space Complexity

## Use Cases



## Edge Cases and Concerns

## Citations

