---
layout: default
title: Basic Algorithm Scripting: Chunky Monkey
---
function chunkArrayInGroups(arr, size) {
  var toofer = [];
  var slice = [];
  
  for (var i = 0; i < (arr.length / size); i++) { //iterates as many times as there will be subarrays
    slice = arr.slice(i * size, (i * size + size)); //slices the array into chunks, beginning and ending at indices determined by the iteration and size
    toofer.push(slice); //adds chunkcs to toofer
  }
  return toofer;
}

chunkArrayInGroups(["a", "b", "c", "d"], 2);
