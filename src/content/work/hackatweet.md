---
title: Hackatweet
publishDate: 2023-01-01 00:00:00
img: /assets/stock-3.jpg
img_alt: Page d'accueil du site internet hackatweet
description: |

tags:
  - React
  - Twitter
  - SPA
---

##### <a href="https://hackatweet-frontend-two.vercel.app">Link to website</a>

<br>

#### Intro

Creating a Single Page Application (SPA) based on Twitter.

Handling the entire frontend and backend development.

Implementing Test-Driven Development (TDD) for some features, such as input field validation.

#### Login

The login page allows you to either create an account or log in to the application.

Clicking the "Sign up" or "Sign in" buttons opens a modal with input fields corresponding to the selected action.

In the case of a "Sign in," clicking the button within the modal triggers communication with the backend, and if the information is correct, the user is redirected to the home page.

For a "Sign up," the user's information is stored in the database.

This process involves the use of a token and password hashing for security.

#### Homepage

The home page is divided into three sections:

1. The left section displays a logo that also functions as a button to return to this page, user information, and a logout button.

2. The middle section is used for adding a tweet and viewing the timeline of tweets made by all users.

3. Finally, the right section displays "Trends," which includes all the hashtags that have been used and the number of times they have been used.

#### Tweets

Restricting tweet length to 280 characters.

If a tweet belongs to the logged-in user, he can like and delete it but if the tweet does not belong to the user, he can only like it.

The hashtag page is displayed when a user clicks on one of the hashtags in the Trends section. This action redirects to a customized URL that includes the page name and the hashtag name (e.g., /hashtag/hello for #hello).

The search bar allows users to search for other hashtags, and with each search, the URL updates. If no tweets contain the searched hashtag, a message "No tweets found with #hashtagname" is displayed.

Clicking on the logo takes the user back to the home page.