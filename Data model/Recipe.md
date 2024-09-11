Perhaps recipe extends [[Ingredient]], or they both extend some common property (We need to be able to use recipes as ingredients)
A recipe has properties:
- [[User]]
- createdOn: DateTime
- updatedOn: DateTime
-  set of [[instructionIngredient]]
- Prep Time: Time (minutes)
- Cook Time: Time (minutes)
- ordered sequence of [[section]] 
- countryOfOrigin: Option ([[Country]])
- cuisine: Option ([[Cuisine]])
- Vegetarian: Boolean
- Vegan: Boolean
- wikiLink: Option (Link)
- tags: List (tags), users can create custom tags 