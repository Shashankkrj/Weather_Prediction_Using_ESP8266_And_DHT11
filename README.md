# Weather Prediction Using ESP8266 And DHT11
This project uses an ESP8266 chip and a DHT11 temperature and humidity sensor to collect data about the weather. The data is then sent to predict function of a trained machine learning model to predict the weather. The project also includes ThingSpeak platform that allows users for real-time data visualization of temperature, humidity, heat index and predicted weather.

### Requirements
1. ESP8266 Wi-Fi chip
2. DHT11 temperature and humidity sensor
3. Breadboard
4. Python 3
5. Jupyter Notebook
6. Arduino IDE

### STEPS FOR EXECUTION OF WEATHER PREDICTION
1. Make a Decision Tree ML model by training it with past Weather dataset containing temperature, humidity, heat index and description of weather as columns.
2. After that, use a library micromlgen to make header file named “DecisionTree.h” for the trained model and add it to Arduino IDE libraries.
3. Write code for the DHT11 and ESP8266 interfacing in Arduino IDE and include the header file in code for calling the predict function from the ML model.
4. Add the code for ThingsSpeak in Arduino IDE, so that the real time data is send to the server for analyzing the change in weather with respect to change in temperature, humidity and Heat Index time to time.
5. Now, start and code the ESP8266 by plugging it with the source point and it takes real-time value of temperature, humidity and heat index and pass it to the predict function of Decision Tree Model for predicting the current weather.
