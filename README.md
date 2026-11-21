# Overtime Pay Calculation Formulas & Examples

A simple reference guide and JavaScript formula example for calculating regular pay, time and a half (1.5x), and double time (2x) overtime pay.

## Live Calculator
Try the free online tool here: [OT Calculator](https://otcalculator.us/)

## Basic Formula
- **Regular Pay** = Regular Hours × Hourly Rate
- **Time and a Half (1.5x)** = Overtime Hours × (Hourly Rate × 1.5)
- **Double Time (2x)** = Double-Time Hours × (Hourly Rate × 2)

## Simple JavaScript Example
```javascript
function calculateOvertime(hourlyRate, regularHours, otHours, doubleHours = 0) {
  const regularPay = hourlyRate * regularHours;
  const otPay = hourlyRate * 1.5 * otHours;
  const doublePay = hourlyRate * 2 * doubleHours;
  return {
    regularPay,
    otPay,
    doublePay,
    totalPay: regularPay + otPay + doublePay
  };
}
