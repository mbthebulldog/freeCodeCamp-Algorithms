---
layout: default
title: Basic Algorithm Scripting: Return Largest Numbers in Arrays
---
function largestOfFour(arr) {
  var largeArr = [];

  for (var i = 0; i < arr.length; i++) { //go through ever subarray
    var largest = 0;
  
    for (var j = 0; j < arr[i].length; j++) { //go through every number of the subarray
      largest = largest < arr[i][j] ? arr[i][j] : largest; //assign the largest number of the array to largest
    }
    largeArr.push(largest); //adds largest number to largeArr
  }
  
  return largeArr;
}

largestOfFour([[4, 5, -21, 3], [13, 27, 18, -26], [-32, -35, -37, -39], [1000, 5318008, 857, 1]]);
