local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("A Lagacy time by TNX", "DarkTheme")
local Tab = Window:NewTab("Tp item")
local Section = Tab:NewSection("Tp")
Section:NewToggle("tp", "ToggleInfo", function(state)
    if state then
        print("Toggle On")
        _G.AutoTp = true
        while _G.AutoTp do wait()
        for i,v in pairs(game:GetService("Workspace").Items:GetDescendants()) do
 if   v.Name == "TouchInterest" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Parent.CFrame
        end
    end
end

    else
        print("Toggle Off")
        _G.AutoTp = false
        while _G.AutoTp do wait()
            end
    end
end)
Section:NewToggle("Warp ma ha chan", "ToggleInfo", function(state)
    if state then
        print("Toggle On")
        _G.AutoWarp = true
        while _G.AutoWarp do wait()
        for i,v in pairs(game:GetService("Workspace").Items:GetChildren()) do
    if v.ClassName == "Tool" then
        v.Handle.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
         end
    end
end
    else
        print("Toggle Off")
        _G.AutoWarp = false
        while _G.AutoWarp do wait()
            end
    end
end)
local Tab = Window:NewTab("Tp ณเส้นขอบฟ้า")
local Section = Tab:NewSection("Save")
Section:NewButton("วาปมาหาพ่อเธอ", "ButtonInfo", function()
    print("Clicked")
     game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-3830.00415, 1426.65918, 1997.70215, -0.959183216, 3.81081655e-09, 0.282785296, 1.69172676e-08, 1, 4.39058994e-08, -0.282785296, 4.68977603e-08, -0.959183216)
end)
Section:NewButton("ประกอบของ", "ButtonInfo", function()
    print("Clicked")
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4385.94775, 1287.07959, 2994.97876, -0.927346885, -3.53716452e-08, 0.374202788, -9.34182331e-09, 1, 7.13744868e-08, -0.374202788, 6.26931751e-08, -0.92734)
end)
Section:NewButton("สนามไร้ขอบเขต", "ButtonInfo", function()
    print("Clicked")
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4896.4126, 1285.21277, 2719.66235, -0.866724372, 4.99054487e-09, 0.498787433, -8.41134362e-09, 1, -2.46214338e-08, -0.498787433, -2.55354689e-08, -0.866724372)
end)
Section:NewButton("กลาง", "ButtonInfo", function()
    print("Clicked")
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4186.15039, 1288.64673, 2411.88721, -0.12451636, -2.22644321e-08, 0.992217541, 2.56058215e-08, 1, 2.56524153e-08, -0.992217541, 2.86006916e-08, -0.12451636)
end)
