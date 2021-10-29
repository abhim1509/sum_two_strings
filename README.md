# sum_two_strings

/**
 * @param {string} num1
 * @param {string} num2
 * @return {string}
 */
var addStrings = function(num1, num2) {   
    return String(convertToInt(num1)+ convertToInt(num2))
};

function convertToInt(str){
    let    sum=0;
    for (var i = 1; i <= str.length; i++) {
        sum = sum*10 + parseInt(str.charAt(i-1));
    }
    console.log(sum);
    return sum;
}
