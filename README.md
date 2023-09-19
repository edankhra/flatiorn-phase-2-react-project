# flatiorn-phase-2-react-project

**Requirements**
- You must make a single page application (only one index.html file) using create-react-app.
- Your app should use at least 3 components in a way that keeps your code well organized.
- There should be at least 2 client-side routes using React RouterLinks to an external site.. Be sure to include a nav bar or other UI element that allows users to navigate between routes.

- Use a json-server to create a RESTful API for your backend and make both a GET and a POST request to the json server. Use a form to make your post request, specifically a controlled form/component. Additionally, you may choose to incorporate data from an external API but it is not required.

- You should keep your json-server data simple: avoid nested data and associations. You'll learn how to work with more complex data in the next two phases. Focus on the frontend for this project.
Upon return of json from your POST request, a state update by a setState function is required!


**Stretch Goals**
- Use more components and client-side routes.
- Add some styling: you're encouraged to write your CSS from scratch, either by using styled componentsLinks to an external site. or writing CSS files and using id/className to style your elements. You can also incorporate a UI framework (like React BootstrapLinks to an external site., Semantic UILinks to an external site., or Material UILinks to an external site.) if you prefer.
- Incorporate data from an external API. Check out this list of APIsLinks to an external site. if you need some inspiration!
- Anything else you'd like! These are only the basic requirements — you're free to explore and add on as much stuff as you'd like. 

**Setup**
- For this project, you will need two separate repositories: one for your frontend and one for your backend. This will make it easier to deploy your project later, should you choose to do so.

**Frontend Setup**
- Use create-react-app to generate starter code for your project. Follow the instructions on the create-react-appLinks to an external site. site to get started.

**Backend Setup**
- You can use this json-server templateLinks to an external site. to generate your backend code. Using this template will make it easier to deploy your backend later on.

- sIf you prefer, instead of using the template, you can create a db.json file in the root of your project with a structure that looks like this:

{
  "toys": [
    {
      "id": 1,
      "name": "Woody",
      "image": "http://www.pngmart.com/files/3/Toy-Story-Woody-PNG-Photos.png",
      "likes": 8
    },
    {
      "id": 2,
      "name": "Buzz Lightyear",
      "image": "http://www.pngmart.com/files/6/Buzz-Lightyear-PNG-Transparent-Picture.png",
      "likes": 14
    }
  ]
}
Then, assuming you have json-server installed globally, you can run this command to run the server:

 json-server --watch db.json
Whatever top-level keys exist in your db.json file will determine the routes available. In the example above, since we have a key of toys pointing to an array of toy objects, json-server will generate the following routes:

GET /toys
POST /toys
GET /toys/:id
PATCH /toys/:id
DELETE /toys/:id
You can consult the json-server docsLinks to an external site. for more information.