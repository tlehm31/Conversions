function convert() {
  const inputValue = document.getElementById("userInput").value;
  const unit = document.getElementById("unit").value;
  const inchesToMm = unit === "inchesToMm";
  let result = 0;
  if (isNaN(inputValue)) {
    resultString = "Please enter a valid number.";
  } else if (unit === "inchesToMm") {
    result = inputValue * 25.4;
    resultString = `${inputValue} inches is ${result.toFixed(10)} millimeters.`;
  } else if (unit === "mmsToInch") {
    result = inputValue / 25.4;
    resultString = `${inputValue} millimeters is ${result.toFixed(10)} inches.`;
  } else if (unit === "inchesToCm") {
    result = inputValue * 2.54;
    resultString = `${inputValue} inches is ${result.toFixed(10)} centimeters.`;
  } else if (unit === "cmToInch") {
    result = inputValue / 2.54;
    resultString = `${inputValue} centimeters is ${result.toFixed(10)} inches.`;
  } else if (unit === "inchesToM") {
    result = inputValue / 39.37;
    resultString = `${inputValue} inches is ${result.toFixed(10)} meters.`;
  } else if (unit === "metersToInch") {
    result = inputValue * 39.37;
    resultString = `${inputValue} meters is ${result.toFixed(10)} inches.`;
  } else if (unit === "inchesToKm") {
    result = inputValue / 39370.0;
    resultString = `${inputValue} inches is ${result.toFixed(10)} kilometers.`;
  } else if (unit === "kmToInch") {
    result = inputValue * 39370.0;
    resultString = `${inputValue} kilometers is ${result.toFixed(10)} inches.`;
  } else if (unit === "feetToMm") {
    result = inputValue * 304.8;
    resultString = `${inputValue} feet is ${result.toFixed(10)} millimeters.`;
  } else if (unit === "mmsToFeet") {
    result = inputValue / 304.8;
    resultString = `${inputValue} millimeters is ${result.toFixed(10)} feet.`;
  } else if (unit === "feetToCm") {
    result = inputValue * 30.48;
    resultString = `${inputValue} feet is ${result.toFixed(10)} centimeters.`;
  } else if (unit === "cmToFeet") {
    result = inputValue / 30.48;
    resultString = `${inputValue} centimeters is ${result.toFixed(10)} feet.`;
  } else if (unit === "feetToM") {
    result = inputValue / 32.81;
    resultString = `${inputValue} feet is ${result.toFixed(10)} meters.`;
  } else if (unit === "metersToFeet") {
    result = inputValue * 32.81;
    resultString = `${inputValue} meters is ${result.toFixed(10)} feet.`;
  } else if (unit === "feetToKm") {
    result = inputValue / 3281.0;
    resultString = `${inputValue} feet is ${result.toFixed(10)} kilometers.`;
  } else if (unit === "kmToFeet") {
    result = inputValue * 3281.0;
    resultString = `${inputValue} kilometers is ${result.toFixed(10)} feet.`;
  } else if (unit === "yardToMm") {
    result = inputValue * 914.4;
    resultString = `${inputValue} yards is ${result.toFixed(10)} millimeters.`;
  } else if (unit === "mmsToYard") {
    result = inputValue / 914.4;
    resultString = `${inputValue} millimeters is ${result.toFixed(10)} yards.`;
  } else if (unit === "yardToCm") {
    result = inputValue * 91.44;
    resultString = `${inputValue} yards is ${result.toFixed(10)} centimeters.`;
  } else if (unit === "cmToYard") {
    result = inputValue / 91.44;
    resultString = `${inputValue} centimeters is ${result.toFixed(10)} yards.`;
  } else if (unit === "yardToM") {
    result = inputValue / 1.094;
    resultString = `${inputValue} yards is ${result.toFixed(10)} meters.`;
  } else if (unit === "metersToYard") {
    result = inputValue * 1.094;
    resultString = `${inputValue} meters is ${result.toFixed(10)} yards.`;
  } else if (unit === "yardToKm") {
    result = inputValue / 1094.0;
    resultString = `${inputValue} yards is ${result.toFixed(10)} kilometers.`;
  } else if (unit === "kmToYard") {
    result = inputValue * 1094.0;
    resultString = `${inputValue} kilometers is ${result.toFixed(10)} yards`;
  } else if (unit === "mileToMm") {
    result = inputValue * 1.609e+6;
    resultString = `${inputValue} miles is ${result.toFixed(10)} millimeters.`;
  } else if (unit === "mmsToMiles") {
    result = inputValue / 1.609e+6;
    resultString = `${inputValue} millimeters is ${result.toFixed(10)} miles`;
  } else if (unit === "mileToCm") {
    result = inputValue * 160900;
    resultString = `${inputValue} miles is ${result.toFixed(10)} centimeters.`;
  } else if (unit === "cmToMiles") {
    result = inputValue / 160900;
    resultString = `${inputValue} centimeters is ${result.toFixed(10)} miles.`;
  } else if (unit === "milesToM") {
    result = inputValue * 1609;
    resultString = `${inputValue} miles is ${result.toFixed(10)} meters.`;
  } else if (unit === "metersToMiles") {
    result = inputValue / 1609;
    resultString = `${inputValue} meters is ${result.toFixed(10)} miles.`;
  } else if (unit === "milesToKm") {
    result = inputValue / 1.609;
    resultString = `${inputValue} miles is ${result.toFixed(10)} kilometers.`;
  } else if (unit === "kmToMiles") {
    result = inputValue * 1.609;
    resultString = `${inputValue} kilometers is ${result.toFixed(10)} miles`;
  }
  console.log(resultString);
  const resultElement = document.getElementById("resultElement");
  resultElement.innerHTML = resultString;
}
