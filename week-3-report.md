## Connor Wu - Week 3 Lab Report

This report will demonstrate the creation of a webserver called StringServer,
and explain a bug found during lab 3.

## Part 1: StringServer

I created a file called StringServer.java containing a handler class and a StringServer class that initiates the server. The backend is implemented using the same Server.java file provided during lab.

StringServer.java:

```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String myStrings = "";

    @Override
    public String handleRequest(URI url) {
        if (url.getPath().equals("/add-message")) {
            String[] param = url.getQuery().split("=");
            myStrings = myStrings + param[0] + "\n";
            return myStrings;
        } else {
            return "404 Not Found!";
        }
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if (args.length == 0) {
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```
