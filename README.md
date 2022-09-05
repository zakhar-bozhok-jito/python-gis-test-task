# Junior Python developer test task (GIS)
![python3](https://img.shields.io/badge/-python3-yellowgreen)
## Helpful links (DON'T FORGET TO UPDATE LINKS)
To submit your application, please put your results into this [form](https://forms.gle/hLrkZvZDVFkBG7Wy6)
Feel free to ask questions [here](https://app.sli.do/event/es9DAm5Y8SipuNvhzqp96Q/live/questions)
## Overiview
GIS is Geospatial Information Systems. 
Sure we don't expect you to know what is GIS for the test task, but in further work you will have to work with it.

## Task
You have to develop a streets colouring algorithm using python3 and create a really simple web server where use can attach a file which should be processed.

## Requirements:
- Web site has to accept .zip archive with .shp file and other files required to read .shp (like .shx, .sbx, etc.)
- Server has to return generated image in base64 
- Solution has to generate images large enough to destignuish lines while zooming in
- Your repo with solution should contain file with explanation of how your algorithm works (it can be added to README.md with section Explanation)
- Web site should allow to generate .png from sample data. In other words sample data should be embedded into the solution (create separate button for that)
- Solution has to be dockerized so anyone can easily run it using `docker-compose up`
- Solution should work just by running './run.sh'

## Hints
- Task can be solved in at least 3 different ways
- Hashmap will be helpful here
- Key point of solving this task is to understand how to know that several lines are one street
- For plotting purpose you can use 'matplotlib'
- To read .shp file you can use 'fiona' or 'shapely' or any other lib you like
- To understand what is inside initial data you can use QGis