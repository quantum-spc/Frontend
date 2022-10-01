1. 단순정렬
function simpleSort(arr) {
 var t;
 for (var i=0; i<arr.length-1; i++) {
  for (var j=i+1; j<arr.length; j++) {
    if (arr[i] > arr[j]) {
     t = arr[i];
     arr[i] = arr[j];
     arr[j] = t;
    } // End of if
  } // End of for // j
 } // End of for // i
 return arr;
}
console.log(simpleSort(new Array(3,1,4,2))); // 출력 1234

2. 버블정렬 
function bubbleSort(arr) {
 var t;
 for (var i=0; i<arr.length; i++) {
   for (var j=0; j<arr.length-1; j++) {
     if (arr[j] > arr[j+1]) {
       t = arr[j+1];
       arr[j+1] = arr[j];
       arr[j] = t;
     }
   } // End of for // j
 } // End of for // i
 return arr;
}
console.log(bubbleSort(new Array(3,1,4,2))); // 출력 1234

3. 삽입정렬
function insertionSort(arr) {
 var t;
 for (var i=1; i<arr.length; i++) {
   t = arr[i];
   for (var j=i-1; j>=0; j--) {
     if (arr[j] > t) {
       arr[j+1] = arr[j];
     } else {
       break;
     } // End of if
    } // End of for // j
    arr[j+1] = t;
   } // End of for // i
 return arr;
}
console.log(insertionSort(new Array(2,6,1,9,5))); // 출력 12569

4. 퀵정렬
function quickSort(arr) {
 if (arr.length < 2) {
  return arr;
 }
 var pivot = arr[Math.floor(arr.length/2)];
 var middle = arr.filter(function (data) {
   return data == pivot;
 });

 var low = quickSort(arr.filter(function (data) {
  return data < pivot;
 }));

 var high = quickSort(arr.filter(function (data) {
  return data > pivot;
 }));
 return low.concat(middle).concat(high);
}
console.log(quickSort(new Array(4,8,6,5,2,1,3,9,7))); // 출력 123456789
