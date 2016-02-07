# MyFavoriteMovies
“My Favorite Movies” is an iOS application that allows users to add and remove movies from a favorites list using TheMovieDB. Movies are displayed individually and in a list format.


Functionality: 

1. Users can log into TheMovieDB and obtain a session token which uses GET. 
2. Display the favourite movies which uses GET.
3. Add or remove the favourite movies which uses POST.

Configuring the Post Request:

let request = NSMutableURLRequest(URL: url) 

request.HTTPMethod = "POST" 

request.addValue("application/json", forHTTPHeaderField: "Accept")

request.addValue("application/json", forHTTPHeaderField: "Content-Type")

request.HTTPBody = "{\"media_type\": \"movie\",\"media_id\":550,\"favorite\":true}".dataUsingEncoding(NSUTF8StringEncoding)
