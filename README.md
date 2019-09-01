# Broadcasting solution using websockets

This POC upload video chunks from browser using socket.io to a server which converts to a RMTP stream uisng ffmpeg.

MediaRecorder -> Socket.IO -> FFMPEG -> RTMP

## Run frontend

Open `broadcast.html` in chrome browser.

# Run backend

Add `RTMP_URL` to enviroment. If you are using a stream service like mux.io url is similler to `rtmp://live.mux.com/app/STREAM_KEY`. Replace your stream key with `STREAM_KEY`

.One way to do this is to running following command in terminal

`export RTMP_URL=rtmp://live.mux.com/app/STREAM_KEY`

## dependencies

* install ffmpeg
* Run `npm install`

To run the server.

`node server.js`