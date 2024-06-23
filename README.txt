
this is a very rough solution asked by Anaconda for the problem referenced below
https://jimmont.github.io/anaconda/

to use it I served the index over http with this Deno script (but any http service will do):
PORT=8080 && deno run --allow-read=./ --allow-net=localhost:$PORT https://raw.githubusercontent.com/sourdough/starter/main/tools/http.js --port=$PORT --index=index.html --www=./

- it's very crude, just click start and take turns selecting
- or reset the game
- there is a bug for auto-play when user is 'computer'
- the solution could be substantially improved, though I have never had an interest in games so tend to think it would be worth looking at how games work and are designed (as in architecture) a little to improve the approach with better separation of concerns which got fairly mixed with this ad-hoc naive approach
- and obviously the aesthetics here are nonexistent, from where the web began
- see the rock, papger, scissors problem statement in the lower index, toward the bottom of that page

