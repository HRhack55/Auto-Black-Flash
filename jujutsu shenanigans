local function blackflashgojo()
    print("blackflashgojo start", tick())
    game:GetService("ReplicatedStorage").Knit.Knit.Services.ReversalRedMaxService.RE.Activated:FireServer("false")
    game:GetService("ReplicatedStorage").Knit.Knit.Services.GojoService.RE.RightActivated:FireServer()
    print("blackflashgojo end", tick())
end

local function blackflashsmg()
game:GetService("ReplicatedStorage").Knit.Knit.Services.FocusStrikeService.RE.Activated:FireServer("false")
end

local function blackflash()
    print("blackflash start", tick())
    game:GetService("ReplicatedStorage").Knit.Knit.Services.DivergentFistService.RE.Activated:FireServer("false")
    print("blackflash end", tick())
end

local function blueflash()
    print("blueflash start", tick())
    game:GetService("ReplicatedStorage").Knit.Knit.Services.DivergentFistService.RE.Activated:FireServer("true")
    print("blueflash end", tick())
end

local function run_blackflashgojo()
    local success, err = pcall(function()
        blackflashgojo()
        wait(0.32)
        blackflashgojo()
    end)

    if not success then
        blueflash()
    end
end

local function run_blackflash()
    local success, err = pcall(function()
        blackflash()
        wait(0.32)
        blackflash()
    end)

    if not success then
        blueflash()
    end
end

local function run_blackflashsmg()
local success, err = pcall(function()
        blackflashsmg()
        wait(0.32)
        blackflashsmg()
    end)

    if not success then
        blueflash()
    end
end

local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Parent = game.CoreGui

local ServerHopButton = Instance.new("TextButton")
ServerHopButton.Text = "Black Flash"
ServerHopButton.Size = UDim2.new(0, 200, 0, 50)
ServerHopButton.Position = UDim2.new(0.5, -100, 0.25, 0)
ServerHopButton.Active = true
ServerHopButton.Draggable = true
ServerHopButton.ClipsDescendants = true
ServerHopButton.Parent = ScreenGui

ServerHopButton.MouseButton1Click:Connect(function()
    task.spawn(run_blackflashgojo)
    task.spawn(run_blackflashsmg)
    task.spawn(run_blackflash)
end)
