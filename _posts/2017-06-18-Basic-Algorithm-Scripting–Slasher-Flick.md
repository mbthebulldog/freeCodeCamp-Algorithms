---
layout: default
title: Basic Algorithm Scripting: Slasher Flick
---
function slasher(arr, howMany) {
  arr = arr.slice(howMany); //slices the end off of the array at the index indicated by howMany and returns the tail
  return arr;
}

slasher([1, 2, 3], 2);
