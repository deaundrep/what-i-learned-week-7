# what-i-learned-week-7
## Array of Radioactive Mutants
* you can pass array into a function that uses that same line on its parameter, and your array after calling that function will have a different value as well.
ex.)
function changeLast(arr, value){
  arr[arr.length -1 ] = value;
}

function changeAllValuesTo(arr, value) {
  let i = arr.length;
  while (i--) {
    arr[i] = value;
  }
}

## String Theory
* string building!
ex.)
const repeatIt = function(str, num){
  let repeatStr = ''
  while(num > 0){
    repeatStr += str;
    num--;
  }
  return repeatStr;
}

const truncate = function(str){
  let result = ''
  for (let i = 0; i < str.length; i++){
    if (str[i] >= 15){
      result += '...'
    } else{
      result += str[i]
    }
  }
  return result;
}

## Mapmaker Mapmaker
* string-building for arrays!
ex.)
const absoluteValues = function(arr){
  let newArr = [];
  for(let i = 0; i < arr.length; i++){
      if(arr > 0 ? arr * -1 : arr ){
        newArr.push(arr[i])
      }
        }
    return newArr;
}

const upperCaseFirstLetters = function(arr){
  let newArr = [];
    for(let i = 0; i < arr.length; i++){
      let lowerCase = arr[i].slice(1, arr[i].length).toLowerCase();
      newArr.push(arr[i][0].toUpperCase() + lowerCase);
    }
    return newArr
}
