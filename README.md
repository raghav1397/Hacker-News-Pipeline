# Hacker News Pipeline

we will use the pipeline we have been building, and apply it to a real world data pipeline project. From a JSON API, we will filter, clean, aggregate, and summarize data in a sequence of tasks that will apply these transformations for us.

The data we will use comes from a Hacker News (HN) API that returns JSON data of the top stories in 2014. If you're unfamiliar with Hacker News, it's a link aggregator website that users vote up stories that are interesting to the community. It is similar to Reddit, but the community only revolves around on computer science and entrepreneurship posts.

screenshot of hacker news

To make things easier, we have already downloaded a list of JSON posts to a file called hn_stories_2014.json. The JSON file contains a single key stories, which contains a list of stories (posts). Each post has a set of keys, but we will deal only with the following keys:

    created_at: A timestamp of the story's creation time.
    created_at_i: A unix epoch timestamp.
    url: The URL of the story link.
    objectID: The ID of the story.
    author: The story's author (username on HN).
    points: The number of upvotes the story had.
    title: The headline of the post.
    num_comments: The number of a comments a post has.
