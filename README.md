[simple-pwa-files-generator](https://dirkarnez.github.io/simple-pwa-files-generator)
====================================================================================
### TODOs
- [ ] icon (launcher icon, macOS "mask-icon", apple "apple-touch-icon"...) generation
- [ ] manifest.json
- [ ] service worker (sw.js)
- [ ] service worker registration
  - ```html
    <script>
      if ('serviceWorker' in navigator) {
        navigator.serviceWorker
          .ready
          .then((registration) => {
            debugger;
          });
        
        navigator.serviceWorker
          .register('./sw.js')
          .then(registration => {
            console.log('Service Worker registered');
            debugger;
          })
          .catch(error => {
            console.error('Service Worker registration failed:', error);
          });
      }
    </script>
    ```
- [ ] `<head/>`
  - ```html
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    
    <meta name="viewport" content="user-scalable=no, initial-scale=1, maximum-scale=1, minimum-scale=1, width=device-width, height=device-height">
    
    <base href="/video-player/">
    
    <meta name="description" content="This is description">
  
    <title>Video Player</title>
  
    <link rel="apple-touch-icon" sizes="180x180" href="./apple-touch-icon.png">
    <link rel="icon" type="image/png" href="./favicon-32x32.png" sizes="32x32">
    <link rel="icon" type="image/png" href="./favicon-16x16.png" sizes="16x16">
    <link rel="manifest" href="./manifest.json">
    <link rel="mask-icon" href="./safari-pinned-tab.svg" color="#fed049">
    <meta name="theme-color" content="#fed049">
    ```
