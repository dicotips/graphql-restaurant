# graphql-restaurant

In this assignment I created a Graphql localhost using NodeJs. Following are the mutations and queries to GraphQL.


```JSON
mutation editrestaurants($idd: Int = 1, $name: String = "OLDO") {
  editrestaurant(id: $idd, name: $name) { 
    name 
    description
  } 
}
```

```JSON
mutation setrestaurants { 
  setrestaurant(input: { 
    name: "Granite", 
    description: "American",
  }) { 
    name
    description
  } 
}
```

```JSON
mutation deleterestaurants($iid: Int = 1) {
  deleterestaurant(id: $iid) { ok }
}
```

```JSON
query getrestaurants { 
  restaurants {
    name
    description
    dishes {
      name
      price
    }
  } 
} 
```

```JSON
query getrestaurant($iid: Int = 1) { 
  restaurant(id: $iid) { 
    name
    description
  }
}
```

<img src="img/graphql%20restaurant%20-%20jheser%20guzman.png" width="350" title="hover text">