1.Compare two jason have the same properties without order
let obj1 = {name: "person 1", age: 30};
let obj2 = {age: 30, name: "person 1"};

if (JSON.obj1 === JSON.obj2) {
console.log("The two objects have the same properties.");
} else {
console.log("The two objects do not have the same properties.");
}
2.Display all flags in the console:

function printData() {
const countries = JSON.parse(this.responseText);
countries.forEach((coun) => console.log(coun.flags));
}

var request = new XMLHttpRequest();
request.addEventListener("load", printData);
request.open("GET", "https://restcountries.com/v3.1/all");
request.send();

3.Display all countries name region and population in the console:

function printData() {
const countries = JSON.parse(this.responseText);
countries.forEach((coun) => console.log(coun.name));
countries.forEach((coun) => console.log(coun.region));
countries.forEach((coun) => console.log(coun.population));
}

var request = new XMLHttpRequest();
request.addEventListener("load", printData);
request.open("GET", "https://restcountries.com/v3.1/all");
request.send();
