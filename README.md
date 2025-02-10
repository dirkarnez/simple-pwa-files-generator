[simple-pwa-files-generator](https://dirkarnez.github.io/simple-pwa-files-generator)
====================================================================================
### TODOs
- [ ] icon (launcher icon, macOS "mask-icon", apple "apple-touch-icon"...) generation
  - ```
    <link rel="apple-touch-icon" sizes="57x57" href="/icons/apple-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/icons/apple-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/icons/apple-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/icons/apple-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/icons/apple-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/icons/apple-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/icons/apple-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/icons/apple-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/icons/apple-icon-180x180.png">
    <link rel="icon" type="image/png" sizes="192x192"  href="/icons/android-icon-192x192.png">
    <link rel="icon" type="image/png" sizes="32x32" href="/icons/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="96x96" href="/icons/favicon-96x96.png">
    <link rel="icon" type="image/png" sizes="16x16" href="/icons/favicon-16x16.png">
    ``` 
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
