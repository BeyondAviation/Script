wait(2)
script.Parent.Text = "loading scripts 0/6"
wait(0.5)
script.Parent.Text = "loading scripts 1/6"
wait(0.5)
script.Parent.Text = "loading scripts 2/6"
wait(0.5)
script.Parent.Text = "loading scripts 3/6"
wait(0.5)
script.Parent.Text = "loading scripts 4/6"
wait(0.5)
script.Parent.Text = "loading scripts 5/6"
wait(0.5)
script.Parent.Text = "loading scripts 6/6"
wait(2)
script.Parent.Text = "Finding game."
wait(.25)
script.Parent.Text = "Finding game.."
wait(.25)
script.Parent.Text = "Finding game..."
wait(.25)
script.Parent.Text = "Finding game.."
wait(.25)
script.Parent.Text = "Finding game."
wait(.25)
script.Parent.Text = "Finding game.."
wait(.25)
script.Parent.Text = "Finding game..."
wait(.25)
script.Parent.Text = "Finding game.."
wait(.25)
script.Parent.Text = "Finding game."
wait(.25)
script.Parent.Text = "Finding game.."
wait(.25)
script.Parent.Text = "Finding game..."
wait(.25)
script.Parent.Text = "Finding game.."
wait(.25)
script.Parent.Text = "Finding game."
wait(.25)
script.Parent.Text = "Finding game.."
wait(.25)
script.Parent.Text = "Finding game..."
wait(.25)
script.Parent.Text = "Finding game.."
wait(.25)
script.Parent.Text = "Finding game."
wait(.25)
script.Parent.Text = "Finding game.."
wait(.25)
script.Parent.Text = "Finding game..."
wait(1)
script.Parent.Text = "Found game!"
wait(2)
if game then
	script.Parent.Text = "Game Is supported!"
end

wait(3)
script.Parent.Visible = false
script.Parent.Parent.Image.Visible = true
script.Parent.Parent.TextLabel2.Visible = true

while true do 
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525499"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525683"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525701"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525701"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525723"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525739"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525800"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525806"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525814"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525821"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525833"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525858"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114525874"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526055"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526120"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526125"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526135"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526159"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526166"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526176"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526195"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526204"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526214"
	wait(0.1)
	script.Parent.Parent.Image.Image = "http://www.roblox.com/asset/?id=114526229"
	wait(0.1)
end 

local UserInputService = game:GetService("UserInputService")

local gui = script.Parent.Parent

local dragging
local dragInput
local dragStart
local startPos

local function update(input)
	local delta = input.Position - dragStart
	gui.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
end

gui.InputBegan:Connect(function(input)
	if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
		dragging = true
		dragStart = input.Position
		startPos = gui.Position

		input.Changed:Connect(function()
			if input.UserInputState == Enum.UserInputState.End then
				dragging = false
			end
		end)
	end
end)

gui.InputChanged:Connect(function(input)
	if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
		dragInput = input
	end
end)

UserInputService.InputChanged:Connect(function(input)
	if input == dragInput and dragging then
		update(input)
	end
end)
