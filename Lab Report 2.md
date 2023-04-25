`StringServer.java`:
![Image](https://github.com/whatuptj/cse15l-lab-reports/blob/main/stringserver.png)
- `StringServer.java` contains a `main` method that firstly checks if a port number is provided when trying to run the server.
- Within the `main` method is another method called `Server.start` that takes the port number and passes it to the `URLHandler`
- `handleRequest` takes a URI object representing the incoming String as its parameter and returns a String representing the server's response to the request
1st `/add-message`:
![Image](https://github.com/whatuptj/cse15l-lab-reports/blob/main/idk.png)
- For this request, since the path does equal "/add-message" and the query isn't empty, "Idk if this works" is appended to `searchQuery`
2nd `/add-message`:
![Image](https://github.com/whatuptj/cse15l-lab-reports/blob/main/okay.png)
- For this request, since the path does equal "/add-message" and the query isn't empty, "okay it works now" is appended to `searchQuery`

