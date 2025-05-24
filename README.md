Shipment Management Form
This project is a web-based Shipment Management Form built with HTML, Bootstrap, jQuery, and a REST API backend provided by Login2Explore. The form allows users to create, update, and manage shipment records stored in a cloud-based database.

Features
Create a new shipment record by entering a unique Shipment No.

Retrieve existing shipment details by entering the Shipment No.

Update shipment details for existing shipments.

Reset the form to enter a new shipment.

Automatic creation and verification of the backend database and relation (table).

Form validation to ensure all fields are filled before save or update.

Responsive UI using Bootstrap for styling.

Technologies Used
HTML5 and CSS3 (Bootstrap 3.4.1)

JavaScript and jQuery (3.5.1)

Login2Explore REST API for database and relation management

AJAX calls to interact with the backend API

Setup and Usage
Open the HTML file in any modern web browser (Chrome, Firefox, Edge).

On page load, the application:

Checks if the database (SHIP-DB) exists. If not, it creates the database.

Checks if the relation (SHIPMENT-rel) exists. If not, it creates the relation with the specified schema.

To add a shipment:

Enter a unique Shipment No. and blur or press Enter.

If the shipment does not exist, input fields will be enabled.

Fill in the Description, Source, Destination, Shipping Date, and Expected Delivery Date.

Click Save to store the shipment record.

To update a shipment:

Enter an existing Shipment No. and blur or press Enter.

The shipment data will be fetched and populated in the fields.

Edit the necessary fields and click Update.

To clear the form, click Reset.
