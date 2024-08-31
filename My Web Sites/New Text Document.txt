const num1 = document.getElementById("num1");
const num2 = document.getElementById("num2");
const num3 = document.getElementById("num3");
const num4 = document.getElementById("num4");
const num5 = document.getElementById("num5");
const num6 = document.getElementById("num6");
const num7 = document.getElementById("num7");
const num8 = document.getElementById("num8");
const num9 = document.getElementById("num9");
const num10 = document.getElementById("num10");
const searchNum = document.getElementById("searchNum");
const searchBtn = document.getElementById("searchBtn");
const result = document.getElementById("result");
const sortBtn = document.getElementById("sortBtn");
const sortedArray = document.getElementById("sortedArray");

searchBtn.addEventListener("click", function() {
  const numbers = [
    num1.value,
    num2.value,
    num3.value,
    num4.value,
    num5.value,
    num6.value,
    num7.value,
    num8.value,
    num9.value,
    num10.value
  ];
  const searchVal = searchNum.value;

  if (numbers.includes(searchVal)) {
    result.textContent = `${searchVal} is present in the array.`;
  } else {
    result.textContent = `${searchVal} is not present in the array.`;
  }
});

sortBtn.addEventListener("click", function() {
  const numbers = [
    num1.value,
    num2.value,
    num3.value,
    num4.value,
    num5.value,
    num6.value,
    num7.value,
    num8.value,
    num9.value,
    num10.value
  ];

  const sorted = numbers.sort((a, b) => a - b);
  sortedArray.textContent = `Sorted Array: [${sorted}]`;
});
