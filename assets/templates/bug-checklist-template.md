# Bug-001 Checklist — 9 Lives

**Preconditions**
- Game build with fix applied
- Platform: Windows 10
- Input: Keyboard

**Test cases**

**Interactions**
- [ ] Menus and UI → works as expected
- [ ] Sounds → works as expected
- [ ] Music (On and Off) → works as expected

**Movement**
- [ ] Character walks left/right → works as expected
- [ ] Character jumps → works as expected
- [ ] Character dashes → works as expected in all directions EXCEPT up-right (bug-001)

**Attack**
- [ ] Character attacks → works as expected
- [ ] Character shoot enemies → works as expected
- [ ] Character takes damage when touched by enemy → works as expected
- [ ] Character takes damage when touched by enemy projectile → works as expected

**Defense**
- [ ] Collisions with enemies → works as expected
- [ ] Collisions with enemies projectiles → works as expected
- [ ] Collisions with walls → works as expected
      
**Progression**
- [ ] Character finish stages when touching heart → works as expected
- [ ] Character can collect Wool Balls → works as expected

**Life/ Death**
- [ ] Character dies and respawns from the beggining of the stage (checkpoint not acquired) → works as expected
- [ ] Character dies and respawns from last checkpoint (checkpoint acquired) → works as expected

**Notes**
- Confirm consistency across multiples tries
- Bug-001: Character cannot dash diagonally upward (already reported in Jira)
