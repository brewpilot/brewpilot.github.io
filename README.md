# brewpilot.github.io
Website for BrewPilot, a platform for managing and optimizing brewing operations. Hosted on GitHub Pages. https://www.brewpilot.com

To run this site, do not open the index.html file in a browser. It will open it with the file:/// protocol. Instead, run a local server.

In a terminal:

```

cd brewpilot.github.io
python3 -m http.server

```

Running from a local server is reuired becuase the legal pages load pdf files via Javascript. Even though these are local files, browsers treat local files as if they are from an unknown origin, and so they trigger CORS errors. Running a local server sets all of the files to be from the same origin.