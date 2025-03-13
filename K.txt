local players = game:GetService("Players")
local player = players.LocalPlayer
local teams = game:GetService("Teams")
local replicatedStorage = game:GetService("ReplicatedStorage")
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/PresidentZuyi/S/refs/heads/main/C"))()

MakeWindow({
  Hub = {
    Title = "President Zuyi Official Hub (¥)",
    Animation = "Enjoy!🔥👀"
  },
  Key = {
    KeySystem = true,
    Title = "PresidentZuyi Official Hub ‼️  (¥)",
    Description = "^ Blue Lock Rivals ^",
    KeyLink = "https://discord.gg/TAFQb2QvaM",
    Keys = {"zuyiandexecutive", "71838", "28282", "1", "28282"},
    Notifi = {
      Notifications = true,
      CorrectKey = "Correct✅",
      Incorrectkey = "False😡‼️",
      CopyKeyLink = "Copied Discord Link"
    }
  }
})

MinimizeButton({
  Image = "rbxassetid://14693252997",
  Size = {40, 40},
  Color = Color3.fromRGB(10, 10, 10),
  Corner = true,
  Stroke = true,
  StrokeColor = Color3.fromHSV(0.5, 1, 1)  -- Hue: 180° for cyan
})

MakeNotifi({
  Title = "Executed!",
  Text = "Boom!✅",
  Time = 5
})

local Main = MakeTab({Name = "Zuyis Portal😜"})

local Image = AddImageLabel(Main, {
  Name = "PresidentZuyi🔗",
  Image = "rbxassetid://7229442422"
})
local Paragraph1 = AddParagraph(Main, {"Zuyi’s Official Hub ✅", "CREDIT"})
local Paragraph2 = AddParagraph(Main, {"More Games Getting Supported Soon", "INFO"})
local Paragraph3 = AddParagraph(Main, {"Only Blue Lock Rivals Supported"})
local Paragraph4 = AddParagraph(Main, {"PresidentZuyi Is The Owner Of This Script"})

-- Auto
local Main = MakeTab({Name = "Custom Styles"})

AddButton(Main, { 
  Name = "¥ Get Gojo Satoru Style💙❤️", 
  Description = "Why’d u click it ts pmo☠️!", 
  Callback = function()
      loadstring(game:HttpGet('https://raw.githubusercontent.com/PresidentZuyi/H/refs/heads/main/B'))()
  end
}) 

AddButton(Main, {
  Name = "¥ Get Ego Jinpachi Style🧠",
  Callback = function()
    local function runScript(url)
      loadstring(game:HttpGet(url))()
    end
    
    local co1 = coroutine.create(runScript)
    local co2 = coroutine.create(runScript)
    
    coroutine.resume(co1, "https://raw.githubusercontent.com/PresidentZuyi/Shh/refs/heads/main/C")
    coroutine.resume(co2, "https://raw.githubusercontent.com/PresidentZuyi/Shh/refs/heads/main/F")
  end
})

AddButton(Main, {
  Name = "¥ Get Igaguri Gurimu Style🕉️",
  Callback = function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/PresidentZuyi/Hi/refs/heads/main/Chh"))()
  end
})

AddButton(Main, {
  Name = "¥ Lavinho The Dribbler Coming Soon!✅",
  Callback = function()
    -- No action needed for this button
  end
})

-- Rename Read section to Important and add the buttons
local Important = MakeTab({Name = "Misc😵‍💫"})

local Image = AddImageLabel(Important, {
  Name = "PresidentZuyi🔗",
  Image = "rbxassetid://7229442422"
})

AddButton(Important, {
  Name = "‼️ No Ability Cooldown",
  Callback = function()
    local AbilityController = require(cloneref(game:GetService("ReplicatedStorage")).Controllers.AbilityController)
    local OriginalAbilityCooldown; 
    OriginalAbilityCooldown = hookfunction(AbilityController.AbilityCooldown, function(Self)
      return
    end)

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "‼️ No Cooldown Script Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(Important, {
  Name = "🔥 GK Ball Expander",
  Callback = function()
    while task.wait(0) do
      loadstring(game:HttpGet("https://pastebin.com/raw/T5m4nwPq"))()

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Infinite Stamina Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(Important, {
  Name = "⬆️ Infinite Jump",
  Callback = function()
    local InfiniteJumpEnabled = true
    game:GetService("UserInputService").JumpRequest:connect(function()
      if InfiniteJumpEnabled then
        game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Humanoid"):ChangeState("Jumping")
      end
    end)

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Infinite Jump Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

-- New Cosmetics section
local NewCosmetics = MakeTab({Name = "New Cosmetics‼️"})

local Paragraph1 = AddParagraph(NewCosmetics, {"This Is Where All The New Cosmetics Will Be Added"})

AddButton(NewCosmetics, {
  Name = "¥ New Cosmic Aura",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("Cosmetics", "COSMIC")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "New Cosmic Aura Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewCosmetics, {
  Name = "¥ Angel Wings",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("Cosmetics", "Angel Wings")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Angel Wings Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewCosmetics, {
  Name = "¥ Lanterns!",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("Cosmetics", "Lanterns!")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Lanterns Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewCosmetics, {
  Name = "¥ Shidou Wings",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("Cosmetics", "Shidou Wings!")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Shidou Wings Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewCosmetics, {
  Name = "¥ Dragon Cape",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("Cosmetics", "Dragon Cape")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Dragon Cape Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewCosmetics, {
  Name = "¥ New Grills Cosmetic",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("Cosmetics", "Golden Grills")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "New Grills Cosmetic Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewCosmetics, {
  Name = "¥ Valentines Aura",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("Cosmetics", "Valentines")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Valentines Aura Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewCosmetics, {
  Name = "¥ New Zodiac Aura👀",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("Cosmetics", "Zodiac")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Zodiac Aura Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewCosmetics, {
  Name = "¥ New Designer Gloves Cosmetic🔥",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("Cosmetics", "Designer Gloves")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Designer Gloves Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

-- New Goal Effects section
local NewGoalEffects = MakeTab({Name = "New Goal Effects🤑"})

local Paragraph1 = AddParagraph(NewGoalEffects, {"This Is Where All The New Goal Effects Will Be Located"})

AddButton(NewGoalEffects, {
  Name = "¥ Grillz Goal Effect",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("GoalEffects", "Grillz")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Grillz Goal Effect Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewGoalEffects, {
  Name = "¥ Timestop Goal Effect",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("GoalEffects", "Time Stop")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Timestop Goal Effect Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewGoalEffects, {
  Name = "¥ Vaporwave Goal Effect",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("GoalEffects", "Vaporwave")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Vaporwave Goal Effect Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewGoalEffects, {
  Name = "¥ Graveyard Goal Effect",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("GoalEffects", "GRAVEYARD")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Graveyard Goal Effect Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

AddButton(NewGoalEffects, {
  Name = "¥ Conquer Goal Effect",
  Callback = function()
    cloneref(game:GetService("ReplicatedStorage")).Packages.Knit.Services.CustomizationService.RE.Customize:FireServer("GoalEffects", "Conquer")

    game:GetService("StarterGui"):SetCore("SendNotification", {
      Title = "Join PresidentZuyi Hub For Updates!",
      Text = "Conquer Goal Effect Completed✅",
      Button1 = "W Zuyi!",
      Button2 = "W Zuyi!",
      Duration = 90
    })
  end
})

-- New Emotes sections
local AnimeEmotes = MakeTab({Name = "Anime Emotes🐐"})
local ToxicEmotes = MakeTab({Name = "Toxic Emotes😡"})
local OtherEmotes = MakeTab({Name = "Other Emotes😉"})

local Paragraph1 = AddParagraph(AnimeEmotes, {"This Is Where All The Anime Emotes Will Be Added"})
local Paragraph2 = AddParagraph(ToxicEmotes, {"This Is Where All The Toxic Emotes Will Be Added"})
local Paragraph3 = AddParagraph(OtherEmotes, {"This Is Where All The Other Emotes Will Be Added"})

-- Adding the new button to the Toxic Emotes section
AddButton(ToxicEmotes, {
  Name = "¥ Toxic Laugh Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://117834213273979"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Toxic Laugh By Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(ToxicEmotes, {
  Name = "¥ Toxic L Dance Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://105830694875557"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Toxic L Dance By Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(ToxicEmotes, {
  Name = "¥ Toxic Ninja Run Dance Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://72224249513625"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Toxic Ninja Run Dance Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(ToxicEmotes, {
  Name = "¥ Toxic Money Rain Dance Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://71762198316531"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Money Rain Run Dance Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(AnimeEmotes, {
  Name = "¥ Honoured One Anime Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://125865269944406"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Six Eyes By Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(AnimeEmotes, {
  Name = "¥ Ultra Instinct Anime Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://80405783743287"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Goku Aura Emote Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(AnimeEmotes, {
  Name = "¥ Bizzare Anime Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://94252080933749"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Bizzare Emote Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(AnimeEmotes, {
  Name = "¥ ROAR Anime Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://133572818797711"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "ROAR Emote Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(OtherEmotes, {
  Name = "¥ Whip Dance Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://94649499784710"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Whip Emote Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(OtherEmotes, {
  Name = "¥ Rin Quest Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://89006553430967"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Rin Emote Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(OtherEmotes, {
  Name = "¥ Isagi Kneel Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://88982797209625"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Kneel Emote Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(OtherEmotes, {
  Name = "¥ Grillz Paid Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://111955433756506"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Grillz Emote Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(OtherEmotes, {
  Name = "¥ Gentleman Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://96723009482766"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Gentleman Emote Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(OtherEmotes, {
  Name = "¥ Cry Loser Paid Emote",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://97771700408539"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Cry Emote Zuyi"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})

AddButton(OtherEmotes, {
  Name = "⚠️‼️ZUYI SPECIAL EMOTE‼️⚠️",
  Callback = function()
    local player = game.Players.LocalPlayer

    local function cleanup()
        -- Remove any existing GUI named "PlayEmoteGUI"
        if player.PlayerGui:FindFirstChild("PlayEmoteGUI") then
            player.PlayerGui:FindFirstChild("PlayEmoteGUI"):Destroy()
        end
    end

    local function initializeAbility()
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

        -- The animation for the dribble/drive move
        local animation = Instance.new("Animation")
        animation.AnimationId = "rbxassetid://85217612132841"  -- Replace with your desired animation ID
        local animationTrack = humanoid:LoadAnimation(animation)

        -- Set the animation priority to Action to ensure it overrides the idle animation
        animationTrack.Priority = Enum.AnimationPriority.Action

        -- Sound for the move
        local sound = Instance.new("Sound")
        sound.SoundId = ""  -- Change the sound ID
        sound.Parent = humanoidRootPart  -- You can attach the sound to the character's root part

        -- Function to trigger the ability
        local function triggerAbility()
            -- Play the sound at the start of the move
            sound:Play()

            -- Start the animation immediately with smooth blending
            animationTrack:Play(0.1, 1, 1)

            -- Stop the animation after 3 seconds
            task.delay(3, function()
                animationTrack:Stop(0.1)
            end)
        end

        -- Create the GUI button
        local screenGui = Instance.new("ScreenGui")
        screenGui.Name = "PlayEmoteGUI"
        screenGui.Parent = player.PlayerGui

        local button = Instance.new("TextButton")
        button.Size = UDim2.new(0, 150, 0, 30)
        button.Position = UDim2.new(0.5, -75, 0.5, -15)
        button.BackgroundColor3 = Color3.new(0, 0, 0)
        button.TextColor3 = Color3.new(1, 1, 1)
        button.Text = "Zuyi Special Emote"
        button.Parent = screenGui

        -- Make the GUI draggable
        local dragging
        local dragInput
        local dragStart
        local startPos

        local function update(input)
            local delta = input.Position - dragStart
            button.Position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X, startPos.Y.Scale, startPos.Y.Offset + delta.Y)
        end

        button.InputBegan:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
                dragging = true
                dragStart = input.Position
                startPos = button.Position

                input.Changed:Connect(function()
                    if input.UserInputState == Enum.UserInputState.End then
                        dragging = false
                    end
                end)
            end
        end)

        button.InputChanged:Connect(function(input)
            if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
                dragInput = input
            end
        end)

        game:GetService("UserInputService").InputChanged:Connect(function(input)
            if input == dragInput and dragging then
                update(input)
            end
        end)

        -- Listen for the button activation (when clicked)
        button.MouseButton1Click:Connect(function()
            -- Trigger the ability when the button is clicked
            triggerAbility()
        end)
    end

    -- Reinitialize the ability each time the character is added (e.g., when joining a match)
    player.CharacterAdded:Connect(function()
        cleanup()
        initializeAbility()
    end)

    -- Initial cleanup and ability initialization
    cleanup()
    if player.Character then
        initializeAbility()
    end
  end
})
