# Design and Verification of On-Chip Instruments for Functional Safety

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
  <h1>Motivation</h1>
  <p>The automotive industry has witnessed significant transformations towards the development of autonomous vehicles capable of interacting with their environment. This has led to increased emphasis on ensuring safety for end-users and their surroundings. Extensive research is being conducted at various levels - vehicle, system, and chip - to meet safety requirements and reduce the risk of fatalities due to electronic malfunctions.</p>

  <h2>Theory</h2>
  <p>The integration of functional safety measures in automotive chip design includes Clock Monitoring, Built-In Self-Test (BIST) for the Arithmetic Logic Unit (ALU), and Performance Monitoring Unit (PPMU). Clock Monitoring employs a counter-based methodology to address signal jitters and duty-cycle errors, enhancing functional safety. BIST conducts ALU testing and signature comparison to identify potential errors and facilitate timely corrective actions. PPMU monitors critical hardware events and provides insights into system performance, contributing significantly to comprehensive functional safety for automotive applications.</p>

  <h2>Implementation</h2>
  <ol>
    <li><strong>Clock Monitor:</strong> The clock monitor generates a similar signal to the main signal and compares it with the possibly erroneous clock using a counter approach. Rise edge detection and count accumulation are performed, and upon comparison of values when the checker clock signal rises, an error flag is raised.</li>
    <li><strong>BIST:</strong> Built-In Self-Test (BIST) instructions are stored within the system, which checks for flaws in the ALU upon system power-up. The BIST instructions are executed, and the output signature is compared with a pre-stored golden signature. Any discrepancies lead to an error flag being raised.</li>
    <li><strong>PPMU:</strong> The Performance Monitoring Unit (PPMU) plays a pivotal role in reporting DMA activities, BIST results, and clock monitoring data in automotive chip design. Its capability to provide insights into instruction execution times contributes significantly to performance analysis, ensuring a comprehensive approach to functional safety.</li>
  </ol>
</body>
</html>

