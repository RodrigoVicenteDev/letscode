# IronBeers API
We will be building a React app so the API (server) needs to be built somewhere for us, right? You are completely right, it's deployed, and the root for the API is: https://ironbeer-api.fly.dev/
## EndPoints




|       Method         |Endpoint     |   Response (200)                  |HTML                         |
|----------------|-------------------|------------|-----------------------------|
|GET|/|[beers]          |  Get all the beers from the DB
|GET        |/:id         |{beer}         |Get a single/specific beer
|GET          |/random |{beer}   |Get a random beer from the DB
|POST          |/new|{message: "New beer successfully saved to database!"}  |Create a new beer (the fields are specified in the instructions)from the DB
|GET          |  /search?q=`{query}` |[beers]   |Get beers from the DB whose name contains the search term. For example `/search?q=lager` searches for all beers with lager in the name.
|DELETE        |/delete/:id      |{beer}         |Delete a single/specific beer



## Schemas
    
    `{    
    name: { type: String, required: true, trim: true },    
    image: { type: String, trim: true },    
    tagline: { type: String, trim: true },    
    contributed_by: { type: String, trim: true },    
    attenuation_level: { type: String, trim: true },    
    description: { type: String, trim: true },    
    first_brewed: { type: String, trim: true },    
    brewers_tips: { type: String },    
    },    
    { timestamps: true }    
    );` 

