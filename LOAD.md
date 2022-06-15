local Library = loadstring(game:HttpGet("https://pastebin.com/raw/vff1bQ9F", true))() 

local Window = Library.CreateLib("vape hub", "Ocean")


local Tab1 = Window:NewTab("main")
local Tab1Section = Tab1:NewSection("main")


Tab1Section:NewButton("vape loader", "by 7granddad", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Error-virus/holy-arceus-x-working-vape-v4/main/vape%20v4%20fixed%20version.lua", true))()
end)

Tab1Section:NewToggle("infjump", "Fly", function(state)
    if state then
        local infjump = true
Ij = game:GetService("UserInputService").JumpRequest:connect(function()
    if infjump then
        game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
    end
end)
    else
        Ij:disconnect()
    end
end)

Tab1Section:NewButton("tpwalk 0.6", "gives you super speed", function()
local a=game.Players.LocalPlayer;spawn(function()while true do a.Character:TranslateBy(a.Character.Humanoid.MoveDirection*1.06)wait()end end)
end)

Tab1Section:NewButton("keyboard", "g", function()
    -- Gui to Lua
-- Version: 3.2

-- Instances:

loadstring(game:HttpGet(('https://raw.githubusercontent.com/manimcool21/Keyboard-FE/main/Protected%20(3).lua'),true))()
local KeyboardguiWarriorRoberrVersion = Instance.new("ScreenGui")
local Drag = Instance.new("Frame")
local Close = Instance.new("TextButton")

--Properties:

KeyboardguiWarriorRoberrVersion.Name = "Keyboard gui WarriorRoberr Version"
KeyboardguiWarriorRoberrVersion.Parent = game.CoreGui
KeyboardguiWarriorRoberrVersion.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Drag.Name = "Drag"
Drag.Parent = KeyboardguiWarriorRoberrVersion
Drag.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Drag.BorderSizePixel = 0
Drag.Position = UDim2.new(0.147916675, 0, 0.0593749993, 0)
Drag.Size = UDim2.new(0, 270, 0, 30)
Drag.Active = true
Drag.Draggable = true

Close.Name = "Close"
Close.Parent = Drag
Close.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Close.BorderSizePixel = 0
Close.Position = UDim2.new(0.999839723, 0, -0.00729167089, 0)
Close.Size = UDim2.new(0, 30, 0, 30)
Close.Font = Enum.Font.SourceSans
Close.Text = "X"
Close.TextColor3 = Color3.fromRGB(255, 255, 255)
Close.TextSize = 35.000
Close.MouseButton1Click:Connect(function()
	KeyboardguiWarriorRoberrVersion:Destroy()
end)
game.CoreGui["BUNB0yBUN BOARD"].KeyBoard.Parent = Drag
game.CoreGui["BUNB0yBUN BOARD"]:Destroy()
game.CoreGui["Keyboard gui WarriorRoberr Version"].Drag.KeyBoard.Bunb0ybun.Text = "MADE BY WARRIORROBERR BETTER VERSION "
game.CoreGui["Keyboard gui WarriorRoberr Version"].Drag.KeyBoard.Position = UDim2.new(0, 0, 0, 35)
game.CoreGui["Keyboard gui WarriorRoberr Version"].Drag.KeyBoard.Bunb0ybun.TextSize = 10
end)

Tab1Section:NewButton("vape cape", "hello", function()
local player = game:GetService("Players")

local lplr = player.LocalPlayer

if lplr.Character.Humanoid.RigType == Enum.HumanoidRigType.R15 then

      if lplr.Character:FindFirstChild("Torso") then

        torso = lplr.Character.Torso

      else

        torso = lplr.Character.UpperTorso

      end

      local CapeP = Instance.new("Part", torso.Parent)

      CapeP.Name = "Cape"

      CapeP.Anchored = false

      CapeP.CanCollide = false

      CapeP.TopSurface = 0

      CapeP.BottomSurface = 0

      CapeP.Color = Color3.fromRGB(0,0,0)

      CapeP.FormFactor = "Custom"

      CapeP.Size = Vector3.new(0.2,0.2,0.2)

      local decal = Instance.new("Decal", CapeP)

      decal.Texture = "http://www.roblox.com/asset/?id=9608953346"

      decal.Face = "Back"

      local msh = Instance.new("BlockMesh", CapeP)

      msh.Scale = Vector3.new(9,17.5,0.5)

      local motor = Instance.new("Motor", CapeP)

      motor.Part0 = CapeP

      motor.Part1 = torso

      motor.MaxVelocity = 0.01

      motor.C0 = CFrame.new(0,1.75,0) * CFrame.Angles(0,math.rad(90),0)

      motor.C1 = CFrame.new(0,1,0.45) * CFrame.Angles(0,math.rad(90),0)

      local wave = false

      repeat wait(1/44)

        decal.Transparency = torso.Transparency

        local ang = 0.1

        local oldmag = torso.Velocity.magnitude

        local mv = 0.002

        if wave then

          ang = ang + ((torso.Velocity.magnitude/10) * 0.05) + 0.05

          wave = false

        else

          wave = true

        end

        ang = ang + math.min(torso.Velocity.magnitude/11, 0.5)

        motor.MaxVelocity = math.min((torso.Velocity.magnitude/111), 0.04) + mv

        motor.DesiredAngle = -ang

        if motor.CurrentAngle < -0.2 and motor.DesiredAngle > -0.2 then

          motor.MaxVelocity = 0.04

        end

        repeat wait() until motor.CurrentAngle == motor.DesiredAngle or math.abs(torso.Velocity.magnitude - oldmag) >= (torso.Velocity.magnitude/10) + 1

        if torso.Velocity.magnitude < 0.1 then

          wait(0.1)

        end

      until not CapeP or CapeP.Parent ~= torso.Parent

    end


    print("...")
end)

Tab1Section:NewButton("reduce anticheat", "Reduced", function()
local player = game.Players.LocalPlayer
	repeat
		wait()
	until player:FindFirstChild("Backpack")
	local Connection = game.DescendantAdded:Connect(function(Inst)
		local Success, Error = pcall(function()
			return Inst.DisplayOrder
		end)
		if tostring(Inst) ~= "DevConsoleMaster" and tostring(Inst) ~= "InputCatcher" and Error == "The current identity (2) cannot Class security check (lacking permission 1)" then
			while true do
			end
		end
	end)
	local toSave = {}
	local function saveScript(saved)
		toSave[saved] = true
		local storedName = saved.Name
		saved:GetPropertyChangedSignal("Disabled"):connect(function()
			if saved.Disabled then
				local robloxlocked = pcall(function()
					saved.Disabled = false
				end)
				if not robloxlocked then
					while true do
					end
				end
			end
		end)
		saved:GetPropertyChangedSignal("Name"):connect(function()
			saved.Name = storedName
		end)
	end
	for _, v in pairs(script.Parent:GetChildren()) do
		if v:IsA("LocalScript") and (v.Name == "check" or v.Name == "checkDo") and v ~= script then
			saveScript(v)
		end
	end
	script.Parent.ChildRemoved:connect(function(child)
		if toSave[child] then
			local saved, cloned = pcall(function()
				return child:Clone()
			end)
			if saved then
				cloned.Parent = script.Parent
				saveScript(cloned)
			else
				while true do
				end
			end
		end
	end)
	local setUpCharacter = function(char)
		wait(5)
		for _, v in pairs(char:GetDescendants()) do
			if v:IsA("BasePart") and v:FindFirstChildOfClass("TouchTransmitter") then
				while true do
				end
			elseif v:IsA("BasePart") then
				v.ChildAdded:connect(function(child)
					if child:IsA("TouchTransmitter") then
						while true do
						end
					end
				end)
			end
		end
		char:WaitForChild("HumanoidRootPart"):GetPropertyChangedSignal("CFrame"):connect(function()
			while true do
			end
		end)
	end
	if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
		wait(5)
		setUpCharacter(player.Character)
	end
	player.CharacterAdded:connect(function(char)
		wait(5)
		setUpCharacter(char)
	end)
	player.Backpack.ChildAdded:Connect(function(added)
		local toolCount = 0
		for i, v in pairs(player.Backpack:GetChildren()) do
			if v:IsA("Tool") then
				toolCount = toolCount + 1
			end
		end
		for i, v in pairs(player.Character:GetChildren()) do
			if v:IsA("Tool") then
				toolCount = toolCount + 1
			end
		end
		for i, v in pairs(player:GetChildren()) do
			if v:IsA("Tool") then
				toolCount = toolCount + 1
			end
		end
		if toolCount > 2 then
			while true do
			end
		end
	end)
    print("By NTD")
end)

Tab1Section:NewButton("reduce anticheat 2", "anticheat reduced", function()
local player = game.Players.LocalPlayer local character = player.Character local humanoid = character:WaitForChild('Humanoid') local head = character:WaitForChild('Head') local base = game.Workspace.Baseplate local fall = false local value = nil local value2 = nil local value3 = nil humanoid.StateChanged:connect(function(state) 	if state == Enum.HumanoidStateType.Jumping then 	fall = true 	value = head.CFrame.Y - base.CFrame.Y 	elseif state == Enum.HumanoidStateType.Running or state == Enum.HumanoidStateType.RunningNoPhysics then 		value = head.CFrame.Y - base.CFrame.Y 	elseif state == Enum.HumanoidStateType.Freefall then 		fall = true 	elseif state == Enum.HumanoidStateType.Landed then 		if fall == true then 			value2 = head.CFrame.Y - base.CFrame.Y 			value3 = value - value2 			if value3 > 29 then 				fall = false 				value3 = nil 				humanoid:TakeDamage(30) 			
end 		
end 	
end 
end)
    print("...")
end)

Tab1Section:NewButton("reduce anticheat 3", "Hello", function()
local player = game.Players.LocalPlayer local character = player.Character local humanoid = character:WaitForChild('Humanoid') local head = character:WaitForChild('Head') local base = game.Workspace.Baseplate local fall = false local value = nil local value2 = nil local value3 = nil humanoid.StateChanged:connect(function(state) 	if state == Enum.HumanoidStateType.Jumping then 	fall = true 	value = head.CFrame.Y - base.CFrame.Y 	elseif state == Enum.HumanoidStateType.Running or state == Enum.HumanoidStateType.RunningNoPhysics then 		value = head.CFrame.Y - base.CFrame.Y 	elseif state == Enum.HumanoidStateType.Freefall then 		fall = true 	elseif state == Enum.HumanoidStateType.Landed then 		if fall == true then 			value2 = head.CFrame.Y - base.CFrame.Y 			value3 = value - value2 			if value3 > 29 then 				fall = false 				value3 = nil 				humanoid:TakeDamage(30) 			
end 		
end 	
end 
end)
    print("Reduced")
end)

Tab1Section:NewButton("full bright + no fog", "Full Bright", function()
game.Lighting.FogEnd = 1000000000000000000000000000000000000000
game.Lighting.FogStart = 0
game.Lighting.ClockTime = 14
game.Lighting.Brightness = 18
game.Lighting.GlobalShadows = false
    print("...")
end)

Tab1Section:NewButton("fps boost", "boost", function()
    local decalsyeeted = true -- Leaving this on makes games look shitty but the fps goes up by at least 20.
local g = game
local w = g.Workspace
local l = g.Lighting
local t = w.Terrain
t.WaterWaveSize = -100
t.WaterWaveSpeed = -100
t.WaterReflectance = -100
t.WaterTransparency = -100
l.GlobalShadows = false
l.FogEnd = 9e9999
l.Brightness = 18.8
settings().Rendering.QualityLevel = "Level01"
for i, v in pairs(g:GetDescendants()) do
    if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then
        v.Material = "Plastic"
        v.Reflectance = 0
    elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
        v.Transparency = 1
    elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
        v.Lifetime = NumberRange.new(0)
    elseif v:IsA("Explosion") then
        v.BlastPressure = 1
        v.BlastRadius = 1
    elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") then
        v.Enabled = false
    elseif v:IsA("MeshPart") then
        v.Material = "Plastic"
        v.Reflectance = 0
        v.TextureID = 10385902758728957
    end
end
for i, e in pairs(l:GetChildren()) do
    if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
        e.Enabled = false
    end
end
end)


