
local Test = Instance.new("ScreenGui")
local FrameMenu = Instance.new("Frame")
local namescript = Instance.new("TextLabel")
local Magma = Instance.new("TextButton")
local Light = Instance.new("TextButton")
local comingsoon = Instance.new("TextButton")


Test.Name = "Test"
Test.Parent = game.CoreGui

FrameMenu.Name = "Frame Menu"
FrameMenu.Parent = Test
FrameMenu.BackgroundColor3 = Color3.fromRGB(34, 34, 34)
FrameMenu.Position = UDim2.new(0.732198119, 0, 0.430674851, 0)
FrameMenu.Size = UDim2.new(0, 230, 0, 300)

namescript.Name = "name script"
namescript.Parent = FrameMenu
namescript.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
namescript.Position = UDim2.new(0.0652173907, 0, 0.0289855078, 0)
namescript.Size = UDim2.new(0, 200, 0, 50)
namescript.Font = Enum.Font.ArialBold
namescript.Text = "Script test By Pae23221"
namescript.TextColor3 = Color3.fromRGB(0, 0, 0)
namescript.TextSize = 14.000
namescript.TextWrapped = true

Magma.Name = "Magma"
Magma.Parent = FrameMenu
Magma.BackgroundColor3 = Color3.fromRGB(67, 26, 26)
Magma.Position = UDim2.new(0.0652173907, 0, 0.253623188, 0)
Magma.Size = UDim2.new(0, 200, 0, 50)
Magma.Font = Enum.Font.Code
Magma.Text = "Magma"
Magma.TextColor3 = Color3.fromRGB(255, 0, 0)
Magma.TextSize = 20.000
Magma.MouseButton1Down:connect(function()
	local plr = game:GetService("Players").LocalPlayer
	plr.Character.Powers.Magma.RemoteEvent:FireServer("MagmaPower1","StopCharging",plr.Character.HumanoidRootPart.CFrame,workspace.IslandSnowyMountains.Stone.Stone,100)
end)

Light.Name = "Light"
Light.Parent = FrameMenu
Light.BackgroundColor3 = Color3.fromRGB(202, 185, 0)
Light.Position = UDim2.new(0.0652173907, 0, 0.469420314, 0)
Light.Size = UDim2.new(0, 200, 0, 50)
Light.Font = Enum.Font.Bodoni
Light.Text = "Light"
Light.TextColor3 = Color3.fromRGB(255, 255, 0)
Light.TextSize = 20.000
Light.MouseButton1Down:connect(function()
	local plr = game:GetService("Players").LocalPlayer
	plr.Character.Powers.Light.RemoteEvent:FireServer("LightPower2","StopCharging",plr.Character.HumanoidRootPart.CFrame,workspace.IslandSnowyMountains.Stone.Stone,100)
end)

comingsoon.Name = "coming soon"
comingsoon.Parent = FrameMenu
comingsoon.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
comingsoon.Position = UDim2.new(0.0652173907, 0, 0.697681189, 0)
comingsoon.Size = UDim2.new(0, 200, 0, 50)
comingsoon.Font = Enum.Font.SourceSans
comingsoon.Text = "Coming soon"
comingsoon.TextColor3 = Color3.fromRGB(0, 0, 0)
comingsoon.TextSize = 25.000
