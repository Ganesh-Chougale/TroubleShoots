### Problem:  
#### Terminal:  
```bash
> frontend@0.1.0 start
> react-scripts start

Cannot find module 'ajv/dist/compile/codegen'
```  
### Solution:  
#### Terminal:  
```bash
npm install --save-dev ajv@^7
```  