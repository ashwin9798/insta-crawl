<img src="https://s3-eu-central-1.amazonaws.com/centaur-wp/designweek/prod/content/uploads/2016/05/11170038/Instagram_Logo-1002x1003.jpg" width="200" align="right">

# Instagram-Profilecrawl

## Quickly crawl the information (e.g. followers, tags etc...) of an instagram profile. No login required!
Automation Script for crawling information from ones instagram profile.  
Like e.g. the number of posts, followers, and the tags of the the posts

#### Getting started
Just do:
```bash
git clone https://github.com/timgrossmann/instagram-profilecrawl.git
```

It uses selenium to get all the information so install it with:
```bash
pip install selenium
```

Install the proper `chromedriver` for your operating system.  Once you (download it)[https://sites.google.com/a/chromium.org/chromedriver/downloads] just drag and drop it into the `instagram-profilecrawl` directory.

## Use it!
Now you can start it using:
```bash
python3.5 crawl_profile.py username1 username2 ... usernameX
```

#### The information will be saved in a JSON-File in ./profiles/{username}.json.
> Example of a files data
```
{
  "alias": "Tim Gro\u00dfmann",
  "username": "grossertim",
  "num_of_posts": 127,
  "posts": [
    {
      "tags": ["#fun", "#good", "#goodday", "#goodlife", "#happy", "#goodtime", "#funny", ...],
      "comments": 12,
      "img": "https://scontent.cdninstagram.com/t51.2885-15/e15/p640x640/16585292_1355568261161749_3055111083476910080_n.jpg?ig_cache_key=MTQ0ODY3MjA3MTQyMDA3Njg4MA%3D%3D.2",
      "likes": 284
     },
     {
      "tags": ["#vegan", "#veganfood", "#vegansofig", "#veganfoodporn", "#vegansofig", ...],
      "comments": 6,
      "img": "https://scontent.cdninstagram.com/t51.2885-15/e35/16122741_405776919775271_8171424637851271168_n.jpg?ig_cache_key=MTQ0Nzk0Nzg2NDI2ODc5MTYzNw%3D%3D.2",
      "likes": 206
     },
     .
     .
     .
     ],
  "prof_img": "https://scontent.cdninstagram.com/t51.2885-19/s320x320/14564896_1313394225351599_6953533639699202048_a.jpg",
  "followers": 1950,
  "following": 310
}
```

#### With the help of [Wordcloud](https://github.com/amueller/word_cloud) you could do something like that with your used tags
![](http://i65.tinypic.com/2nkrrtg.png)

<hr />

###### Have Fun & Feel Free to report any issues
