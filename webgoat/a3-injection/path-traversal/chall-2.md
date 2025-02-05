## Challenge name: Path traversal while uploading files

**Challenge Description:**
The developer became aware of the vulnerability and implemented a fix that removed the ../ from the input. Again the same assignment, but can you bypass the implemented fix?

**My Solution**
- As described, it is definitely not possible to use the previous method because the server will find and delete the string `../`
- But there is still a way to bypass it, by using the string `....//`, the server will find and remove the `../` in the middle and we will still have a complete string `../`. Submit it and complete the challenge.