# Potal

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.0.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

##
# Front-end OMDb assessment
Search the OMDb API

### Archived Content Follows

## Task Details
- Consume the [OMDb API](http://www.omdbapi.com/) to fetch the top 10 results matching your search query (JSON).
- Create an interface with at least one input field to be used to search for movies by title.
- Present the results in real time and update the interface as the user types his search query.
- Once the results are displayed allow the user to click on any particular movie to view its details.
- On the movie details view display more information.


## OMDb API Examples
OMDb API does not require any form of authentication. See the [OMDb API documentation](http://www.omdbapi.com/#parameters) for all supported parameters.

### Search by query

```
http://www.omdbapi.com/?s=ghost //results 1-10
http://www.omdbapi.com/?s=ghost&page=2 //  results 11-20
```
- Returns the first 10 results based on the query value provided as `s`
- Pagination can be added via `&page=n`, where `n` is 1-100

#### Movie Object Structure
```json
{
    "Title": "Mission: Impossible - Ghost Protocol",
    "Year": "2011",
    "imdbID": "tt1229238",
    "Type": "movie",
    "Poster": "https://images-na.ssl-images-amazon.com/images/M/MV5BMTY4MTUxMjQ5OV5BMl5BanBnXkFtZTcwNTUyMzg5Ng@@._V1_SX300.jpg"
}
```

### View movie details by `imdbID`
```
http://www.omdbapi.com/?i=tt1229238
```
- Using the `imdbID` provided by the search results will let you fetch the details of a particular movie.

##
![Screenshot (313)](https://user-images.githubusercontent.com/36602031/125169442-ca144680-e1c7-11eb-85ae-dd2d9cbd2df0.png)
