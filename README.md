## BUILDING A HACKER NEWS PIPELINE

### OVERVIEW

In this guided project, we will build a pipeline and apply it to a real world data pipeline project. From a JSON API, we will filter, clean, aggregate, and summarize data in a sequence of tasks that will apply these transformations for us.

The data we will use comes from a Hacker News (HN) API that returns JSON data of the top stories in 2014. If you're unfamiliar with Hacker News, it's a link aggregator website that users vote up stories that are interesting to the community. It is similar to Reddit, but the community only revolves around on computer science and entrepreneurship posts.

The JSON file contains a single key stories, which contains a list of stories (posts). Each post has a set of keys, but we will deal only with the following keys:

    created_at: A timestamp of the story's creation time.
    created_at_i: A unix epoch timestamp.
    url: The URL of the story link.
    objectID: The ID of the story.
    author: The story's author (username on HN).
    points: The number of upvotes the story had.
    title: The headline of the post.

    num_comments: The number of a comments a post has.
    
### AIM
Using this dataset, we will run a sequence of basic natural language processing tasks using our Pipeline class. The goal will be to find the top 100 keywords of Hacker News posts in 2014. Because Hacker News is the most popular technology social media site, this will give us an understanding of the most talked about tech topics in 2014!

