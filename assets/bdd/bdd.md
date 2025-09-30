BDD — 9 Lives

  Scenario: Menus and UI interactions
    Given the game is running
    When the user interacts with the menu using the keyboard
    Then the menu options move up and down correctly
    And sounds are played as expected
    And music responds to On/Off settings

  Scenario: Movement
    Given the game is running
    When the character moves left or right
    Then the character walks correctly

    Given the game is running
    When the character jumps
    Then the jump occurs as expected

    Given the game is running
    When the character dashes in any direction
    Then the dash works as expected
    Except when dashing up-right (bug-001)

  Scenario: Attack
    Given the game is running
    When the character attacks
    Then the attack hits enemies as expected

    Given the game is running
    When the character touches an enemy or enemy projectile
    Then the character takes damage correctly

  Scenario: Defense
    Given the game is running
    When the character collides with enemies, projectiles, or walls
    Then collisions behave correctly

  Scenario: Progression
    Given the game is running
    When the character finishes a stage by touching the heart
    Then the stage completes as expected
    And Wool Balls can be collected

  Scenario: Life / Death
    Given the game is running
    When the character dies without a checkpoint
    Then the character respawns at the beginning of the stage

    Given the game is running
    When the character dies after reaching a checkpoint
    Then the character respawns at the last checkpoint
