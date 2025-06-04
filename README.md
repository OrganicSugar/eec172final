# EEC 172 Final - Golf Simulator

Sean Weber - Ryan Nguyen
## Project Description
Our motivation for this project was a combination of our enjoyment of minigolf as well as client-server models in software engineering. While discussing potential ideas for our project at the beginning, we remembered the requirement for at least 2 sensors, and we realized that most of our ideas did not work within these requirements. Then we both considered a minigolf style game, and as we both continued to consider the idea, the more we enjoyed it and continued to develop the idea to something we could act upon. Furthermore, our enjoyment of server-client models also added to the project, where we decided to make it so one board was the client that played the game but all the actual data was handled by the server.
The golf minigame consists of a client-run board which has access to basic tools such as a help screen as well as the gameplay of the minigolf courses. The client contains a menu screen the user can traverse. Selecting maps and looking at each map causes the client to send requests to the server using the REST API on AWS. The server will then get these AWS requests by actively sending GET requests to the AWS shadow, and then handles the requests, either updating map lists, identifying specific map data, updating leaderboards, or saving leaderboards when the client exits the program. The client receives these updates to play different maps, and uses the accelerometer as well as the tv remote to update the angle of the swing, and then enters the fire mode to swing the club, where the accelerometer uses the change in x, y, and z values to identify the power of the swing. Upon completion of the courses, the client is prompted to input their name and then sends their score to the server, which as stated updates leaderboards if their score was good enough.
## Maps
### Map 1
![map1](./IMG_6365.png)
### Map 2
![map1](./IMG_6366.png)
### Map 3
![map1](./IMG_6368.png)
## Demo Videos
### Start Sequence and General Layout
[![Watch on YouTube](https://img.youtube.com/vi/dNdLlvfLy9k/0.jpg)](https://youtube.com/shorts/dNdLlvfLy9k)

### Gameplay
[![Watch on YouTube](https://img.youtube.com/vi/Q7B1dx4AepA/0.jpg)](https://youtube.com/shorts/Q7B1dx4AepA)




