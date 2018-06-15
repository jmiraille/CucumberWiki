# |CrM B2B| Structures

```gherkin
Feature: |CrM B2B| Structures
Description: A loggedin user can manage and see their structures from the arenametrix website.

Background: User is logged in and have some structures created.
  Given I am a logged in user
  And   I have 5 structures
  And   I visit the structure management page

Scenario: An user can see all his structures
  Then I can see all my structures
  And  I can see each structure's informations

Scenario: An user can see details about one structure
  When I open a structure detail page
  Then I can see all informations for this structures
  And  I can see 5 first contacts belonging to this structure

Scenario: An user can edit details of a structure
  When I am on the structure detail page
  Then I can edit this structure's informations

Scenario: An user can add a new structure
  When I add a new structure
  Then I see my newly created structure on the management page
```
