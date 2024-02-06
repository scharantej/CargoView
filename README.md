## VoyagerSafe Web Application

### HTML Files

1. **index.html:**
   - The main HTML file that serves as the landing page of the web application.
   - Includes the necessary HTML code for the layout, such as navigation bar, header, and footer.
   - Contains the structure for the dashboard, with sections or tabs for different sensor types.
   - Implements the functionality for displaying mock data and receiving updates from the space satellite.

2. **register.html:**
   - The HTML file for registering cargo containers.
   - Contains a form for users to provide information about their cargo containers, including name, type, and destination.
   - Upon form submission, the data is sent to the server (Flask application) for processing.

3. **data.html:**
   - The HTML file for displaying real-time data from the cargo containers.
   - Contains a table or other suitable visual elements for presenting the data received from the satellite.
   - Continuously updates the displayed data to show the latest readings from the sensors.

### Routes

1. **Route to Register Cargo Containers:**
   - Endpoint: /register
   - Method: POST
   - Accepts information about the cargo containers from the registration form (index.html).
   - Processes the received data, validates it, and stores it in a database or other suitable storage mechanism.

2. **Route to Retrieve Real-Time Data:**
   - Endpoint: /data
   - Method: GET
   - Returns the real-time data collected from the space satellite.
   - The route is called periodically by the client (index.html) to update the displayed data.

3. **Route to Display Dashboard:**
   - Endpoint: /dashboard
   - Method: GET
   - Serves the dashboard page (index.html) to the user.
   - The route is accessed when the user opens the web application or navigates to the dashboard.