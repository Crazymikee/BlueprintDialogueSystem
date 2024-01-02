# BlueprintDialogueSystem
A dialogue system made in Unreal Engine 5.0 EA using blueprint, structured through data tables.

Example content is included which contains a level that holds an example speaker, player, dialogue tree, and events bound to dialogue choices.

The dialogue system is structured to receive "conversation modules" in which the dialogue component (which manages the dialogue data) generates a full conversation from the modules, recevied primarally from a data table.

The example conversation table can be found in this Data Table.
Content/DialogueExample/DT/Conversations/DT_Conv_Root.uasset

In the example dialogue, there are 3 conversation modules used to build the tree, Core, Small_Talk, LongConv1. By default in the example a conversation body (inside a module) that is marked as "Intro" will be used as the entry to the dialogue. The next conversation module "Small_Talk" has player response additions inserted into the "Intro" conversation body. When selecting this player response it will allow switching into the small talk module and bodies. The LongConv1 example module contains a longer form dialogue which also has event triggers in use which change various elements in the level.

Feel free to use this for anything, pick it apart, or just take a look, I made it primarally to see if scripting in UE5 was any different then scripting in UE4, and overall it is not really different at all, so this little project was a success for what I wanted to do. I did include a decent amount of comments and descriptions to hopefully assist whoever decides to look at the system, thanks!
