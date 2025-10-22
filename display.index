<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Payroll Summary</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container">
    <h1>Payroll Summary</h1>
    <div id="output"></div>
    <button onclick="goBack()">Return to Form</button>
  </div>

  <script>
    const data = JSON.parse(localStorage.getItem("payrollData"));
    const output = document.getElementById("output");

    output.innerHTML = `
      <p><strong>Employee Name:</strong> ${data.name}</p>
      <p><strong>Daily Rate:</strong> ₱${data.rate.toFixed(2)}</p>
      <p><strong>Days Worked:</strong> ${data.days}</p>
      <p><strong>Gross Pay:</strong> ₱${data.grossPay.toFixed(2)}</p>
      <p><strong>SSS (5%):</strong> ₱${data.sss.toFixed(2)}</p>
      <p><strong>Pag-ibig (3%):</strong> ₱${data.pagibig.toFixed(2)}</p>
      <p><strong>Philhealth (2%):</strong> ₱${data.philhealth.toFixed(2)}</p>
      <p><strong>Tax (5%):</strong> ₱${data.tax.toFixed(2)}</p>
      <p><strong>Total Deduction:</strong> ₱${data.totalDeduction.toFixed(2)}</p>
      <p><strong>Net Pay:</strong> ₱${data.netPay.toFixed(2)}</p>
    `;

    function goBack() {
      window.location.href = "main.html";
    }
  </script>
</body>
</html>
