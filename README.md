# binarySort-
        function binarySearch(array, targetValue) {
          var min = 0;
          var max = array.length - 1;
          var guess;
      
          while (max >= min) {
       guess = Math.floor((max + min) / 2);
       if (array[guess] === targetValue) {
           return guess;
       }
       else if (array[guess] < targetValue) {
           min = guess + 1;
       }
      else {
          max = guess - 1;
          }
      }
      return -1;
      };
      
      binarySearch([1,2,3,4,5,6,7,8,9,10,11],4);
