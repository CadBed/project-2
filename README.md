# project-2
index.html,1615453691018,2e137137095e9073305e262a6258de6161867c0f42755f03f822e7cb64c71ebc
 assets/favicon.af219669.svg,1615453691018,4310a0a4003e9d7557335a43c4a8eb712eaf813354b5a45af285aac7d84e4f8b
 assets/index.cada961e.css,1615453691018,22f93586aeed4a57d5d7a362fdb5d13311707c31b22b3dcc8fc7fe92db2996ea
 assets/index.a9d60add.js,1615453691018,2f206f74128bd60a61c20ec45c941b73887fb42eb7f8c865182ece8c6349259a
 assets/vendor.00093675.js,1615453691018,f7079922d6872630aecc89abacf8fcde15a9672b16349afdc43f28d10cb168be
 index.html,1615453813633,a7ef9ba1fe89ae8d3ce432ef4df678a9af75d6aaf1adab128b092e69e53fac72
 assets/index.cada961e.css,1615453813633,22f93586aeed4a57d5d7a362fdb5d13311707c31b22b3dcc8fc7fe92db2996ea
 assets/favicon.af219669.svg,1615453813633,4310a0a4003e9d7557335a43c4a8eb712eaf813354b5a45af285aac7d84e4f8b
 assets/index.455266c4.js,1615453813633,32a4fb644ae2aee9ae3c456ce0b173590e013acd6287466793ef29f0dcde5772
 assets/vendor.00093675.js,1615453813633,f7079922d6872630aecc89abacf8fcde15a9672b16349afdc43f28d10cb168be
 1  __mocks__/@excalidraw/excalidraw.js 

@@ -0,0 +1 @@
 module.exports = {};
 1  __mocks__/points-on-curve.js 

@@ -0,0 +1 @@
 module.exports = {};
 7  __mocks__/roughjs/bin/math.js 

@@ -0,0 +1,7 @@
 module.exports = {
   Random: class {
     next() {
       return 0;
     }
   },
 };
 1  __mocks__/roughjs/bin/rough.js 

@@ -0,0 +1 @@
 module.exports = {};
 8  babel.config.js 

@@ -0,0 +1,8 @@
 // babel.config.js
 module.exports = {
   presets: [
     ["@babel/preset-env", { targets: { node: "current" } }],
     "@babel/preset-react",
     "@babel/preset-typescript",
   ],
 };
   13  package.json 
 

 @@ -5,7 +5,8 @@
     "dev": "vite",
     "build": "vite build",
     "deploy": "npm run build && firebase deploy",
     "serve": "vite preview"
     "serve": "vite preview",
     "test": "jest"
   },
   "dependencies": {
     "@excalidraw/excalidraw": "^0.4.1",
 @@ -27,9 +28,19 @@
     "sass": "^1.32.8"
   },
   "devDependencies": {
     "@babel/core": "^7.13.10",
     "@babel/preset-env": "^7.13.10",
     "@babel/preset-react": "^7.12.13",
     "@babel/preset-typescript": "^7.13.0",
     "@types/jest": "^26.0.20",
     "@types/react": "^17.0.0",
     "@types/react-dom": "^17.0.0",
     "@types/react-test-renderer": "^17.0.1",
     "@vitejs/plugin-react-refresh": "^1.1.0",
     "babel-jest": "^26.6.3",
     "canvas": "^2.7.0",
     "jest": "^26.6.3",
     "react-test-renderer": "^17.0.1",
     "typescript": "^4.1.2",
     "vite": "^2.0.1"
   }
