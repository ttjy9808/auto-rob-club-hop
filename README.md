task.wait(30)

local myScreenGui = Instance.new("ScreenGui")
myScreenGui.Name = "MyScreenGui"
myScreenGui.Parent = game.Players.LocalPlayer.PlayerGui


local myTextLabel = Instance.new("TextLabel")
myTextLabel.Name = "MyTextLabel"
myTextLabel.Parent = myScreenGui
myTextLabel.Size = UDim2.new(0, 200, 0, 50)
myTextLabel.Position = UDim2.new(0.5, -100, 0.5, -25)
myTextLabel.BackgroundTransparency = 1
myTextLabel.TextColor3 = Color3.fromRGB(0, 255, 0)
myTextLabel.Text = "AUTO ROB START"
myTextLabel.TextSize = 50


local blur = Instance.new("BlurEffect")
blur.Name = "MyBlurEffect"
blur.Size = 50
blur.Parent = game.Lighting


game:GetService("RunService").RenderStepped:connect(function()
    for _, cam in ipairs(workspace.Camera:GetChildren()) do
        if cam:IsA("Camera") then
            cam:WaitForChild("DepthOfField"):Destroy()
            blur.Parent = cam
        end
    end
end)


game:GetService("RunService").RenderStepped:connect(function()
    for _, cam in ipairs(workspace.Camera:GetChildren()) do
        if cam:IsA("Camera") then
            cam:WaitForChild("DepthOfField"):Destroy()
            blur.Parent = cam
        end
    end
end)

game:GetService("RunService").RenderStepped:connect(function()
    for _, cam in ipairs(workspace.Camera:GetChildren()) do
        if cam:IsA("Camera") then
            cam:WaitForChild("DepthOfField"):Destroy() 
            blur.Parent = cam
        end
    end
end)

wait(1)


local Noclip = nil
local Clip = nil

function noclip()
	Clip = false
	local function Nocl()
		if Clip == false and game.Players.LocalPlayer.Character ~= nil then
			for _,v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
				if v:IsA('BasePart') and v.CanCollide and v.Name ~= floatName then
					v.CanCollide = false
				end
			end
		end
		wait(0.21)
	end
	Noclip = game:GetService('RunService').Stepped:Connect(Nocl)
end

function clip()
	if Noclip then Noclip:Disconnect() end
	Clip = true
end

noclip()

wait(1)

local part = Instance.new("Part")
part.Name = "cell1"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4321.41,61.13,1126.43)
local part = Instance.new("Part")
part.Name = "cell2"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4318.9,61.13,1108.38)
local part = Instance.new("Part")
part.Name = "cell3"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4319.66,61.13,1088.87)
local part = Instance.new("Part")
part.Name = "cell4"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4309.31,61.13,1080.79)
local part = Instance.new("Part")
part.Name = "cell5"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4289.63,61.13,1082.93)
local part = Instance.new("Part")
part.Name = "cell6"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4271.86,61.13,1084.61)
local part = Instance.new("Part")
part.Name = "cell7"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4254.13,61.13,1086.65)
local part = Instance.new("Part")
part.Name = "cell8"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4236.96,61.13,1087.97)
local part = Instance.new("Part")
part.Name = "cell9"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4322.96,75.53,1127.09)
local part = Instance.new("Part")
part.Name = "cell10"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4318.9,75.53,1108.38)
local part = Instance.new("Part")
part.Name = "cell11"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4319.66,75.53,1088.87)
local part = Instance.new("Part")
part.Name = "cell12"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4309.31,75.53,1080.79)
local part = Instance.new("Part")
part.Name = "cell13"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4289.63,75.53,1082.93)
local part = Instance.new("Part")
part.Name = "cell14"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4271.79,75.53,1083.58)
local part = Instance.new("Part")
part.Name = "frontcell1"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4272.22,61.13,1117.63)
local part = Instance.new("Part")
part.Name = "frontcell2"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4272.22,75.53,1117.63)
local part = Instance.new("Part")
part.Name = "cell15"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4322.96,86.83,1127.09)
local part = Instance.new("Part")
part.Name = "cell16"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4318.9,86.83,1108.38)
local part = Instance.new("Part")
part.Name = "cell17"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4319.66,86.83,1088.87)
local part = Instance.new("Part")
part.Name = "cell18"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4309.31,86.83,1080.79)
local part = Instance.new("Part")
part.Name = "cell19"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4289.63,86.83,1082.93)
local part = Instance.new("Part")
part.Name = "cell20"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4271.79,86.83,1083.58)
local part = Instance.new("Part")
part.Name = "cell21"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4322.96,98.63,1127.09)
local part = Instance.new("Part")
part.Name = "cell22"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4318.9,98.63,1108.38)
local part = Instance.new("Part")
part.Name = "cell23"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4319.66,98.63,1088.87)
local part = Instance.new("Part")
part.Name = "cell24"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4309.31,98.63,1080.79)
local part = Instance.new("Part")
part.Name = "cell25"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4289.63,98.63,1082.93)
local part = Instance.new("Part")
part.Name = "cell26"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4271.79,98.63,1083.58)
local part = Instance.new("Part")
part.Name = "frontcell"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4272.22,98.63,1117.63)
task.wait(5)
local VirtualInputManager = game:GetService('VirtualInputManager')

function keyPress(Key, Press)
    VirtualInputManager:SendKeyEvent(Press, Key, false, game)
end
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell1" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
keyPress(Enum.KeyCode.Space, true)
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell2" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell3" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell4" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell5" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell6" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell7" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell8" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
keyPress(Enum.KeyCode.Space, false)
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell9" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell10" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell11" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell12" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell13" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell14" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell15" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell16" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell17" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell18" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell19" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell20" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell21" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell22" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell23" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell24" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell25" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "cell26" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "frontcell" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)


local LocalPlayer = game:GetService("Players").LocalPlayer
local Character = LocalPlayer.Character or LocalPlayer.CharacterAdded:Wait()
local Humanoid = nil

while not Humanoid do
    for i, v in pairs(Character:GetChildren()) do
        if v:IsA("Humanoid") then
            Humanoid = v
        end
    end
    task.wait()
end

local FakeHumanoid = Humanoid:Clone()

local ToSpoof = {
    WalkSpeed = FakeHumanoid.WalkSpeed,
    JumpPower = FakeHumanoid.JumpPower
}

local index, newindex, namecall; index = hookmetamethod(game, "__index", function(...)
    if not checkcaller() then
        local self, index = ...
        if self and index then
            if rawequal(self, Humanoid) and rawget(ToSpoof, index) then
                return rawget(ToSpoof, index)
            end
        end
    end
    
    return index(...)
end); newindex = hookmetamethod(game, "__newindex", function(...)
    if not checkcaller() then
        local self, index, value = ...
        if self and index then
            if rawequal(self, Humanoid) and rawget(ToSpoof, index) then
                rawset(ToSpoof, index, value)
                return
            end
        end
    end
    
    return newindex(...)
end); namecall = hookmetamethod(game, "__namecall", function(...)
    if not checkcaller() then
        local self, args, method = ..., {...}, getnamecallmethod(); table.remove(args, 1)
        if self and method then
            if rawequal(self, Humanoid) then
                if rawequal(method, "Clone") then
                    return namecall(FakeHumanoid, ...)
                elseif rawequal(method, "GetPropertyChangedSignal") and rawget(ToSpoof, rawget(args, 1)) then
                    rawset(args, 1, "ClassName")
                end
            end
        end
    end
    
    return namecall(...)
end)

for i, v in pairs(getconnections(Humanoid.Changed)) do
    if v and v.Function then
        local vFunc; vFunc = hookfunc(v.Function, function(...)
            if not checkcaller() then
                local args = {...}
                if rawget(ToSpoof, rawget(args, 1)) then
                    rawset(args, 1, "ClassName")
                end
            end
            
            return vFunc(...)
        end)
    end
end

Humanoid.WalkSpeed = 100

task.wait(1)


local char = game.Players.LocalPlayer.Character

local cPos = char.HumanoidRootPart.Position
local fPos = cPos.Z + 2

char.Humanoid:MoveTo(Vector3.new(-4320.17,61.13,1162.96))
task.wait(1.5)
char.Humanoid:MoveTo(Vector3.new(-4297,61.13,1247.97))
task.wait(1.8)
char.Humanoid:MoveTo(Vector3.new(-4326.89,61.13,1283.79))
task.wait(1)
local part = Instance.new("Part")
part.Name = "escape prison"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(-4386.95,100,1271.76)
task.wait(1.5)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "escape prison" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
char.Humanoid:MoveTo(Vector3.new(-4438.63,111.76,1158.66))
task.wait(3)
char.Humanoid:MoveTo(Vector3.new(-4399.05,21.01,815.5))
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(-3893.02,21.01,712.02))
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(-2755.63,20.73,44.2))
Humanoid.WalkSpeed = 300
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(-1696.28,19.66,189.81))
task.wait(4)
char.Humanoid:MoveTo(Vector3.new(-383.91,25.26,-351.14))
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(-182.57,25.26,-57.87))
task.wait(1)


Humanoid.WalkSpeed = 100

wait(1)
local char = game.Players.LocalPlayer.Character

local cPos = char.HumanoidRootPart.Position
local fPos = cPos.Z + 2

char.Humanoid:MoveTo(Vector3.new(56.66,25.25,-152.68))
task.wait(1)
char.Humanoid:MoveTo(Vector3.new(-176.59,25.26,-32.21))
task.wait(3)
char.Humanoid:MoveTo(Vector3.new(-648.72,21.57,-1191.24))
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(-648.72,21.57,-1191.24))
task.wait(6)
char.Humanoid:MoveTo(Vector3.new(-648.72,21.57,-1191.24))
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(456.75,16.05,-1126.51))
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(456.75,16.05,-1126.51))
task.wait(2)
char.Humanoid:MoveTo(Vector3.new(459.87,16.11,-1156.8))
task.wait(4)
char.Humanoid:MoveTo(Vector3.new(787.32,37.64,-1132.74))
task.wait(3)
char.Humanoid:MoveTo(Vector3.new(873.42,38.69,-1098.35))
task.wait(4)
char.Humanoid:MoveTo(Vector3.new(1396.89,45.01,-1059.35))
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(1484.65,44.89,-959.16))
task.wait(3)
char.Humanoid:MoveTo(Vector3.new(1408.73,73.03,-1154.57))
task.wait(3)
char.Humanoid:MoveTo(Vector3.new(1470.4,73.03,-1240.91))
task.wait(2)
char.Humanoid:MoveTo(Vector3.new(1696.74,73.73,-1229.09))
task.wait(2)
local part = Instance.new("Part")
part.Name = "club1"
part.CanCollide = true
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace
part.Position = Vector3.new(1696.74,241.91,-1229.09)
local part = Instance.new("Part")
part.Name = "club2"
part.CanCollide = false
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace 
part.Position = Vector3.new(1696.74,272,-1229.09)
local part = Instance.new("Part")
part.Name = "club3"
part.CanCollide = true
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace
part.Position = Vector3.new(1696.74,241.91,-1229.09)
local part = Instance.new("Part")
part.Name = "club4"
part.CanCollide = true
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace
part.Position = Vector3.new(1748.68,230,-1226.93)
local part = Instance.new("Part")
part.Name = "club5"
part.CanCollide = true
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace
part.Position = Vector3.new(1748.68,250,-1226.93)
local part = Instance.new("Part")
part.Name = "club6"
part.CanCollide = true
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace
part.Position = Vector3.new(1763.11,229.26,-1223.8)
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "club2" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(2)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "club5" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
char.Humanoid:MoveTo(Vector3.new(1793.76,225.42,-1222.06))
task.wait(1)
Humanoid.WalkSpeed = 20
task.wait(3)
char.Humanoid:MoveTo(Vector3.new(1795.28,221.42,-1196.98))
task.wait(2)
local part = Instance.new("Part")
part.Name = "club7"
part.CanCollide = true
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace
part.Position = Vector3.new(1795.28,192.62,-1196.98)
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "club7" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
char.Humanoid:MoveTo(Vector3.new(1827.35,192.62,-1157.92))
task.wait(5)
local part = Instance.new("Part")
part.Name = "club8"
part.CanCollide = true
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace
part.Position = Vector3.new(1827.35,225.42,-1157.92)
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "club8" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(2)
char.Humanoid:MoveTo(Vector3.new(1823.63,227.62,-1154.38))
task.wait(30)
char.Humanoid:MoveTo(Vector3.new(1820.92,225.42,-1164))
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "club7" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
Humanoid.WalkSpeed = 100
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "club7" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
local part = Instance.new("Part")
part.Name = "club9"
part.CanCollide = true
part.Anchored = true
part.Color = Color3.new(1, 1, 1)
part.Parent = workspace
part.Position = Vector3.new(1795.28,221.42,-1196.98)
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "club9" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
for i,v in pairs(workspace:GetChildren())do
if v:IsA("Part") and v.Name == "club6" then
game.workspace.fan_token345.HumanoidRootPart.CFrame = v.CFrame
end
end
task.wait(1)
char.Humanoid:MoveTo(Vector3.new(1546.95,73.03,-1237.45))
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(1546.95,73.03,-1237.45))
task.wait(3)
Humanoid.WalkSpeed = 100
task.wait(1)
char.Humanoid:MoveTo(Vector3.new(1338.37,38.69,-1241.04))
task.wait(2)
char.Humanoid:MoveTo(Vector3.new(1323.92,38.69,-1062.81))
task.wait(2)
Humanoid.WalkSpeed = 200
task.wait(1)
char.Humanoid:MoveTo(Vector3.new(300.3,12.69,-1096.8))
task.wait(5)
char.Humanoid:MoveTo(Vector3.new(-647.95,21.57,-1226.11))
task.wait(6)
char.Humanoid:MoveTo(Vector3.new(-180.38,25.26,-24.03))
task.wait(8)
char.Humanoid:MoveTo(Vector3.new(107.45,26.49,-180.01))
task.wait(10)
game:GetService("TeleportService"):Teleport(1224212277, game:GetService("Players").LocalPlayer)
