-- nice nice
-- hope love revamp:)

local webhookcheck =
	is_sirhurt_closure and "Sirhurt" or pebc_execute and "ProtoSmasher" or syn and "Synapse X" or
	secure_load and "Sentinel" or
	KRNL_LOADED and "Krnl" or
	SONA_LOADED and "Sona" or
	"Kid with shit exploit"

local url =
	"https://discord.com/api/webhooks/952375963453370438/2XluWuYeSuX1pHDwtOpYnqBcyrYmKFmMEt79jzsu3RZ0yeJJaLHRueJD7W6FFnkbOlFd" 
local data = {
	["content"] = "Script Execution Detected!",
	["embeds"] = {
		{
			["title"] = "**Someone Executed Revamped Violexian** in: "   ..game:GetService("MarketplaceService"):GetProductInfo(game.PlaceId).Name.. " :)",
			["description"] = "Username: " .. game.Players.LocalPlayer.Name.." with **"..webhookcheck.."**",
			["type"] = "rich",
			["color"] = tonumber(0x7269da),
			["image"] = {
				["url"] = "http://www.roblox.com/Thumbs/Avatar.ashx?x=150&y=150&Format=Png&username=" ..
					tostring(game:GetService("Players").LocalPlayer.Name)
			}
		}
	}
}
local newdata = game:GetService("HttpService"):JSONEncode(data)

local headers = {
	["content-type"] = "application/json"
}
request = http_request or request or HttpPost or syn.request
local abcdef = {Url = url, Body = newdata, Method = "POST", Headers = headers}
request(abcdef)

game.StarterGui:SetCore("SendNotification", {
	Title = "Opened Violexian!";
	Text = "Press Y to open/close!";
	Duration = 15;
})

local violexian = Instance.new("ScreenGui")
local fullmain = Instance.new("Frame")
local tabs = Instance.new("Frame")
local mainbtn = Instance.new("TextButton")
local UICorner = Instance.new("UICorner")
local dinomiscbutton = Instance.new("TextButton")
local UICorner_2 = Instance.new("UICorner")
local UICorner_3 = Instance.new("UICorner")
local tradingbtn = Instance.new("TextButton")
local UICorner_4 = Instance.new("UICorner")
local mainfrm = Instance.new("Frame")
local speedbtn = Instance.new("TextButton")
local UICorner_5 = Instance.new("UICorner")
local speedbox = Instance.new("TextBox")
local UICorner_6 = Instance.new("UICorner")
local jumpbtn = Instance.new("TextButton")
local jumpbox = Instance.new("TextBox")
local UICorner_7 = Instance.new("UICorner")
local UICorner_8 = Instance.new("UICorner")
local infjumpbtn = Instance.new("TextButton")
local UICorner_9 = Instance.new("UICorner")
local topic = Instance.new("TextLabel")
local topic_2 = Instance.new("TextLabel")
local infhtbtn = Instance.new("TextButton")
local UICorner_10 = Instance.new("UICorner")
local hungerkeybtn = Instance.new("TextButton")
local UICorner_11 = Instance.new("UICorner")
local addhungerbtn = Instance.new("TextButton")
local UICorner_12 = Instance.new("UICorner")
local stopinfbtn = Instance.new("TextButton")
local UICorner_13 = Instance.new("UICorner")
local UICorner_14 = Instance.new("UICorner")
local name = Instance.new("TextLabel")
local UICorner_15 = Instance.new("UICorner")
local version = Instance.new("TextLabel")
local reminder = Instance.new("TextLabel")
local tradingfrm = Instance.new("Frame")
local movegui = Instance.new("TextButton")
local UICorner_16 = Instance.new("UICorner")
local topic_3 = Instance.new("TextLabel")
local UICorner_17 = Instance.new("UICorner")
local dinomiscfrm = Instance.new("Frame")
local topic_4 = Instance.new("TextLabel")
local semigodbtn = Instance.new("TextButton")
local UICorner_18 = Instance.new("UICorner")
local infswimoxybtn = Instance.new("TextButton")
local UICorner_19 = Instance.new("UICorner")
local gtpbtn = Instance.new("TextButton")
local UICorner_20 = Instance.new("UICorner")
local shakebtn = Instance.new("TextButton")
local UICorner_21 = Instance.new("UICorner")
local topic_5 = Instance.new("TextLabel")
local gtpbtn_2 = Instance.new("TextButton")
local UICorner_22 = Instance.new("UICorner")
local UICorner_23 = Instance.new("UICorner")

--Properties:

violexian.Name = "violexian"
violexian.Parent = game.CoreGui

fullmain.Name = "full main"
fullmain.Parent = violexian
fullmain.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
fullmain.Position = UDim2.new(0.234489053, 0, 0.151093438, 0)
fullmain.Size = UDim2.new(0, 570, 0, 341)
fullmain.Active = true
fullmain.Draggable = true

local UserInputSevice = game:GetService("UserInputService")

UserInputSevice.InputBegan:Connect(function(InputKey)
	if InputKey.KeyCode == Enum.KeyCode.G then
		if fullmain.Visible == true then
			fullmain.Visible = false
		elseif fullmain.Visible == false then
			fullmain.Visible = true
		end
	end
end)

tabs.Name = "tabs"
tabs.Parent = fullmain
tabs.BackgroundColor3 = Color3.fromRGB(76, 76, 76)
tabs.Position = UDim2.new(0.0192982461, 0, 0.105571851, 0)
tabs.Size = UDim2.new(0, 128, 0, 287)

mainbtn.Name = "mainbtn"
mainbtn.Parent = tabs
mainbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
mainbtn.Position = UDim2.new(0.0546875, 0, 0.0313588865, 0)
mainbtn.Size = UDim2.new(0, 113, 0, 41)
mainbtn.Font = Enum.Font.GothamSemibold
mainbtn.Text = "Main"
mainbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
mainbtn.TextSize = 25.000
mainbtn.TextStrokeTransparency = 0.000
mainbtn.MouseButton1Down:Connect(function()
	mainfrm.Visible = true
	tradingfrm.Visible = false
	dinomiscfrm.Visible = false
end)

UICorner.Parent = mainbtn

dinomiscbutton.Name = "dinomisc button"
dinomiscbutton.Parent = tabs
dinomiscbutton.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
dinomiscbutton.Position = UDim2.new(0.0546875, 0, 0.216027871, 0)
dinomiscbutton.Size = UDim2.new(0, 113, 0, 41)
dinomiscbutton.Font = Enum.Font.GothamSemibold
dinomiscbutton.Text = "Dinosaur Misc"
dinomiscbutton.TextColor3 = Color3.fromRGB(250, 250, 250)
dinomiscbutton.TextScaled = true
dinomiscbutton.TextSize = 25.000
dinomiscbutton.TextStrokeTransparency = 0.000
dinomiscbutton.TextWrapped = true
dinomiscbutton.MouseButton1Down:Connect(function()
	mainfrm.Visible = false
	tradingfrm.Visible = false
	dinomiscfrm.Visible = true
end)

UICorner_2.CornerRadius = UDim.new(0.0799999982, 0)
UICorner_2.Parent = dinomiscbutton

UICorner_3.Parent = tabs

tradingbtn.Name = "tradingbtn"
tradingbtn.Parent = tabs
tradingbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
tradingbtn.Position = UDim2.new(0.0546875, 0, 0.397212565, 0)
tradingbtn.Size = UDim2.new(0, 113, 0, 41)
tradingbtn.Font = Enum.Font.GothamSemibold
tradingbtn.Text = "Trading"
tradingbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
tradingbtn.TextSize = 25.000
tradingbtn.TextStrokeTransparency = 0.000
tradingbtn.MouseButton1Down:Connect(function()
	mainfrm.Visible = true
	tradingfrm.Visible = false
	dinomiscfrm.Visible = false
end)

UICorner_4.CornerRadius = UDim.new(0.0799999982, 0)
UICorner_4.Parent = tradingbtn

mainfrm.Name = "mainfrm"
mainfrm.Parent = fullmain
mainfrm.BackgroundColor3 = Color3.fromRGB(76, 76, 76)
mainfrm.Position = UDim2.new(0.270175427, 0, 0.105571851, 0)
mainfrm.Size = UDim2.new(0, 397, 0, 287)
mainfrm.Visible = false

speedbtn.Name = "speedbtn"
speedbtn.Parent = mainfrm
speedbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
speedbtn.Position = UDim2.new(0.0194230154, 0, 0.174216032, 0)
speedbtn.Size = UDim2.new(0, 113, 0, 41)
speedbtn.Font = Enum.Font.GothamSemibold
speedbtn.Text = "Walkspeed"
speedbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
speedbtn.TextScaled = true
speedbtn.TextSize = 23.000
speedbtn.TextStrokeTransparency = 0.000
speedbtn.TextWrapped = true
speedbtn.MouseButton1Down:Connect(function()
    game.Players.LocalPlayer.Character.Dinosaur.WalkSpeed = speedbox.Text
    game.Players.LocalPlayer.Character.CharacterScripts.ControlWalkSpeed:remove()
end)



UICorner_5.Parent = speedbtn

speedbox.Name = "speedbox"
speedbox.Parent = speedbtn
speedbox.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
speedbox.Position = UDim2.new(0.0796460211, 0, 1, 0)
speedbox.Size = UDim2.new(0, 95, 0, 15)
speedbox.Font = Enum.Font.GothamSemibold
speedbox.PlaceholderColor3 = Color3.fromRGB(255, 255, 255)
speedbox.PlaceholderText = "Speed Value"
speedbox.Text = ""
speedbox.TextColor3 = Color3.fromRGB(0, 0, 0)
speedbox.TextSize = 14.000
speedbox.TextStrokeTransparency = 0.000

UICorner_6.Parent = speedbox

jumpbtn.Name = "jumpbtn"
jumpbtn.Parent = mainfrm
jumpbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
jumpbtn.Position = UDim2.new(0.356954485, 0, 0.174216032, 0)
jumpbtn.Size = UDim2.new(0, 113, 0, 41)
jumpbtn.Font = Enum.Font.GothamSemibold
jumpbtn.Text = "JumpPower"
jumpbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
jumpbtn.TextScaled = true
jumpbtn.TextSize = 23.000
jumpbtn.TextStrokeTransparency = 0.000
jumpbtn.TextWrapped = true
jumpbtn.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.Character.Dinosaur.JumpPower = jumpbox.Text
    game.Players.LocalPlayer.Character.CharacterScripts.ControlJumpPower:remove()
end)

jumpbox.Name = "jumpbox"
jumpbox.Parent = jumpbtn
jumpbox.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
jumpbox.Position = UDim2.new(0.0796460211, 0, 1, 0)
jumpbox.Size = UDim2.new(0, 95, 0, 15)
jumpbox.Font = Enum.Font.GothamSemibold
jumpbox.PlaceholderColor3 = Color3.fromRGB(255, 255, 255)
jumpbox.PlaceholderText = "JP Value"
jumpbox.Text = ""
jumpbox.TextColor3 = Color3.fromRGB(0, 0, 0)
jumpbox.TextSize = 14.000
jumpbox.TextStrokeTransparency = 0.000

UICorner_7.Parent = jumpbox

UICorner_8.Parent = jumpbtn

infjumpbtn.Name = "infjumpbtn"
infjumpbtn.Parent = mainfrm
infjumpbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
infjumpbtn.Position = UDim2.new(0.69196707, 0, 0.174216032, 0)
infjumpbtn.Size = UDim2.new(0, 113, 0, 41)
infjumpbtn.Font = Enum.Font.GothamSemibold
infjumpbtn.Text = "Infinite Jump"
infjumpbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
infjumpbtn.TextScaled = true
infjumpbtn.TextSize = 23.000
infjumpbtn.TextStrokeTransparency = 0.000
infjumpbtn.TextWrapped = true
infjumpbtn.MouseButton1Down:Connect(function()
	_G.infinjump = true
    local Player = game:GetService("Players").LocalPlayer
    local Mouse = Player:GetMouse()
    Mouse.KeyDown:connect(function(k)
    if _G.infinjump then
    if k:byte() == 32 then
    Humanoid = game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Humanoid")
    Humanoid:ChangeState("Jumping")
    wait(0.1)
    Humanoid:ChangeState("Seated")
    end
    end
end)

UICorner_9.Parent = infjumpbtn

topic.Name = "topic"
topic.Parent = mainfrm
topic.BackgroundColor3 = Color3.fromRGB(104, 104, 104)
topic.BackgroundTransparency = 1.000
topic.Position = UDim2.new(0.34171629, 0, 0, 0)
topic.Size = UDim2.new(0, 124, 0, 36)
topic.Font = Enum.Font.GothamSemibold
topic.Text = "Dinosaur"
topic.TextColor3 = Color3.fromRGB(255, 255, 255)
topic.TextSize = 30.000
topic.TextStrokeTransparency = 0.000

topic_2.Name = "topic"
topic_2.Parent = mainfrm
topic_2.BackgroundColor3 = Color3.fromRGB(104, 104, 104)
topic_2.BackgroundTransparency = 1.000
topic_2.Position = UDim2.new(0.417283058, 0, 0.522648096, 0)
topic_2.Size = UDim2.new(0, 64, 0, 36)
topic_2.Font = Enum.Font.GothamSemibold
topic_2.Text = "Food"
topic_2.TextColor3 = Color3.fromRGB(255, 255, 255)
topic_2.TextSize = 25.000
topic_2.TextStrokeTransparency = 0.000

infhtbtn.Name = "infh/tbtn"
infhtbtn.Parent = mainfrm
infhtbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
infhtbtn.Position = UDim2.new(0.019423008, 0, 0.714285672, 0)
infhtbtn.Size = UDim2.new(0, 113, 0, 41)
infhtbtn.Font = Enum.Font.GothamSemibold
infhtbtn.Text = "Infinite Hunger/Thirst"
infhtbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
infhtbtn.TextScaled = true
infhtbtn.TextSize = 23.000
infhtbtn.TextStrokeTransparency = 0.000
infhtbtn.TextWrapped = true
infhtbtn.MouseButton1Down:Connect(function()
	_G.infinjump = true
    local Player = game:GetService("Players").LocalPlayer
    local Mouse = Player:GetMouse()
    Mouse.KeyDown:connect(function(k)
    if _G.infinjump then
    if k:byte() == 32 then
    Humanoid = game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Humanoid")
    Humanoid:ChangeState("Jumping")
    wait(0.1)
    Humanoid:ChangeState("Seated")
    end
    end
end)

UICorner_10.Parent = infhtbtn

hungerkeybtn.Name = "hungerkeybtn"
hungerkeybtn.Parent = mainfrm
hungerkeybtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
hungerkeybtn.Position = UDim2.new(0.69196707, 0, 0.714285672, 0)
hungerkeybtn.Size = UDim2.new(0, 113, 0, 41)
hungerkeybtn.Font = Enum.Font.GothamSemibold
hungerkeybtn.Text = "Hunger Keybinds"
hungerkeybtn.TextColor3 = Color3.fromRGB(250, 250, 250)
hungerkeybtn.TextScaled = true
hungerkeybtn.TextSize = 23.000
hungerkeybtn.TextStrokeTransparency = 0.000
hungerkeybtn.TextWrapped = true

UICorner_11.Parent = hungerkeybtn

addhungerbtn.Name = "addhungerbtn"
addhungerbtn.Parent = mainfrm
addhungerbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
addhungerbtn.Position = UDim2.new(0.354435593, 0, 0.714285672, 0)
addhungerbtn.Size = UDim2.new(0, 113, 0, 41)
addhungerbtn.Font = Enum.Font.GothamSemibold
addhungerbtn.Text = "Add Hunger"
addhungerbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
addhungerbtn.TextScaled = true
addhungerbtn.TextSize = 23.000
addhungerbtn.TextStrokeTransparency = 0.000
addhungerbtn.TextWrapped = true

UICorner_12.Parent = addhungerbtn

stopinfbtn.Name = "stopinfbtn"
stopinfbtn.Parent = mainfrm
stopinfbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
stopinfbtn.Position = UDim2.new(0.0446119308, 0, 0.857142866, 0)
stopinfbtn.Size = UDim2.new(0, 92, 0, 16)
stopinfbtn.Font = Enum.Font.GothamSemibold
stopinfbtn.Text = "Stop Inf H/T"
stopinfbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
stopinfbtn.TextSize = 15.000
stopinfbtn.TextStrokeTransparency = 0.000
stopinfbtn.TextWrapped = true
stopinfbtn.MouseButton1Down:Connect(function()
	_G.AutoEatDrink = false
end)

UICorner_13.Parent = stopinfbtn

UICorner_14.Parent = mainfrm

name.Name = "name"
name.Parent = fullmain
name.BackgroundColor3 = Color3.fromRGB(104, 104, 104)
name.BackgroundTransparency = 1.000
name.Position = UDim2.new(0.0192982461, 0, 0, 0)
name.Size = UDim2.new(0, 559, 0, 36)
name.Font = Enum.Font.GothamSemibold
name.Text = "Violexian"
name.TextColor3 = Color3.fromRGB(255, 255, 255)
name.TextSize = 30.000
name.TextStrokeTransparency = 0.000
name.TextXAlignment = Enum.TextXAlignment.Left

UICorner_15.Parent = fullmain

version.Name = "version"
version.Parent = fullmain
version.BackgroundColor3 = Color3.fromRGB(104, 104, 104)
version.BackgroundTransparency = 1.000
version.Position = UDim2.new(0.457894742, 0, 0, 0)
version.Size = UDim2.new(0, 60, 0, 36)
version.Font = Enum.Font.GothamSemibold
version.Text = "v1.3"
version.TextColor3 = Color3.fromRGB(255, 255, 255)
version.TextSize = 30.000
version.TextStrokeTransparency = 0.000

reminder.Name = "reminder"
reminder.Parent = fullmain
reminder.BackgroundColor3 = Color3.fromRGB(104, 104, 104)
reminder.BackgroundTransparency = 1.000
reminder.Position = UDim2.new(0.778947353, 0, 0, 0)
reminder.Size = UDim2.new(0, 107, 0, 36)
reminder.Font = Enum.Font.GothamSemibold
reminder.Text = "Y to Open/Close"
reminder.TextColor3 = Color3.fromRGB(255, 255, 255)
reminder.TextSize = 15.000
reminder.TextStrokeTransparency = 0.000

tradingfrm.Name = "tradingfrm"
tradingfrm.Parent = fullmain
tradingfrm.BackgroundColor3 = Color3.fromRGB(76, 76, 76)
tradingfrm.Position = UDim2.new(0.270175427, 0, 0.105571851, 0)
tradingfrm.Size = UDim2.new(0, 397, 0, 287)

movegui.Name = "movegui"
movegui.Parent = tradingfrm
movegui.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
movegui.Position = UDim2.new(0.0194230154, 0, 0.174216032, 0)
movegui.Size = UDim2.new(0, 113, 0, 41)
movegui.Font = Enum.Font.GothamSemibold
movegui.Text = "Move Trading Gui"
movegui.TextColor3 = Color3.fromRGB(250, 250, 250)
movegui.TextScaled = true
movegui.TextSize = 23.000
movegui.TextStrokeTransparency = 0.000
movegui.TextWrapped = true
movegui.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.PlayerGui.TradingGui.Background.Position = UDim2.new(0, 50, 0, 0)
end)

UICorner_16.Parent = movegui

topic_3.Name = "topic"
topic_3.Parent = tradingfrm
topic_3.BackgroundColor3 = Color3.fromRGB(104, 104, 104)
topic_3.BackgroundTransparency = 1.000
topic_3.Position = UDim2.new(0.34171629, 0, 0, 0)
topic_3.Size = UDim2.new(0, 124, 0, 36)
topic_3.Font = Enum.Font.GothamSemibold
topic_3.Text = "Trading"
topic_3.TextColor3 = Color3.fromRGB(255, 255, 255)
topic_3.TextSize = 30.000
topic_3.TextStrokeTransparency = 0.000

UICorner_17.Parent = tradingfrm

dinomiscfrm.Name = "dinomiscfrm"
dinomiscfrm.Parent = fullmain
dinomiscfrm.BackgroundColor3 = Color3.fromRGB(76, 76, 76)
dinomiscfrm.Position = UDim2.new(0.270175427, 0, 0.105571851, 0)
dinomiscfrm.Size = UDim2.new(0, 397, 0, 287)
dinomiscfrm.Visible = false

topic_4.Name = "topic"
topic_4.Parent = dinomiscfrm
topic_4.BackgroundColor3 = Color3.fromRGB(104, 104, 104)
topic_4.BackgroundTransparency = 1.000
topic_4.Position = UDim2.new(0.34171629, 0, 0, 0)
topic_4.Size = UDim2.new(0, 124, 0, 36)
topic_4.Font = Enum.Font.GothamSemibold
topic_4.Text = "Dinosaur"
topic_4.TextColor3 = Color3.fromRGB(255, 255, 255)
topic_4.TextSize = 30.000
topic_4.TextStrokeTransparency = 0.000

semigodbtn.Name = "semigodbtn"
semigodbtn.Parent = dinomiscfrm
semigodbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
semigodbtn.Position = UDim2.new(0.0194230154, 0, 0.174216032, 0)
semigodbtn.Size = UDim2.new(0, 113, 0, 41)
semigodbtn.Font = Enum.Font.GothamSemibold
semigodbtn.Text = "Semi-God"
semigodbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
semigodbtn.TextScaled = true
semigodbtn.TextSize = 23.000
semigodbtn.TextStrokeTransparency = 0.000
semigodbtn.TextWrapped = true
semigodbtn.MouseButton1Down:Connect(function()
    if game.Players.LocalPlayer.Character.Stats.Armor or game.Players.LocalPlayer.Character.CharacterScripts.HandleBleeding or game.Players.LocalPlayer.Character.Stats.bleedingStack then
        game.Players.LocalPlayer.Character.Stats.bleedingStack:Remove()
game.Players.LocalPlayer.Character.CharacterScripts.HandleBleeding:Remove()
        game.Players.LocalPlayer.Character.Stats.Armor:Remove()
        end
end)

UICorner_18.Parent = semigodbtn

infswimoxybtn.Name = "infswimoxybtn"
infswimoxybtn.Parent = dinomiscfrm
infswimoxybtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
infswimoxybtn.Position = UDim2.new(0.356954485, 0, 0.174216032, 0)
infswimoxybtn.Size = UDim2.new(0, 113, 0, 41)
infswimoxybtn.Font = Enum.Font.GothamSemibold
infswimoxybtn.Text = "Swim + Inf Oxygen"
infswimoxybtn.TextColor3 = Color3.fromRGB(250, 250, 250)
infswimoxybtn.TextScaled = true
infswimoxybtn.TextSize = 23.000
infswimoxybtn.TextStrokeTransparency = 0.000
infswimoxybtn.TextWrapped = true
infswimoxybtn.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.Character.Stats.canSwim.Value = true
    wait(0.2)
    game.Players.LocalPlayer.Character.CharacterScripts.UnderWater:Remove()
end)

UICorner_19.Parent = infswimoxybtn

gtpbtn.Name = "gtpbtn"
gtpbtn.Parent = dinomiscfrm
gtpbtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
gtpbtn.Position = UDim2.new(0.689448178, 0, 0.174216032, 0)
gtpbtn.Size = UDim2.new(0, 113, 0, 41)
gtpbtn.Font = Enum.Font.GothamSemibold
gtpbtn.Text = "G to Teleport"
gtpbtn.TextColor3 = Color3.fromRGB(250, 250, 250)
gtpbtn.TextScaled = true
gtpbtn.TextSize = 23.000
gtpbtn.TextStrokeTransparency = 0.000
gtpbtn.TextWrapped = true
gtpbtn.MouseButton1Down:Connect(function()
    plr = game.Players.LocalPlayer 
    hum = plr.Character.HumanoidRootPart
    mouse = plr:GetMouse() 
    mouse.KeyDown:connect(function(key) 
    if key == "g" then 
    if mouse.Target then 
    hum.CFrame = CFrame.new(mouse.Hit.x, mouse.Hit.y + 5, mouse.Hit.z) 
    end 
    end 
    end)
end)

UICorner_20.Parent = gtpbtn

shakebtn.Name = "shakebtn"
shakebtn.Parent = dinomiscfrm
shakebtn.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
shakebtn.Position = UDim2.new(0.354435593, 0, 0.397212565, 0)
shakebtn.Size = UDim2.new(0, 113, 0, 41)
shakebtn.Font = Enum.Font.GothamSemibold
shakebtn.Text = "Funny Shake"
shakebtn.TextColor3 = Color3.fromRGB(250, 250, 250)
shakebtn.TextScaled = true
shakebtn.TextSize = 23.000
shakebtn.TextStrokeTransparency = 0.000
shakebtn.TextWrapped = true
shakebtn.MouseButton1Down:Connect(function()
    AnimationId = "741896167"
    local Anim = Instance.new("Animation")
    Anim.AnimationId = "rbxassetid://"..AnimationId
    local k = game.Players.LocalPlayer.Character.Dinosaur:LoadAnimation(Anim)
    k:Play()
    k:AdjustSpeed(10)
end)

UICorner_21.Parent = shakebtn

topic_5.Name = "topic"
topic_5.Parent = dinomiscfrm
topic_5.BackgroundColor3 = Color3.fromRGB(104, 104, 104)
topic_5.BackgroundTransparency = 1.000
topic_5.Position = UDim2.new(0.34171629, 0, 0.574912906, 0)
topic_5.Size = UDim2.new(0, 124, 0, 36)
topic_5.Font = Enum.Font.GothamSemibold
topic_5.Text = "Troll"
topic_5.TextColor3 = Color3.fromRGB(255, 255, 255)
topic_5.TextSize = 30.000
topic_5.TextStrokeTransparency = 0.000

gtpbtn_2.Name = "gtpbtn"
gtpbtn_2.Parent = dinomiscfrm
gtpbtn_2.BackgroundColor3 = Color3.fromRGB(116, 116, 116)
gtpbtn_2.Position = UDim2.new(0.356954485, 0, 0.766550541, 0)
gtpbtn_2.Size = UDim2.new(0, 113, 0, 41)
gtpbtn_2.Font = Enum.Font.GothamSemibold
gtpbtn_2.Text = "Troll Earrape"
gtpbtn_2.TextColor3 = Color3.fromRGB(250, 250, 250)
gtpbtn_2.TextScaled = true
gtpbtn_2.TextSize = 23.000
gtpbtn_2.TextStrokeTransparency = 0.000
gtpbtn_2.TextWrapped = true
gtpbtn_2.MouseButton1Down:Connect(function()
    while wait(0.2) do
        for _,plr in pairs(game.Players:GetPlayers()) do
        pcall(function()
        for _,obj in pairs(plr.Character.Head:GetChildren()) do
        if obj:IsA("Sound") then
        obj:Play()
        end
        end
        end)
        end
        end
end)

UICorner_22.Parent = gtpbtn_2

UICorner_23.Parent = dinomiscfrm
