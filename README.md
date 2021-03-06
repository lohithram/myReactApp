# React and Flux application to display Bill information from JSON data.

Run `npm install` in the directory to install React from npm. Then run:

    watchify -t babelify ./jsx/*.jsx ./js/*.js -o ./dist/bundle.js -v

to produce `bundle.js`. 

Now load index.html in any browser. Alternatively you can quickly look at the fiddle http://jsfiddle.net/lohithram/L5txxgkn/

Run 'npm test' in order to run unit tests.

### Notes

###### A good example of re-usable React Component in this app is BillList.jsx. Note that it accepts itemRenderer as a property and uses it to render individual items in the list.
###### BillDataStore loads the bill data by require'ing' BillService and when data is loaded, emits change event to notify interested parties.
###### I have produced basic unit tests for react components using Jest, which you can find under '__tests__' folder.
###### Didn't get to write unit tests for the Data Store and Actions. Happy to produce if requested.
###### You can see pre rendered output by loading 'Your Bill.html'. I have used Bootstrap css lightly to structure the information.
###### Again happy to format and improve the look of the bill information further.

