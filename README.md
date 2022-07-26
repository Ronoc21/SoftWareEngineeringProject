# SoftWareEngineeringProject

Clear instructions for how to REQUEST data from the microservice you implemented. Include an example call.

To request data from the microservice I have implemented, the user would open Jia's software program in Python, once they arrived at the create world section, 
the software asks for the name, category, an overview, a description and the body of the entry. When the user finished the prompts, that data is sent to a listening 
server. The server is witten in Javascript with the npm library installed, and the server is listening on port 3000. 
When the program sends a message to the server, it takes the user entered data and submits encoded as a URL request. That URL request creates a JSON object 
The object is available in a web browser opened by the Python program, and it is also saved to the Javascript server.


Clear instructions for how to RECEIVE data from the microservice you implemented
Once the data is sent from the  Python program via http protocol to the listening server it can be recieved through a web browser that populates after 
submitting the user's info. It is also stored in the server itself as a URL that is parsed into an object. That object can be sent to a database for storage. 
For example ( and this example is just a Game of Thrones) the url looks like 
"http://localhost:3000/"/world_name:Essos,overview:5%20houses%20struggle%20for%20supremacy%20in%20a%20Game%20of%20Thrones,category_name:High%20Fantasy,entry_name:Game%20of%20Thrones,entry_body:in%20the%20game%20of%20thrones%20you%20win%20or%20you%20die)"

becomes the more usable

{world name: "Essos",
 overview:"5 houses struggle for supremacy in a Game of Thrones",
 category_name: "High Fantasy",
 entry_name: "A Game of Thrones",
 entry_body:"in the game of thrones you win or you die."
}
