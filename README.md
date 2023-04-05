Autp famr : 
if _G.wl_key then
    return
end
getgenv().Team = "Pirates"
--Do not execute any scripts before running the script
--Put Your Key Between "" at the _G.wl_key
_G.wl_key = "b3a7dae7cb0c92182e5de1d3d2849fa829e49205"
repeat wait()
until game:IsLoaded()
delay(DelayTime or 300,function()
    local CG = game:GetService("CoreGui")
    if not CG:FindFirstChild("W-azure") then
       game:GetService("TeleportService"):Teleport(game.PlaceId, game.Players.LocalPlayer)
    end
end)
wait(2)
loadstring(game:HttpGet('https://scripts.luawl.com/hosted/1989/Main-rewrite.lua'))()
