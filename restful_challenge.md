1. Displays all of the projects
     HTTP Verb: GET                URL: /projects
     rails controller action:      projects#index 
     CRUD Action:                  READ
     Active Record Method:      Project.all 


2. Displays information about one project
     HTTP Verb: GET                URL: /projects/:id
     rails controller action:      projects#show 
     CRUD Action:                  READ
     Active Record Method:         Project.find(params[:id])


3. Displays a form to create a new project
     HTTP Verb: GET                URL: /projects/new
     rails controller action:      projects#new 
     CRUD Action:                  READ
     Active Record Method:         Project.new

4. Creates a new project based on given parameters
     HTTP Verb: POST               URL: /projects
     rails controller action:      projects#create 
     CRUD Action:                  CREATE
     Active Record Method:         Project.create(project_params)


5. Displays a form to update an existing project
     HTTP Verb: GET                URL: /projects/:id/edit
     rails controller action:      projects#edit
     CRUD Action:                  READ
     Active Record Method:         Project.find(params[:id])

6. Updates an existing project with given parameters
     HTTP Verb: PATCH              URL: /projects/:id
     rails controller action:      projects#update 
     CRUD Action:                  UPDATE
     Active Record Method:         Project.update(project_params)


7. Deletes an existing project
     HTTP Verb: DELETE             URL: /projects/:id
     rails controller action:      projects#destroy
     CRUD Action:                  DELETE
     Active Record Method:         Project.destroy(params[:id])


**NOTE - URL is always PLURAL