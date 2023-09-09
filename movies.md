class Movie {
    constructor(title, studio, rating) {
      this.title = title;
      this.studio = studio;
      this.rating = rating;
    }
  
    getrating() {
      console.log("the rating is  " + this.rating);
    };
  }
   
  class movie {
      constructor(title, studio, _rating){
          this.title = title;
          this.studio = studio;
          this.rating = "PG";
      }
  }

  const Movies = new Movie( "Casino Royal", "Eon Productions", "PG13");  
  console.log(Movies);
  Movies.getrating();
