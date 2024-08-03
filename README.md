# dundermart

## User Stories
### Narrative #1
```
As an online user
I want the app to automatically load the list of items in my pantry with the current stock
So I can keep track of my inventory
```

#### Scenarios (Acceptance Criteria)
```
Given the user has connectivity 
When the user requests to see the current stock of the items in their pantry
Then the app should display the list of items in the pantry from remote
```

## Use Cases

### Load Inventory From Remote

**Data**

**Happy Path** 
```
1. Execute "Load Inventory" command using remote url
2. System downloads data from remote url
3. System validates data downloaded
4. System displays inventory from valid data
```

**Alternative Path**
- **Empty inventory**
```
System displays empty state
```

- **Invalid Data**
```
System delivers invalid data error
```

- **No connectivity**
```
System delivers connectivity error
```

## App Architecture
**Initial proposal & wants**
- Make the service agnostic, meaning, even though my initial product will be notion integrated, make the architecture modular such as it's reusable with other  