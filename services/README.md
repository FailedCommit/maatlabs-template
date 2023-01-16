1. In `api` module, add/update your schema. I've added petstore.yml
2. In `api` module, run the `openApiGenerate` gradle task, to generate the code from the Spec
   - This step will generate code corresponding to the spec in `service` module
3. Run AppLauncher in `service` module
4. try `curl -I http://localhost:9090/pets/`
   - Note the port
   - Expected Output
     - HTTP/1.1 501
       Content-Length: 0
       Date: Mon, 16 Jan 2023 14:01:47 GMT
       Connection: close
     
   Note: 501 signifies that the API are not yet implemented. 