# gitpizza

Base repository for the git & pizza evening game

## Instructions phase 1

Each participant creates a branch and
1. Creates and checks out a local branch with name `<username>-gitpizza`
1. Makes a commit adding theirselves to the `participants.json` file (1)
1. Makes a commit with their pizza choice to `pizza.json` file. Use `order` property (2)
1. Makes a commit with their drink choice to `drinks.json` file. Use `order` property (2)
1. Pushes the branch to the repository

## Instructions phase 2

Merge participant choices collaboratively

1. "Play off of merges"
1. Create integration branch for each "matchup"
1. Merge participant changes
1. Add a commit with totals for drinks and pizza (2)
1. Push integration branch
1. Repeat until the final is completed
1. Create PR with final results


## JSON file formats

(1) Format for `participants.json` file: dictionary of nickname - fullname

```
{
  "john": "John Doe"
}
```

(2) Format for `pizza.json` / `drinks.json` file:
```
{
  "choices":[
    "margherita",
    "marinara",
    "quattro stagioni",
    "carbonara"
  ],
  "totals": {
    "carbonara": 1
    "marinara": 2
  },
  "order": {
    "peter": "marinara",
    "paul": "marinara",
    "mary": "carbonara"
  }
}
```

