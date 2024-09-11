I think that the entity relationships are simple enough that we don't need to explicitly model them in db (like with a graph db), which means a PostgreSql will be fine, with standard schema that matches the data model

I feel like it may end up requiring more tables then I want, since the goal is to support very complicated searches
Well we know we need
- A user table that matches properties of user
- A recipe table
	- Can store most things directly
	- including sections since its all text, don't really need to support quick searches by them, that's what tags are for
	- InstructionIngredients is tricky:
		- I guess ingredients could be a list of lists, of ingredient ids (which may also be recipe ids) to another object of (unit, amount),