# week-one-assignment
var arr = [50, 100, 120, 180, 46, 67];
function secondLargest(arr){
    var max = Math.max.apply(null,arr);
    arr.splice(arr.indexOf(max),1);
    return Math.max.apply(null,arr);
}
module.exports = secondLargest
console.log(secondLargest(arr));
