local Material = loadstring(game:HttpGet("https://raw.githubusercontent.com/mrx156/f/main/55"))()
getgenv().KillAura = nil
getgenv().ChestFarm = nil
local X = Material.Load({
	Title = "Project XXL | Lazzy Exploits",
	Style = 2,
	SizeX = 250,
	SizeY = 150,
	Theme = "Light",
	ColorOverrides = {
		MainFrame = Color3.fromRGB(235,235,235)
	}
})

local Y = X.New({
	Title = "Roblox Main Scripts"
})



local B = Y.Toggle({
	Text = "Roblox | Kill Aura",
	Callback = function(Value)
		getgenv().KillAura = Value
	end,
	Enabled = false
})




while wait() do
    if getgenv().KillAura == true then

local args = {
    [1] = false,
    [2] = Vector3.new(6050.79931640625, -7155.2666015625, -5941.45849609375),
    [3] = CFrame.new(6050.79931640625, -7155.2666015625, -5941.45849609375) * CFrame.Angles(-0.8373390436172485, 0.027347246184945107, 0.030333522707223892),
    [4] = 1
}

game:GetService("ReplicatedStorage").RemoteEvents.MadaraSusanooRibcageRemote:FireServer(unpack(args))

  end
  end
