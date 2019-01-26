SocketIO2Unity
==============

## About

This flow provides an example of using Node-Red to establish real time communication with a client application using Socket.IO.

In this example Node-Red polls WeatherUnderground and uses Socket.IO to transmit received events in real-time to the intended client application such as the Unity game engine. To use the Weather Underground node the user will need an API key from the [Weather Underground API](https://www.wunderground.com/weather/api) site.

## Setup

The Socket.IO node has been configured to communicate on port `3000` with an input path of `/socket.io`.

A Socket.IO client running in on the same local machine in Unity would use the following path to connect `ws://127.0.0.1:3000/socket.io/?EIO=4&transport=websocket`.

**Note:** In May 2018 Weather Underground stopped distributing free API keys as a result of a decision by their parent companies The Weather Company and IBM. The API was officially restired at the end of 2018.