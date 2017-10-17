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

