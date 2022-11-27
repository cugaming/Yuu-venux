# venux script
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Venux", "Ocean")

--Aim
local Aim = Window:NewTab("Aim")
local Aimsection = main:NewSection("Aim")

AimSection:NewButton("owl hub", "has aimbot soft aim and esp", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/CriShoux/OwlHub/master/OwlHub.txt"))()
end)

AimSection:NewButton("general aimbot", "aimbot ETC.", function()
    loadstring(game:HttpGet("https://pastebin.com/raw/CwQcEnEd"))()
end)

AimSection:NewButton("silent aim", "the bullets aim for you", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Averiias/Universal-SilentAim/main/main.lua"))()
end)

--Movement hacks
local Player = Window:NewTab("Movement")
local Playersection = main:NewSection("Movement")

PlayerSection:NewSlider("walk speed", "become speed", 500, 16, function(s) -- 500 (MaxValue) | 16 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

PlayerSection:NewSlider("Jump power", "jump to the roof", 350, 50, function(s) -- 350 (MaxValue) | 50 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)
