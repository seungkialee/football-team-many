# football-team-many

# Objectives
Build RESTful actions for index, show, new, create, edit, update, delete
Use form_for for all forms
Correctly redirect when needed
Interlink between pages using link_to

# Instructions:
Make sure that a Fan's show page will show the list of all team that fan is a fan of.
Make sure that a Football Team's page will show a list of all the fans.

You should be able to add/remove a new fan to a football team.

## The models that you need:

  ##  * Football_Team

  ##  * Club

  ##  * Fan

The data relationship will look something like this:

## A Football_Team has many fans through a club 

## A Fan can like many teams through a club

## A Club belongs to a Football_Team and Fans

Your database should look like the following:


```db
table "Football_Teams"
  string "team_name"
  string "city"

table "Fans"
  string   "name"
  integer   "age"
 
table "Clubs"
  integer "football_team_id"
  integer "fan_id"
```

Make sure the app has the following components:

index, show, new, create, edit, update 
2. Use form_for for all forms 
3. Correctly redirect when needed 
4. Interlink between pages using link_to

You can use the resource, model, migration, and controller generators, but do not use the scaffold generator
