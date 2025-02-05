## Challenge name: Guessing & Predicting Patterns

**Challenge Description:**
View Your Own Profile Another Way
The application we are working with seems to follow a RESTful pattern so far as the profile goes. Many apps have roles in which an elevated user may access content of another. In that case, just /profile won’t work since the own user’s session/authentication data won’t tell us whose profile they want view. So, what do you think is a likely pattern to view your own profile explicitly using a direct object reference?

**My Solution**
- This challenge is quite easy, remember the `userId` in challenge 1? It was `2342384`, just try the methods in the Examples section on page 1
- The correct answer is: `WebGoat/IDOR/profile/2342384`

[Next challenge](chall-3-1.md)
[Back to list](/README.md)