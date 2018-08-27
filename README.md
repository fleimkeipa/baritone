# Baritone
A Minecraft bot. This project is an updated version of [Minebot](https://github.com/leijurv/MineBot/),
the original version of the bot for Minecraft 1.8, rebuilt for 1.12.2.

# Setup
- Open the project in IntelliJ as a Gradle project
- Run the Gradle task `setupDecompWorkspace`
- Run the Gradle task `genIntellijRuns`
- Restart IntelliJ and import Gradle changes
- Select the "Minecraft Client" launch config and run

# Chat control
<a href="https://github.com/cabaletta/baritone/blob/master/src/main/java/baritone/utils/ExampleBaritoneControl.java">Defined here</a>

Quick start example: `thisway 1000` or `goal 70` to set the goal, `path` to actually start pathing. Also try `mine diamond_ore`. `cancel` to cancel.

# API example

```
Baritone.settings().allowSprint.value = true;
Baritone.settings().pathTimeoutMS.value = 2000L;

PathingBehavior.INSTANCE.setGoal(new GoalXZ(10000, 20000));
PathingBehavior.INSTANCE.path();
```