---
layout: default
title: JavaScript Algorithms and Data Structures Projects: Caesars Cipher
---
function rot13(str) {
  var arr = [];
  
  for (var i = 0; i < str.length; i++) { //iterate through every letter
    var code = str.charCodeAt(i); //create a variable defined as the character code for the current character
    
    if (code >= 65 && code <= 90) {  //item is a letter A-Z (codes 65-90)
      if (code < 78) {  //item is a letter A-M (codes 65-77)
        arr.push(String.fromCharCode(code + 13));  // add 13 and add to arr
      }
      else  //item is a letter N-Z (codes 78-90)
      {
        arr.push(String.fromCharCode(code - 13));  //subtract 13 and add to arr
      }
    }
    else  //item is not a letter
    {
      arr.push(String.fromCharCode(code));  //simply add as-is to arr
    }
  }

  return arr.join('');  
}

// Change the inputs below to test
rot13("PBQRF? JR'ER QBVAT PBQRF ABJ!? GUNG'F OYBBQL OEVYYVNAG!");
