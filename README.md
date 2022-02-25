# Exploring Hacker News Posts

In this project, we worked with a dataset of submissions to popular technology site Hacker News. 

Hacker News is a site started by the startup incubator Y Combinator, where user-submitted stories (known as "posts") receive votes and comments, similar to reddit. Hacker News is extremely popular in technology and startup circles, and posts that make it to the top of the Hacker News listings can get hundreds of thousands of visitors as a result.

You can find the data set [here](https://www.kaggle.com/hacker-news/hacker-news-posts), but we have reduced from almost 300,000 rows to approximately 20,000 rows by removing all submissions that didn't receive any comments and then randomly sampling from the remaining submissions. Below are descriptions of the columns:
- `id`: the unique identifier from Hacker News for the post
- `title`: the title of the post
- `url`: the URL that the posts links to, if the post has a URL
- `num_points`: the number of points the post acquired, calculated as the total number of upvotes minus the total number of downvotes
- `num_comments`: the number of comments on the post
- `author`: the username of the person who submitted the post
- `created_at`: the date and time of the post's submission

We're specifically interested in posts with titles that begin with either `Ask HN` or `Show HN`. Users submit `Ask HN` posts to ask the Hacker News community a specific question. Below are a few examples:

```
  Ask HN: How to improve my personal website?
  Ask HN: Am I the only one outraged by Twitter shutting down share counts?
  Ask HN: Aby recent changes to CSS that broke mobile?
```
Likewise, users submit Show `HN` posts to show the Hacker News community a project, product, or just something interesting. Below are a few examples:

```
  Show HN: Wio Link  ESP8266 Based Web of Things Hardware Development Platform'
  Show HN: Something pointless I made
  Show HN: Shanhu.io, a programming playground powered by e8vm
```

The final aim is to answer the following questions based on solid analytical proofs:
```
- Do Ask HN or Show HN receive more comments on average?
- Do posts created at a certain time receive more comments on average?
```
