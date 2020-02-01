"# MoviesAPI" 

Following Use cases are possible in this API.

###### Register the user:
http POST http://127.0.0.1:8000/register email=test@gmail.com username=test password=password password2=password

###### Login and get the authentication token:
http POST http://127.0.0.1:8000/login username=test@gmail.com password=password

###### Set the Faviourte Genre:
http POST http://127.0.0.1:8000/set-genere "Authorization: Token `Token Number`" genre=Thriller

###### Get the recommended movies based on the set genre:
http GET http://127.0.0.1:8000/recommended "Authorization: Token `Token Number`"

###### Get the top rated movie:
http GET http://127.0.0.1:8000/top-rated "Authorization: Token `Token Number`"
  
###### Up vote or Down vote a movie using up or down options:
http POST http://127.0.0.1:8000/vote "Authorization: Token `Token Number`" movie=Jumanji vote=up

###### Write a review:
http POST http://127.0.0.1:8000/review "Authorization: Token `Token Number`" movie="The Well" review="Awesome Movie" rating=8

###### Get the Review and Rating of the Movie:
http GET http://127.0.0.1:8000/movie "Authorization: Token `Token Number`" movie="The Well"



