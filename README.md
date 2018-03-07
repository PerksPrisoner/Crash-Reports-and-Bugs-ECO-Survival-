# Crash-Reports-and-Bugs-ECO-Survival-
Depository of issues to consist of crash reports and bugs with Eco Survival (Steam Edition)
As of update 03/16/2018 Update 7.2

And exception is created when using a broken hammer on a cart that has an inventory in this case miscellaneous to include Tier 2 Lumber
that has entered the "Carrying Slot" then attempting to break the cart and still having inventory.

Caught exception:

<size=60.00%>Caught exception invoking RPC PlayerInteract on Player!

Object reference not set to an instance of an object.


Stack:
   at Eco.Gameplay.Items.Inventory.MoveAsManyItemsAsPossible(Inventory destination, Func`2 sourceStackPredicate, User user)
   at Eco.Gameplay.Components.StorageComponent.OnActLeft(InteractionContext context)
   at Eco.Gameplay.Interactions.InteractionExtensions.ExecuteUntilSuccess(IEnumerable`1 results)
   at Eco.Gameplay.Interactions.InteractionExtensions.ExecuteUntilSuccess(IEnumerable`1 results)
   at Eco.Gameplay.Players.Player.PlayerInteract(InteractionInfo info)



Stack:
   at Eco.Shared.Networking.RPCManager.TryInvoke(Object controller, String methodname, BSONObject bsonArgs, Object& result)
   at Eco.Shared.Networking.RPCManager.InvokeOn(BSONObject bson, Object controller, String methodname)
   at Eco.Shared.Networking.RPCManager.HandleReceiveRPC(INetClient client, BSONObject bson)
   at Eco.Shared.Networking.NetPort.ProcessBuffer()
   at Eco.Shared.Networking.NetPort.Update()
   at Eco.Plugins.Networking.Clients.Client.<.ctor>b__56_0()
</size>
