SocketIO2Unity
==============

### About

This flow provides an example of using Node-Red to establish real time communication with a client application using Socket.IO.

In this case Node-Red polls WeatherUnderground and uses Socket.IO to transmit received events in real-time to the intended client application such as the Unity game engine. In this example Socket.IO has been configured to communicate on port `3000`. The input path is `/socket.io`.

**Note:** Unity must be configured as a Socket.IO client in order to receive the transmitted events. A Unity client on the same local machine as the Node-Red application would use the path `ws://127.0.0.1:3000/socket.io\EIO=4&transport=websocket` to connect.