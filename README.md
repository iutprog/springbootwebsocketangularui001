# springbootwebsocketangularui001
🔥 Building a Real-time Chat Application: Spring Boot + WebSocket + Angular + Angular Material UI 🔥  In this step-by-step tutorial, we’ll create an amazing real-time chat application using Spring Boot, WebSocket, Angular, and Angular Material UI! 🚀


## 1. Set up Angular Material
ng add @angular/material

## Service for WebSocket logic
ng g s services/message

## Add dependencies for Stomp.js and SockJS:
npm install @stomp/stompjs
npm install sockjs-client
npm i --save-dev @types/sockjs-client

## install the global and process polyfill packages:
npm install global process --save

## add in package.json

 "browser": {
    "global": "global",
    "process": "process/browser"
  },

## add in angular.json

 "polyfills": [
     "zone.js",
    "src/polyfills.ts"  
 ],

## create Polyfills.ts in src/polyfills and add
	// src/polyfills.ts
	(window as any).global = window;

## add in tsconfig.app.json
  "files": [
    "src/main.ts",
     "src/polyfills.ts"
  ],
