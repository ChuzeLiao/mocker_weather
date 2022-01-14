# mocker_weather

## Introduction
In the actual project development process, the development mode of front-end and back-end separation is generally carried out. The front-end simulates the function of returning data from the background through mock or other plug-ins. In common webpack construction projects, by cooperating with webpack dev server or express to start the local service, you can directly simulate sending Ajax requests. If you want to simulate the data returned from the background, you have to restart a mock server service, which is more troublesome.

## This work
Use apimocker to mock OpenWeatherMap's `GET /data/2.5/weather` endpoint.  
I first create a json file and write a webServices `data/2.5/weather` and specifies that it returns a json file named `weather.json`.  
Then write the response json content in weather.json



## Useage

```bash
sudo apt update
sudo apt install nodejs -y
sudo apt install npm -y
sudo npm install -g apimocker
apimocker -c config.json
```

Then the mocker URL is `http://34.201.45.238:7878/data/2.5/weather`