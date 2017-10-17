# Numbers API Challenge

### API Base URI

http://numbers-api.herokuapp.com/

### Usage

This API accepts form encoded params and returns a JSON payload

### Endpoints

```GET '/'```

```GET '/counters'```

_Displays a random list of all counters 1..1000_

```GET '/counters/:id'```

_Show for a specific counter_

```PUT '/counters/:id'```

_Update a counter accepts params ```[counter][count_by]```_

count_by can be a positive or negative value.

### Release 0

#### Update state with live data

Use ```fetch || axios``` to make a request to the server.

Update the state of your counters to reflect this data.

If you haven't used AXIOS before heres a quick [walk through](https://daveceddia.com/ajax-requests-in-react/).

You'll want to make use of Reacts component life-cycle method ```componentDidMount``` for making this call.

### Release 1

#### Update server as counters change

Each time a user clicks a counter your app should send a put request off to the API and update accordingly.

```PUT '/counters/:id'``` accepting nested attributes as ```counter[count_by]```. The count by value can be positive or negative number

Be sure to reset your counter state after the ```PUT``` resolves so that the data the user sees is always in line with your source of truth, the server data.
