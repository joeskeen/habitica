# Deviations from the upstream Habitica source or instructions

* Had to increase number of allowed filesystem watchers: <https://stackoverflow.com/a/34664097/1396477>
* Instead of running three separate terminals, once everything was set up switched to a single terminal with a single command: `npx concurrently -n mongo,server,watch "npm run mongo:dev" "npm start" "npm run client:dev"`

