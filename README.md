# Note

This is a simple application of checking out how to build a go server
there are various steps to this. If you wish to see the progress follow
the git logs

# TODO
* Add the data directory to the git ignore
* Add a handler to make the web root redirect to /view/FrontPage. --- Done already, will remove it and implement something more functional as printing all the available directories.
[the web root redirects to /home and actually makes a list of all the available wikies]
* Spruce up the page templates by making them valid HTML and adding some CSS rules.
* Implement inter-page linking by converting instances of [PageName] to
  <a href="/view/PageName">PageName</a>. (hint: you could use regexp.ReplaceAllFunc to do this)

# Concepts covered
* Creating a simple data structure
* Reading and writing to files
* Importing and using packages like net/http to build web application
* Processing and doing html templating using html/template
* using regexp package to do regular expression validation
* For loop
* Closures

# Functionalities
* View wiki pages:
Load and view the wiki page
localhost:9000/view/[wiki name]
* Edit
Edit the wiki pages. by loading the exiting weki in a form for edit
localhost:9000/edit/[wiki name]
* Save
Save the edited wikis by sending the form from edit to an action
localhost:9000/save/[wiki name]

# Running
To run the application run the following command. `go run wiki.go`

You can compile and run the program like this:
`$ go build wiki.go`
`$ ./wiki`
(If you're using Windows you must type "wiki" without the "./" to run the program.)

# Project description

