# Yts

YTS api wrapper limited to movies and subtitles search.

## Installation

Add this line to your application's Gemfile:

```
gem 'yts', :git => 'https://github.com/kartouch/yts.git'
```

And then execute:

    $ bundle

## Usage

List movies:<br>
https://ytsto.xyz/#list_movies

    $ Yts.list_movies(params)
    $ Yts.list_movies('quality=3D','limit=10')

Movie details:<br>
https://ytsto.xyz/api#movie_details

    $Yts.movie_details(movie_id)
    $Yts.movie_details(movie_id).title
    
Movie suggestions:<br>
https://ytsto.xyz/api#movie_suggestions

    $Yts.movie_suggestions(movie_id)

Movie comments:<br>
https://ytsto.xyz/api#movie_comments

    $Yts.movie_comments(movie_id)
    
Movie reviews:<br>
https://ytsto.xyz/api#movie_reviews

    $Yts.movie_reviews(movie_id)

Movie parental guides:
https://ytsto.xyz/api#movie_parental_guides

    $Yts.movie_parental_guides(movie_id)
    
Subtitle search:
    
    $Yts.find_subtitles(imdb,lang)
    
## Contributing

1. Fork it ( https://github.com/kartouch/yts/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
