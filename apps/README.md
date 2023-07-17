Hello, Below are my own 3 suggested improvements for the url shortener codebase.

1. Expand current unit tests, and include property base testing.
   As it is, I believe the tests' focus is narrow. More unit tests as well as PBT would allow this a wider net to catch bugs.
2. include url input validation (and test accordingly). 
3. Prevent url duplication. Users, can theoretically enter the same URL an infinite amount. Itd be useful to save us some space by disallowing this.

My changes:
- I refactored several client components into a components folder
- I added a simple regex validation on the url input form using the input pattern attribute
  * itd definitely be safer to validate on the server-side (or better yet, both sides), but I wanted to just provide a demo
    
