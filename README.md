# Ordinals Collections
#### A place for creators &amp; builders to organize ordinal collections!

## Getting Started
***Artists***
Collection creators can format their collection data using the `inscription.json` and `meta.json` format below to be listed on all platforms using the standard! 

All you need to do is create a list of all inscriptions in the format provided below.

***Developers***

1. Add to the registry by creating a pull request including new collections that follow the standard
2. Use the registry to include all ordinal collections on your site!


## File Structure
```
 .
 ├── ...
 └── collection-name            
     ├── inscriptions.json      
     └── meta.json              
```

## Collection Metadata `meta.json`
```
{
  "name": "",                    # inscription name
  "inscription_icon": "",        # collection cover inscription id
  "supply": "",                  # total supply
  "slug": "",                    # directory name
  "description": "",             # collection description
  "twitter_link": "",            # official twitter
  "discord_link": "",            # official discord
  "website_link": ""             # official website
}
```

## Inscription Data `inscriptions.json`
```
[
  {
    "id": "",                    # inscription id
    "meta": { 
      "name": ""                 # inscription name
    }
  },
  ...
]
```

## Expanding Inscription Data
Collections can be organized using `status` and `rank`
```
[
  {
    "id": "",
    "meta": {
      "name": "",
      "status": "",               # inscription theme
      "rank":                     # inscription rarity rank
    }
  },
  ...
]
```
Artists can assign unqiue traits to ordinals with `attributes`
```
[
  {
    "id": "",
    "meta": {
      "status": "",
      "rank": ,
      "name": ""
      "attributes": [
        {
          "trait_type": "",        # trait category
          "value": "",             # trait value
          "status": "",            # trait theme
          "percent": ""            # percent of inscriptions in collection with trait
        },
        ...
      ]
    }
  },
  ...
]
```
***Here is an example of a completed collection inscription***

