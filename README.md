<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Shipment Management Form - README</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 30px;
      line-height: 1.6;
      max-width: 800px;
    }
    h1, h2 {
      color: #2c3e50;
    }
    ul {
      margin-top: 0;
    }
    code {
      background-color: #f4f4f4;
      padding: 2px 5px;
      font-family: monospace;
    }
  </style>
</head>
<body>
  <h1>Shipment Management Form</h1>
  <p>This project is a web-based Shipment Management Form built with HTML, Bootstrap, jQuery, and a REST API backend provided by Login2Explore. The form allows users to create, update, and manage shipment records stored in a cloud-based database.</p>

  <h2>Features</h2>
  <ul>
    <li>Create a new shipment record by entering a unique Shipment No.</li>
    <li>Retrieve existing shipment details by entering the Shipment No.</li>
    <li>Update shipment details for existing shipments.</li>
    <li>Reset the form to enter a new shipment.</li>
    <li>Automatic creation and verification of the backend database and relation (table).</li>
    <li>Form validation to ensure all fields are filled before save or update.</li>
    <li>Responsive UI using Bootstrap for styling.</li>
  </ul>

  <h2>Technologies Used</h2>
  <ul>
    <li>HTML5 and CSS3 (Bootstrap 3.4.1)</li>
    <li>JavaScript and jQuery (3.5.1)</li>
    <li>Login2Explore REST API for database and relation management</li>
    <li>AJAX calls to interact with the backend API</li>
  </ul>

  <h2>Setup and Usage</h2>
  <p>Open the HTML file in any modern web browser (Chrome, Firefox, Edge).</p>
  <p>On page load, the application:</p>
  <ul>
    <li>Checks if the database (<code>SHIP-DB</code>) exists. If not, it creates the database.</li>
    <li>Checks if the relation (<code>SHIPMENT-rel</code>) exists. If not, it creates the relation with the specified schema.</li>
  </ul>

  <h3>To add a shipment:</h3>
  <ul>
    <li>Enter a unique <code>Shipment No.</code> and blur or press Enter.</li>
    <li>If the shipment does not exist, input fields will be enabled.</li>
    <li>Fill in the <code>Description</code>, <code>Source</code>, <code>Destination</code>, <code>Shipping Date</code>, and <code>Expected Delivery Date</code>.</li>
    <li>Click <code>Save</code> to store the shipment record.</li>
  </ul>

  <h3>To update a shipment:</h3>
  <ul>
    <li>Enter an existing <code>Shipment No.</code> and blur or press Enter.</li>
    <li>The shipment data will be fetched and populated in the fields.</li>
    <li>Edit the necessary fields and click <code>Update</code>.</li>
  </ul>

  <h3>To clear the form:</h3>
  <ul>
    <li>Click <code>Reset</code>.</li>
  </ul>
</body>
</html>
