# ragu-components
Simple approach for sharing shared components in microfrontend pattern.

## Qick start

Host shared components
```
$ cd shared-components; yarn; npx ragu-cli dev --directory ./src;
```

Host static app
```
$ python -m SimpleHTTPServer
```
---

## How it works
- Host shared components with ragu serice
  ```
   $ npx ragu-cli dev --directory ./src
   
    📦 your build is ready!

    Output path: /Users/nirajmaharjan/sandbox/my-ragu-mf/shared-components/.ragu-components
    Base URL: http://localhost:3100

    🗺 Component Routes:
    ▸ my-mfe: http://localhost:3100/components/my-mfe
    ▸ my-mfe2: http://localhost:3100/components/my-mfe2


    🔭 Preview Routes:
    ▸ my-mfe: http://localhost:3100/preview/my-mfe
    ▸ my-mfe2: http://localhost:3100/preview/my-mfe2
  ```
  
- consume shared componets 
  ``` 
      <ragu-framework src="http://localhost:3100/preview/my-mfe?name=World"/>
  ```

