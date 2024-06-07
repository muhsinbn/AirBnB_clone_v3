# AirBnB Clone - RESTFUL-API
The RESTFUL API is third version the AirBnB project at Holberton School that will collectively cover fundamental concepts of higher level programming. The goal of the AirBnB-clone RESTful API is to replicate the functionalities of the original AirBnB platform in a customized and independent environment. It aims to provide developers with a set of endpoints and resources that mimic the behavior of the AirBnB API, allowing them to build applications with similar features such as property listing, reservation management, user profiles, reviews, messaging, and payment processing. The AirBnB-clone RESTful API enables developers to develop their own version of a property rental platform that utilizes the same principles and design patterns as the original AirBnB platform.

#### Functionalities of this command interpreter:
* Listing properties: Users can search for and view available properties on AirBnB.
* Making reservations: Users can book and manage reservations for properties.
* Viewing reviews and ratings: Users can read reviews and ratings of properties from previous guests.
* Managing user profile: Users can update their profiles, add payment methods, and view booking history.
* Communicating with hosts: Users can send messages to hosts, ask questions about properties, and coordinate check-in details.
* Searching for properties: Users can search for properties based on location, price, amenities, and other criteria.
* Handling payments: Users can process payments for reservations and manage payment information.
* Managing notifications: Users can receive and manage notifications about bookings, messages, and other updates.

# Setup

## Using virtual env
* Clone this repository: `git clone "https://github.com/muhsinbn/AirBnB_clone_v3.git"`
* Access AirBnb directory: `cd AirBnB_clone_v3`

## Run the app

flask run


## File Descriptions
[API](app.py) - API contain specific commands, options, and parameters that can be used to interact with different functionalities or services. Some common components that an API  contain for a command-line interpreter include:. 

* `Endpoints`- Defined URLs that accept incoming requests and return responses with data or actions. 
* `Request methods:` - HTTP methods such as GET, POST, PUT, DELETE, PATCH that indicate the type of operation being performed on the resource.
* `Parameters:` - Data that can be submitted along with the request to customize the operation or filter results.
* `Response:` - Data or actions returned by the API in response to a request, typically in JSON or XML format.
* `Authentication` - Mechanisms for verifying the identity of the user or application making the API calls to ensure security.
* `Rate limiting` - Restrictions on the number of requests that can be made to the API within a certain time period to prevent abuse and ensure fair usage.
* `Documentation:` -  Detailed information on how to use the API, including endpoints, request formats, response formats, authentication methods, and usage examples.
* `Error handling` - Guidelines on how errors are communicated and how developers can handle and troubleshoot issues encountered while using the API.

#### `models/` directory contains classes used for this project:
[base_model.py](/models/base_model.py) - The BaseModel class from which future classes will be derived
* `def __init__(self, *args, **kwargs)` - Initialization of the base model
* `def __str__(self)` - String representation of the BaseModel class
* `def save(self)` - Updates the attribute `updated_at` with the current datetime
* `def to_dict(self)` - returns a dictionary containing all keys/values of the instance

## Endpoints
* GET /state - Retrieve a list of all states.
* POST /state - Create a new state.
* GET /state/<string:state_id> - Retrieve a state given its ID.
* DELETE /state/<string:state_id> - Delete a state given its ID.
* GET /city - Retrieve a list of all cities.
* POST /city - Create a new city.
* GET /city/<string:city_id> - Retrieve a city given its ID.
* PUT /city/<string:city_id> - Update a city given its ID.
* DELETE /city/<string:city_id> - Delete a city given its ID.

## Classes inherited from Base Model:
* [amenity.py](/models/amenity.py)
* [city.py](/models/city.py)
* [place.py](/models/place.py)
* [review.py](/models/review.py)
* [state.py](/models/state.py)
* [user.py](/models/user.py)


## Authors
Mohammed Yahaya - [Github](https://github.com/muhsinbnbn) / [Twitter](https://twitter.com/muhad_2020)  
Christian Chukwudi - [Github](https://github.com/chudistar01) / [Twitter](https://twitter.com/)


## License
Public Domain. No copy write protection. 
