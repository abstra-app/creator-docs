# Variable dropdown items

Let's say you want to make a form with dropdowns for state -> city selection.

This is a problem with fixed values in dropdowns, because the content of cities' dropdown depends on the selected state.

For this example, we will use a JSON file as API directly from GitHub containing Brazilian cities (Cidades) and States (Estados)

## Step 1: Setting up the connectors

Add a rest API with this base url:

`https://raw.githubusercontent.com/felipefdl/cidades-estados-brasil-json/master`

and following methods:

`GET /Estados.json`

`GET /Cidades.json`

``![](<../../.gitbook/assets/image (61) (2).png>)``![](<../../.gitbook/assets/image (63) (2).png>)``

``![](<../../.gitbook/assets/image (54) (1) (1).png>)``![](<../../.gitbook/assets/image (60) (1).png>)``

## Step 2: Adding variables

Add 3 variables:

* states: Array/List -> used for store the list of states
* cities: Array/List -> used for store the list of cities
* selectedState: Text -> used for store the id of selected state

![](<../../.gitbook/assets/image (53) (2).png>)![](<../../.gitbook/assets/image (48).png>)![](<../../.gitbook/assets/image (57) (1) (1).png>)![](<../../.gitbook/assets/image (56) (1) (1).png>)

## Step 3: Grabbing the list of states and cities

At the page start, you can add an action to fetch the states and cities list

![](<../../.gitbook/assets/image (66) (2).png>)![](<../../.gitbook/assets/image (49) (1).png>)![](<../../.gitbook/assets/image (59) (1).png>)![](<../../.gitbook/assets/image (52) (2).png>)![](<../../.gitbook/assets/image (58) (1).png>)

## Step 4: Configuring the dropdowns

![](<../../.gitbook/assets/image (55) (1).png>)![](<../../.gitbook/assets/image (62) (2).png>)![](<../../.gitbook/assets/image (47) (1).png>)

States dropdown -> variable

`selectedState`

States dropdown -> options

```typescript
$.states.map(state => ({
  value: state.ID,
  label: state.Nome
}))
```

Cities dropdown -> options

```javascript
$.cities.filter(city => city.Estado === $.selectedState).map(city => ({
  label: city.Nome,
  value: city.ID
}))
```
