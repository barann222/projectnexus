-- Services
local players = game:GetService("Players")
local tweenService = game:GetService("TweenService")
local runService = game:GetService("RunService")
local coreGui = game:GetService("CoreGui")
local uis = game:GetService("UserInputService")

local redtext = "NEXUS"

--vars
local lp = players.LocalPlayer
local mouse = lp:GetMouse()
local viewport = workspace.CurrentCamera.ViewportSize
local tweenInfo = TweenInfo.new(0.1, Enum.EasingStyle.Quad, Enum.EasingDirection.InOut )

local Library = {}

function Library:validate(defaults, options)
	for i, v in pairs(defaults) do
		if options[i] == nil then
			options[i] = v
		end
	end
	return options
end

function Library:tween(object, goal, callback)
	local tween = tweenService:Create(object, tweenInfo, goal)
	tween.Completed:Connect(function()
		if callback then
			callback()
		end
	end)
	tween:Play()
end



function Library:Init(options)
	options = Library:validate({
		name = "PROJECT",
		name2 = "NEXUS",
		name3 = "Shindo Life | v 6.5"
	}, options or {})
	local GUI = {
		CurrentTab = nil
	}

	-- Main Frame
	do



		GUI["1d"] = Instance.new("ScrollingFrame", GUI["1b"])
		GUI["1d"].Active = true
		GUI["1d"].BorderSizePixel = 0
		GUI["1d"].CanvasSize = UDim2.new(0, 0, 0, 559)
		GUI["1d"].ElasticBehavior = Enum.ElasticBehavior.Always
		GUI["1d"].BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		GUI["1d"].VerticalScrollBarInset = Enum.ScrollBarInset.ScrollBar
		GUI["1d"].BackgroundTransparency = 1
		GUI["1d"].Size = UDim2.new(-0.02277432754635811, 470, 1, 49)
		GUI["1d"].ScrollBarImageColor3 = Color3.fromRGB(0, 0, 0)
		GUI["1d"].ClipsDescendants = false
		GUI["1d"].BorderColor3 = Color3.fromRGB(0, 0, 0)
		GUI["1d"].ScrollBarThickness = 0
		GUI["1d"].Position = UDim2.new(0, 9, 0, 19)
		GUI["1d"].Name = "HomeTab"
		GUI["1d"].Parent = GUI["1b"]
		GUI["1d"].Visible = false

		-- StarterGui.MyLibrary
		GUI["1"] = Instance.new("ScreenGui", runService:IsStudio() and players.LocalPlayer:WaitForChild("PlayerGui") or coreGui)
		GUI["1"].Name = "MyLibrary"
		GUI["1"].ZIndexBehavior = Enum.ZIndexBehavior.Sibling
		GUI["1"]["IgnoreGuiInset"] = true
		GUI["1"]["ResetOnSpawn"] = false

		-- StarterGui.MyLibrary.Main
		GUI["2"] = Instance.new("Frame", GUI["1"])
		GUI["2"].BorderSizePixel = 0
		GUI["2"].BackgroundColor3 = Color3.fromRGB(46, 46, 46)
		GUI["2"].AnchorPoint = Vector2.new(0.5, 0.5)
		GUI["2"].Size = UDim2.new(0, 657, 0, 402)
		GUI["2"].BorderColor3 = Color3.fromRGB(0, 0, 0)
		GUI["2"].Position = UDim2.new(0.5, 0,0.5, 0)
		GUI["2"].Name = "Main"

		-- StarterGui.MyLibrary.Main.UICorner
		GUI["3"] = Instance.new("UICorner", GUI["2"])
		-- StarterGui.MyLibrary.Main.TopBar
		GUI["4"] = Instance.new("Frame", GUI["2"]);
		GUI["4"]["BorderSizePixel"] = 0;
		GUI["4"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
		GUI["4"]["Size"] = UDim2.new(1, 0, 0, 27);
		GUI["4"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["4"]["Name"] = [[TopBar]];

		-- StarterGui.MyLibrary.Main.TopBar.UICorner
		GUI["5"] = Instance.new("UICorner", GUI["4"]);


		-- StarterGui.MyLibrary.Main.TopBar.Extension
		GUI["6"] = Instance.new("Frame", GUI["4"]);
		GUI["6"]["BorderSizePixel"] = 0;
		GUI["6"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
		GUI["6"]["AnchorPoint"] = Vector2.new(0, 1);
		GUI["6"]["Size"] = UDim2.new(1, 0, 0.5, 0);
		GUI["6"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["6"]["Position"] = UDim2.new(0, 0, 1, 0);
		GUI["6"]["Name"] = [[Extension]];

		-- StarterGui.MyLibrary.Main.TopBar.Title
		GUI["7"] = Instance.new("TextLabel", GUI["4"]);
		GUI["7"]["TextWrapped"] = true;
		GUI["7"]["BorderSizePixel"] = 0;
		GUI["7"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["7"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		GUI["7"]["FontFace"] = Font.new([[rbxasset://fonts/families/FredokaOne.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		GUI["7"]["TextSize"] = 17;
		GUI["7"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["7"]["Size"] = UDim2.new(0.5, 0, 0.699999988079071, 0);
		GUI["7"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["7"]["Text"] = options["name"];
		GUI["7"]["Name"] = options["name"];
		GUI["7"]["BackgroundTransparency"] = 1;
		GUI["7"]["Position"] = UDim2.new(0, 0, 0, 5);

		-- StarterGui.MyLibrary.Main.TopBar.Title.UIPadding
		GUI["8"] = Instance.new("UIPadding", GUI["7"]);
		GUI["8"]["PaddingLeft"] = UDim.new(0, 23);

		-- StarterGui.MyLibrary.Main.TopBar.Title2
		GUI["9"] = Instance.new("TextLabel", GUI["4"]);
		GUI["9"]["TextWrapped"] = true;
		GUI["9"]["BorderSizePixel"] = 0;
		GUI["9"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["9"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		GUI["9"]["FontFace"] = Font.new([[rbxasset://fonts/families/FredokaOne.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		GUI["9"]["TextSize"] = 17;
		GUI["9"]["TextColor3"] = Color3.fromRGB(246, 3, 3);
		GUI["9"]["Size"] = UDim2.new(0.5, 0, 0.699999988079071, 0);
		GUI["9"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["9"]["Text"] = options["name2"];
		GUI["9"]["Name"] = options["name2"];
		GUI["9"]["BackgroundTransparency"] = 1;
		GUI["9"]["Position"] = UDim2.new(0.11999999731779099, 0, 0, 5);

		-- StarterGui.MyLibrary.Main.TopBar.Title2.UIPadding
		GUI["a"] = Instance.new("UIPadding", GUI["9"]);
		GUI["a"]["PaddingLeft"] = UDim.new(0, 23);

		-- StarterGui.MyLibrary.Main.TopBar.TextBox
		GUI["b"] = Instance.new("TextBox", GUI["4"]);
		GUI["b"]["CursorPosition"] = -1;
		GUI["b"]["PlaceholderColor3"] = Color3.fromRGB(179, 179, 179);
		GUI["b"]["BorderSizePixel"] = 0;
		GUI["b"]["TextEditable"] = false;
		GUI["b"]["TextSize"] = 14;
		GUI["b"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["b"]["TextColor3"] = Color3.fromRGB(179, 179, 179);
		GUI["b"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		GUI["b"]["BackgroundTransparency"] = 1;
		GUI["b"]["Size"] = UDim2.new(0, 100, 0, 15);
		GUI["b"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["b"]["Text"] = [[[ Enum.Keycode.LeftShift ]];
		GUI["b"]["Position"] = UDim2.new(1, -120, 0, 5);
		GUI["b"]["ClearTextOnFocus"] = false;

		-- StarterGui.MyLibrary.Main.TopBar.TextBox.LocalScript
		GUI["c"] = Instance.new("LocalScript", GUI["b"]);


		-- StarterGui.MyLibrary.Main.TopBar.Line
		GUI["d"] = Instance.new("Frame", GUI["4"]);
		GUI["d"]["BorderSizePixel"] = 0;
		GUI["d"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
		GUI["d"]["Size"] = UDim2.new(1, 0, 0, 1);
		GUI["d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["d"]["Position"] = UDim2.new(0, 0, 1, 0);
		GUI["d"]["Name"] = [[Line]];

		-- StarterGui.MyLibrary.Main.TopBar.Game
		GUI["e"] = Instance.new("TextLabel", GUI["4"]);
		GUI["e"]["TextWrapped"] = true;
		GUI["e"]["BorderSizePixel"] = 0;
		GUI["e"]["TextScaled"] = true;
		GUI["e"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["e"]["FontFace"] = Font.new([[rbxasset://fonts/families/GothamSSm.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		GUI["e"]["TextTransparency"] = 0.5;
		GUI["e"]["TextSize"] = 14;
		GUI["e"]["TextColor3"] = Color3.fromRGB(113, 113, 113);
		GUI["e"]["Size"] = UDim2.new(0.5, 0, 0.699999988079071, 0);
		GUI["e"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["e"]["Text"] = options["name3"];
		GUI["e"]["Name"] = options["name3"];
		GUI["e"]["BackgroundTransparency"] = 1;
		GUI["e"]["Position"] = UDim2.new(0, 176, 0, 5);

		-- StarterGui.MyLibrary.Main.TopBar.Game.UIPadding
		GUI["f"] = Instance.new("UIPadding", GUI["e"]);
		GUI["f"]["PaddingLeft"] = UDim.new(0, 23);
		-- StarterGui.MyLibrary.Main.ContentContainer
		GUI["1a"] = Instance.new("Frame", GUI["2"]);
		GUI["1a"]["ZIndex"] = 10;
		GUI["1a"]["BorderSizePixel"] = 0;
		GUI["1a"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
		GUI["1a"]["AnchorPoint"] = Vector2.new(1, 0);
		GUI["1a"]["BackgroundTransparency"] = 1;
		GUI["1a"]["Size"] = UDim2.new(1, -174, 1, -42);
		GUI["1a"]["ClipsDescendants"] = true;
		GUI["1a"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["1a"]["Position"] = UDim2.new(1, -5, 0, 36);
		GUI["1a"]["Name"] = [[ContentContainer]];

		-- StarterGui.MyLibrary.Main.ContentContainer.UICorner
		GUI["1b"] = Instance.new("UICorner", GUI["1a"]);
		
		-- StarterGui.MyLibrary.Main.BackGround
		GUI["50"] = Instance.new("Frame", GUI["2"]);
		GUI["50"]["ZIndex"] = 1;
		GUI["50"]["BorderSizePixel"] = 0;
		GUI["50"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
		GUI["50"]["Size"] = UDim2.new(0, 480, 0, 361);
		GUI["50"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["50"]["Position"] = UDim2.new(0, 168, 0, 34);
		GUI["50"]["Name"] = [[BackGround]];

		-- StarterGui.MyLibrary.Main.BackGround.UICorner
		GUI["51"] = Instance.new("UICorner", GUI["50"]);
	end

	-- Navigation
	do
		-- StarterGui.MyLibrary.Main.Navigation
		GUI["10"] = Instance.new("Frame", GUI["2"]);
		GUI["10"]["BorderSizePixel"] = 0;
		GUI["10"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
		GUI["10"]["Size"] = UDim2.new(0, 158, 0, 361);
		GUI["10"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["10"]["Position"] = UDim2.new(0, 5, 0, 34);
		GUI["10"]["Name"] = [[Navigation]];

		-- StarterGui.MyLibrary.Main.Navigation.UICorner
		GUI["11"] = Instance.new("UICorner", GUI["10"]);


		-- StarterGui.MyLibrary.Main.Navigation.Hide
		GUI["12"] = Instance.new("Frame", GUI["10"]);
		GUI["12"]["BorderSizePixel"] = 0;
		GUI["12"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
		GUI["12"]["Size"] = UDim2.new(1, 0, 0, 20);
		GUI["12"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["12"]["Name"] = [[Hide]];

		-- StarterGui.MyLibrary.Main.Navigation.Hide.UICorner
		GUI["13"] = Instance.new("UICorner", GUI["12"]);


		-- StarterGui.MyLibrary.Main.Navigation.Hide2
		GUI["14"] = Instance.new("Frame", GUI["10"]);
		GUI["14"]["BorderSizePixel"] = 0;
		GUI["14"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
		GUI["14"]["AnchorPoint"] = Vector2.new(1, 0);
		GUI["14"]["BackgroundTransparency"] = 1;
		GUI["14"]["Size"] = UDim2.new(0, 20, 1, 0);
		GUI["14"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["14"]["Position"] = UDim2.new(1, 0, 0, 0);
		GUI["14"]["Name"] = [[Hide2]];

		-- StarterGui.MyLibrary.Main.Navigation.Hide2.UICorner
		GUI["15"] = Instance.new("UICorner", GUI["14"]);


		-- StarterGui.MyLibrary.Main.Navigation.ButtonHolder
		GUI["16"] = Instance.new("Frame", GUI["10"]);
		GUI["16"]["BorderSizePixel"] = 0;
		GUI["16"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["16"]["BackgroundTransparency"] = 1;
		GUI["16"]["Size"] = UDim2.new(1, 0, 1, 0);
		GUI["16"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["16"]["Name"] = [[ButtonHolder]];

		-- StarterGui.MyLibrary.Main.Navigation.ButtonHolder.UIPadding
		GUI["17"] = Instance.new("UIPadding", GUI["16"]);
		GUI["17"]["PaddingTop"] = UDim.new(0, 8);
		GUI["17"]["PaddingBottom"] = UDim.new(0, 8);

		-- StarterGui.MyLibrary.Main.Navigation.ButtonHolder.UIListLayout
		GUI["18"] = Instance.new("UIListLayout", GUI["16"]);
		GUI["18"]["Padding"] = UDim.new(0, 1);
		GUI["18"]["SortOrder"] = Enum.SortOrder.LayoutOrder;
		-- StarterGui.MyLibrary.Main.Navigation.Line
		GUI["1b"] = Instance.new("Frame", GUI["10"]);
		GUI["1b"]["BorderSizePixel"] = 0;
		GUI["1b"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		GUI["1b"]["BackgroundTransparency"] = 1;
		GUI["1b"]["Size"] = UDim2.new(0, 1, 1, 0);
		GUI["1b"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		GUI["1b"]["Position"] = UDim2.new(1, 0, 0, 0);
		
		-- StarterGui.MyLibrary.Main.TopBar.TextBox.LocalScript
		

	end

	function GUI:CreateTab(options)
		options = Library:validate({
			name = "Preview Tab"
		}, options or {})

		local Tab = {
			Hover = false,
			Active = false
			
		}
		
		-- Render
		do
			Tab["1a"] = Instance.new("TextLabel", GUI["16"])
			Tab["1a"].TextWrapped = true
			Tab["1a"].BorderSizePixel = 0
			Tab["1a"].BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			Tab["1a"].Font = Enum.Font.GothamBold
			Tab["1a"].TextSize = 15
			Tab["1a"].TextColor3 = Color3.fromRGB(109, 109, 109)
			Tab["1a"].Size = UDim2.new(1, 0, 0, 35)
			Tab["1a"].BorderColor3 = Color3.fromRGB(0, 0, 0)
			Tab["1a"].Text = options.name
			Tab["1a"].Name = "Inactive"
			Tab["1a"].BackgroundTransparency = 1
			
			-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab
			Tab["1e"] = Instance.new("ScrollingFrame", GUI["1a"]);
			Tab["1e"]["Active"] = true;
			Tab["1e"]["BorderSizePixel"] = 0;
			Tab["1e"]["CanvasSize"] = UDim2.new(0, 0, 0, 559);
			Tab["1e"]["ElasticBehavior"] = Enum.ElasticBehavior.Always;
			Tab["1e"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
			Tab["1e"]["VerticalScrollBarInset"] = Enum.ScrollBarInset.ScrollBar;
			Tab["1e"]["BackgroundTransparency"] = 1;
			Tab["1e"]["Size"] = UDim2.new(-0.02277432754635811, 470, 1, 49);
			Tab["1e"]["ScrollBarImageColor3"] = Color3.fromRGB(0, 0, 0);
			Tab["1e"]["ClipsDescendants"] = false;
			Tab["1e"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
			Tab["1e"]["ScrollBarThickness"] = 0;
			Tab["1e"]["Position"] = UDim2.new(0, 9, 0, 19);
			Tab["1e"]["Name"] = [[HomeTab]];
			Tab["1e"]["Visible"] = false
			

			
			-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.UIListLayout
			Tab["29"] = Instance.new("UIListLayout", Tab["1e"]);
			Tab["29"]["Padding"] = UDim.new(0, 19);
			Tab["29"]["SortOrder"] = Enum.SortOrder.LayoutOrder;

		end
	
		-- Methods
		
		
		function Tab:Deactivate()
			if Tab.Active then
				Tab.Active = false
				Tab.Hover = false
				Library:tween(Tab["1a"], {TextColor3 = Color3.fromRGB(108, 108, 108)})
			end	
			if GUI.CurrentTab == nil then
				Tab.Active()
				Tab["1d"]["Visible"] = false
			end
		end	
		-- Logic
		do
			Tab["1a"].MouseEnter:Connect(function()
				Tab.Hover = true

				if not Tab.Active then
					Library:tween(Tab["1a"], {TextColor3 = Color3.fromRGB(189, 189, 189)})
				end
			end)

			Tab["1a"].MouseLeave:Connect(function()
				Tab.Hover = false

				if not Tab.Active then
					Library:tween(Tab["1a"], {TextColor3 = Color3.fromRGB(108, 108, 108)})
				end
			end)


			uis.InputBegan:Connect(function(input)

				if input.UserInputType == Enum.UserInputType.MouseButton1 then
					if Tab.Hover then
						Tab:Activate()
					end
				end
			end)
		
		
			function Tab:Activate()
				if not Tab.Active then
					if GUI.CurrentTab ~= nil then
						GUI.CurrentTab:Deactivate()
						local currentTabGoal = {}
						currentTabGoal.Position = UDim2.new(0, 9, -3, 19)  -- Yeni tabın başlangıç pozisyonu
						local currentTabTweenInfo = TweenInfo.new(1)
						local currentTabTween = tweenService:Create(GUI.CurrentTab["1e"], currentTabTweenInfo, currentTabGoal)
						currentTabTween:Play()
					end

					local newTabGoal = {}
					newTabGoal.Position = UDim2.new(0, 9, 0, 19)  -- Yeni tabın hedef pozisyonu
					local newTabTweenInfo = TweenInfo.new(1)
					local newTabTween = tweenService:Create(Tab["1e"], newTabTweenInfo, newTabGoal)
					newTabTween:Play()

					Tab["1e"].Visible = true
					Tab.Active = true
					Library:tween(Tab["1a"], {TextColor3 = Color3.fromRGB(189, 189, 189)})
					GUI.CurrentTab = Tab
				end

				-- Mevcut sekmenin görünürlüğünü kapat
				if GUI.CurrentTab ~= nil and GUI.CurrentTab ~= Tab then
					GUI.CurrentTab:Deactivate()
				end
			end
		
		-- Logic
	do
			Tab["1a"].MouseEnter:Connect(function()
				Tab.Hover = true

				if not Tab.Active then
					Library:tween(Tab["1a"], {TextColor3 = Color3.fromRGB(189, 189, 189)})
				end
			end)

			Tab["1a"].MouseLeave:Connect(function()
				Tab.Hover = false

				if not Tab.Active then
					Library:tween(Tab["1a"], {TextColor3 = Color3.fromRGB(108, 108, 108)})
				end
			end)
				
			end
			
			

			uis.InputBegan:Connect(function(input)

				if input.UserInputType == Enum.UserInputType.MouseButton1 then
					if Tab.Hover then
						Tab:Activate()
					end
				end
			end)
		end
		
		function Tab:Button(options)
			options = Library:validate({
				name = "Preview Button",
				callback = function() end
			}, options or {})

			local Button = {
				options.callback,
				Hover = false,
				MouseDown = false,
			}
			
			--render
			do
				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Button
				Button["1f"] = Instance.new("Frame", Tab["1e"]);
				Button["1f"]["BackgroundColor3"] = Color3.fromRGB(46, 46, 46);
				Button["1f"]["AnchorPoint"] = Vector2.new(1, 0);
				Button["1f"]["Size"] = UDim2.new(1, 0, 0, 30);
				Button["1f"]["BorderColor3"] = Color3.fromRGB(246, 3, 3);
				Button["1f"]["Position"] = UDim2.new(1, -1, 0, 8);
				Button["1f"]["Name"] = [[Button]];

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Button.UIStroke
				Button["20"] = Instance.new("UIStroke", Button["1f"]);
				Button["20"]["Color"] = Color3.fromRGB(246, 3, 3);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Button.UICorner
				Button["21"] = Instance.new("UICorner", Button["1f"]);
				Button["21"]["CornerRadius"] = UDim.new(0, 5);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Button.Title
				Button["22"] = Instance.new("TextLabel", Button["1f"]);
				Button["22"]["BorderSizePixel"] = 0;
				Button["22"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Button["22"]["FontFace"] = Font.new([[rbxasset://fonts/families/GothamSSm.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
				Button["22"]["TextSize"] = 16;
				Button["22"]["TextColor3"] = Color3.fromRGB(214, 214, 214);
				Button["22"]["Size"] = UDim2.new(0, 0, 0, 0);
				Button["22"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Button["22"]["Text"] = options.name;
				Button["22"]["Name"] = [[Title]];
				Button["22"]["BackgroundTransparency"] = 1;
				Button["22"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);

			end
			
			--method
			
			function Button:SetText(text)
				Button["22"].Text = text
				options.name = text
			end
			
			
			--logic
			
			do
				Button["1f"].InputBegan:Connect(function()
					Button.Hover = true
					
					if not Button.MouseDown then
						Library:tween(Button["1f"], {BackgroundColor3 = Color3.fromRGB(42, 42, 42)} )
					end
				end)
			end
			
			
			Button["1f"].InputEnded:Connect(function()
				Button.Hover = false
				if not Button.MouseDown then
					Library:tween(Button["1f"], {BackgroundColor3 = Color3.fromRGB(45, 45, 45)} )
				end
			end)
			
			local isMouseDown = false
			
			Button["1f"].InputBegan:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseButton1 then
					Button["1f"]:TweenSize(UDim2.new(1, 0,-0.007, 30), Enum.EasingDirection.InOut, Enum.EasingStyle.Quint, 0.2, true)
					isMouseDown = true
				end
			end)
			
			Button["1f"].InputEnded:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseButton1 and isMouseDown then
					Button["1f"]:TweenSize(UDim2.new(1, 0, 0, 30), Enum.EasingDirection.InOut, Enum.EasingStyle.Quint, 0.2, true)
					isMouseDown = false
					options.callback()
				end
			end)
			
			return Button
		end
		
		
		
		function Tab:Label(options)
			options = Library:validate({
				message = "Text Here",
				callback = function() end
			}, options or {})
			
			local Label = {}
			
			-- render
			
			do
				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Label
				Label["23"] = Instance.new("Frame", Tab["1e"]);
				Label["23"]["BackgroundColor3"] = Color3.fromRGB(46, 46, 46);
				Label["23"]["AnchorPoint"] = Vector2.new(1, 0);
				Label["23"]["BackgroundTransparency"] = 1;
				Label["23"]["Size"] = UDim2.new(1, 0, 0, 30);
				Label["23"]["BorderColor3"] = Color3.fromRGB(246, 3, 3);
				Label["23"]["Position"] = UDim2.new(1, -14, 0, 8);
				Label["23"]["Name"] = [[Label]];

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Label.Title
				Label["24"] = Instance.new("TextLabel", Label["23"]);
				Label["24"]["BorderSizePixel"] = 0;
				Label["24"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Label["24"]["FontFace"] = Font.new([[rbxasset://fonts/families/GothamSSm.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
				Label["24"]["TextSize"] = 16;
				Label["24"]["TextColor3"] = Color3.fromRGB(214, 214, 214);
				Label["24"]["Size"] = UDim2.new(1, 0, 1, 0);
				Label["24"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Label["24"]["Text"] = options.message;
				Label["24"]["Name"] = [[Title]];
				Label["24"]["BackgroundTransparency"] = 1;
				

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Label.ImageLabel1
				Label["25"] = Instance.new("ImageLabel", Label["23"]);
				Label["25"]["BorderSizePixel"] = 0;
				Label["25"]["BackgroundColor3"] = Color3.fromRGB(246, 3, 3);
				Label["25"]["ImageColor3"] = Color3.fromRGB(246, 3, 3);
				Label["25"]["Image"] = [[rbxassetid://5526266602]];
				Label["25"]["Size"] = UDim2.new(0, 110, 0, 2);
				Label["25"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Label["25"]["Name"] = [[ImageLabel1]];
				Label["25"]["Position"] = UDim2.new(0, 0, 0.5, 0);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Label.ImageLabel1.UICorner
				Label["26"] = Instance.new("UICorner", Label["25"]);


				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Label.ImageLabel2
				Label["27"] = Instance.new("ImageLabel", Label["23"]);
				Label["27"]["BorderSizePixel"] = 0;
				Label["27"]["BackgroundColor3"] = Color3.fromRGB(246, 3, 3);
				Label["27"]["ImageColor3"] = Color3.fromRGB(246, 3, 3);
				Label["27"]["Image"] = [[rbxassetid://5526266602]];
				Label["27"]["Size"] = UDim2.new(0, 110, 0, 2);
				Label["27"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Label["27"]["Name"] = [[ImageLabel2]];
				Label["27"]["Position"] = UDim2.new(1, -110, 0.5, 0);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Label.ImageLabel2.UICorner
				Label["28"] = Instance.new("UICorner", Label["27"]);
			end
			
			-- methods 
			
			function Label:SetText(text)
				options.message = text
				Label["24"].Text = text
			
			end
			
			return Label
			
		end
		
		function Tab:Toggle(options)
			options = Library:validate({
				title = "Prewiev Toggle",
				callback = function() end
			}, options or 	{})
			
			
			local Toggle = {
				Hover = false,
				MouseDown = false,
				State = false 
			}
			
			
			
			
			-- Render
			
			
			do
				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.ToggleInactive
				Toggle["40"] = Instance.new("Frame", Tab["1e"]);
				Toggle["40"]["BackgroundColor3"] = Color3.fromRGB(46, 46, 46);
				Toggle["40"]["AnchorPoint"] = Vector2.new(1, 0);
				Toggle["40"]["Size"] = UDim2.new(1, 0, 0, 30);
				Toggle["40"]["BorderColor3"] = Color3.fromRGB(246, 3, 3);
				Toggle["40"]["Position"] = UDim2.new(1, -14, 0, 8);
				Toggle["40"]["Name"] = [[ToggleInactive]];
				

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.ToggleInactive.UIStroke
				Toggle["41"] = Instance.new("UIStroke", Toggle["40"]);
				Toggle["41"]["Color"] = Color3.fromRGB(246, 3, 3);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.ToggleInactive.UICorner
				Toggle["42"] = Instance.new("UICorner", Toggle["40"]);
				Toggle["42"]["CornerRadius"] = UDim.new(0, 5);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.ToggleInactive.Title
				Toggle["43"] = Instance.new("TextLabel", Toggle["40"]);
				Toggle["43"]["BorderSizePixel"] = 0;
				Toggle["43"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Toggle["43"]["FontFace"] = Font.new([[rbxasset://fonts/families/GothamSSm.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
				Toggle["43"]["TextSize"] = 16;
				Toggle["43"]["TextColor3"] = Color3.fromRGB(214, 214, 214);
				Toggle["43"]["Size"] = UDim2.new(0, 0, 0, 0);
				Toggle["43"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Toggle["43"]["Text"] = options.title;
				Toggle["43"]["Name"] = [[Title]];
				Toggle["43"]["BackgroundTransparency"] = 1;
				Toggle["43"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.ToggleInactive.CheckmarkHolder
				Toggle["44"] = Instance.new("Frame", Toggle["40"]);
				Toggle["44"]["BorderSizePixel"] = 0;
				Toggle["44"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Toggle["44"]["AnchorPoint"] = Vector2.new(1, 0);
				Toggle["44"]["BackgroundTransparency"] = 1;
				Toggle["44"]["Size"] = UDim2.new(1, 0, 1, 0);
				Toggle["44"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Toggle["44"]["Position"] = UDim2.new(1, 0, 0, 0);
				Toggle["44"]["Name"] = [[CheckmarkHolder]];

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.ToggleInactive.CheckmarkHolder.Toggle
				Toggle["45"] = Instance.new("ImageLabel", Toggle["40"]);
				Toggle["45"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
				Toggle["45"]["ScaleType"] = Enum.ScaleType.Slice;
				Toggle["45"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Toggle["45"]["SliceScale"] = 0.11999999731779099;
				Toggle["45"]["Image"] = [[rbxassetid://3570695787]];
				Toggle["45"]["Size"] = UDim2.new(0, 50, 0, 23);
				Toggle["45"]["Name"] = [[Toggle]];
				Toggle["45"]["BackgroundTransparency"] = 1;
				Toggle["45"]["Position"] = UDim2.new(0.956, -40,0.5, -13);
				Toggle["45"]["ZIndex"] = "-10"


				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.ToggleInactive.CheckmarkHolder.Toggle.Button
				Toggle["46"] = Instance.new("TextButton", Toggle["45"]);
				Toggle["46"]["TextTransparency"] = 1;
				Toggle["46"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Toggle["46"]["TextSize"] = 14;
				Toggle["46"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
				Toggle["46"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
				Toggle["46"]["Size"] = UDim2.new(1, 0, 1, 0);
				Toggle["46"]["Name"] = [[Button]];
				Toggle["46"]["BackgroundTransparency"] = 1;

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.ToggleInactive.CheckmarkHolder.Toggle.Circle
				Toggle["47"] = Instance.new("ImageLabel", Toggle["45"]);
				Toggle["47"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
				Toggle["47"]["ScaleType"] = Enum.ScaleType.Slice;
				Toggle["47"]["BackgroundColor3"] = Color3.fromRGB(246, 3, 3);
				Toggle["47"]["ImageColor3"] = Color3.fromRGB(246, 3, 3);
				Toggle["47"]["SliceScale"] = 0.11999999731779099;
				Toggle["47"]["Image"] = [[rbxassetid://3570695787]];
				Toggle["47"]["Size"] = UDim2.new(0, 21, 0, 21);
				Toggle["47"]["Name"] = [[Circle]];
				Toggle["47"]["BackgroundTransparency"] = 1;
				Toggle["47"]["Position"] = UDim2.new(0, 2, 0, 1);
				Toggle["47"]["ZIndex"] = "0"
			end
			


			--Methods 
			do
				function Toggle:Toggle(b)
					if b == nil then
						Toggle.State = not Toggle.State
					else
						Toggle.State = b
					end
					
					if Toggle.State then
						Toggle["47"]:TweenPosition(UDim2.new(0, 28, 0, 1), Enum.EasingDirection.InOut, Enum.EasingStyle.Quint, 0.2, true)
						
					else
						Toggle["47"]:TweenPosition(UDim2.new(0, 2, 0, 1), Enum.EasingDirection.InOut, Enum.EasingStyle.Quint, 0.2, true)
					end
					
					options.callback(Toggle.State)
				end
			end

			
			
			--logic

			do
				Toggle["45"].InputBegan:Connect(function()
					Toggle.Hover = true

					if not Toggle.MouseDown then
						
					end
				end)
			end


			Toggle["47"].InputEnded:Connect(function()
				Toggle.Hover = false
				if not Toggle.MouseDown then
					
				end
			end)

			local isMouseDown = false

			Toggle["44"].InputBegan:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseButton1 then
					if isMouseDown then
						Toggle["47"]:TweenPosition(UDim2.new(0, 2, 0, 1), Enum.EasingDirection.InOut, Enum.EasingStyle.Quint, 0.2, true)
					else
						Toggle["47"]:TweenPosition(UDim2.new(0, 28, 0, 1), Enum.EasingDirection.InOut, Enum.EasingStyle.Quint, 0.2, true)
					end

					isMouseDown = not isMouseDown
					Toggle:Toggle()
					
				end
			end)
			return Toggle
		end
		
		function Tab:Slider(options)
			options = Library:validate({
				title = "Preview slider",
				min = 0,
				max = 100,
				default = 1,
				callback = function(v) print(v) end
				

			}, options or {})
			
			local Slider = {
				MouseDown = false,
				Hover = false,
				Connection = nil
			}
			
			
			--render
			do
				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Slider
				Slider["2a"] = Instance.new("Frame", Tab["1e"]);
				Slider["2a"]["BackgroundColor3"] = Color3.fromRGB(46, 46, 46);
				Slider["2a"]["AnchorPoint"] = Vector2.new(1, 0);
				Slider["2a"]["Size"] = UDim2.new(1, 0, 0, 50);
				Slider["2a"]["BorderColor3"] = Color3.fromRGB(246, 3, 3);
				Slider["2a"]["Position"] = UDim2.new(1, -14, 0, 8);
				Slider["2a"]["Name"] = [[Slider]];

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.UIStroke
				Slider["2b"] = Instance.new("UIStroke", Slider["2a"]);
				Slider["2b"]["Color"] = Color3.fromRGB(246, 3, 3);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.UICorner
				Slider["2c"] = Instance.new("UICorner", Slider["2a"]);
				Slider["2c"]["CornerRadius"] = UDim.new(0, 5);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.Title
				Slider["2d"] = Instance.new("TextLabel", Slider["2a"]);
				Slider["2d"]["BorderSizePixel"] = 0;
				Slider["2d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Slider["2d"]["TextXAlignment"] = Enum.TextXAlignment.Left;
				Slider["2d"]["FontFace"] = Font.new([[rbxasset://fonts/families/GothamSSm.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
				Slider["2d"]["TextSize"] = 16;
				Slider["2d"]["TextColor3"] = Color3.fromRGB(214, 214, 214);
				Slider["2d"]["Size"] = UDim2.new(0, 60, 0, 25);
				Slider["2d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Slider["2d"]["Text"] = options.title ;
				Slider["2d"]["Name"] = [[Title]];
				Slider["2d"]["BackgroundTransparency"] = 1;

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.Title.UIPadding
				Slider["2e"] = Instance.new("UIPadding", Slider["2d"]);
				Slider["2e"]["PaddingLeft"] = UDim.new(0, 16);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.Value
				Slider["2f"] = Instance.new("TextLabel", Slider["2a"]);
				Slider["2f"]["BorderSizePixel"] = 0;
				Slider["2f"]["BackgroundColor3"] = Color3.fromRGB(46, 46, 46);
				Slider["2f"]["FontFace"] = Font.new([[rbxasset://fonts/families/GothamSSm.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
				Slider["2f"]["TextColor3"] = Color3.fromRGB(214, 214, 214);
				Slider["2f"]["Size"] = UDim2.new(0, 70, 0, 16);
				Slider["2f"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Slider["2f"]["Text"] = tostring(options.default);
				Slider["2f"]["Name"] = [[Value]];
				Slider["2f"]["Position"] = UDim2.new(0, 380, 0, 5);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.Value.UICorner
				Slider["30"] = Instance.new("UICorner", Slider["2f"]);
				Slider["30"]["CornerRadius"] = UDim.new(0, 4);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.Value.UIStroke
				Slider["31"] = Instance.new("UIStroke", Slider["2f"]);
				Slider["31"]["Color"] = Color3.fromRGB(246, 3, 3);
				Slider["31"]["ApplyStrokeMode"] = Enum.ApplyStrokeMode.Border;

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.SliderBack
				Slider["32"] = Instance.new("Frame", Slider["2a"]);
				Slider["32"]["BorderSizePixel"] = 0;
				Slider["32"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
				Slider["32"]["AnchorPoint"] = Vector2.new(0, 1);
				Slider["32"]["Size"] = UDim2.new(0, 440, 0, 6);
				Slider["32"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Slider["32"]["Position"] = UDim2.new(0, 10, 0, 40);
				Slider["32"]["Name"] = [[SliderBack]];

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.SliderBack.Draggable
				Slider["33"] = Instance.new("Frame", Slider["32"]);
				Slider["33"]["BorderSizePixel"] = 0;
				Slider["33"]["BackgroundColor3"] = Color3.fromRGB(246, 3, 3);
				Slider["33"]["Size"] = UDim2.new(0.5, 0, 1, 0);
				Slider["33"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Slider["33"]["Name"] = [[Draggable]];

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.SliderBack.Draggable.UICorner
				Slider["34"] = Instance.new("UICorner", Slider["33"]);


				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.SliderBack.Draggable.ImageLabel
				Slider["35"] = Instance.new("ImageLabel", Slider["33"]);
				Slider["35"]["BorderSizePixel"] = 0;
				Slider["35"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Slider["35"]["Image"] = [[rbxassetid://5552526748]];
				Slider["35"]["Size"] = UDim2.new(0, 10, 0, 10);
				Slider["35"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Slider["35"]["BackgroundTransparency"] = 1;
				Slider["35"]["Position"] = UDim2.new(1, -3, 0, -2);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeSlider.Slider.SliderBack.UICorner
				Slider["36"] = Instance.new("UICorner", Slider["32"]);
			end
			
			
			
			--methods
			
			--methods
			function Slider:SetValue(v)
				if v == nil then
					local percentage = math.clamp((mouse.X - Slider["32"].AbsolutePosition.X) / Slider["32"].AbsoluteSize.X, 0, 1)
					local value = math.floor(((options.max - options.min) * percentage) + options.min)

					Slider["2f"].Text = tostring(value)
					Slider["33"].Size = UDim2.new(percentage, 0, 1, 0)
					options.callback(value)
				else
					Slider["2f"].Text = tostring(v)
					local percentage = (v - options.min) / (options.max - options.min)
					Slider["33"].Size = UDim2.new(percentage, 0, 1, 0)
					options.callback(v)
				end
			end

			function Slider:GetValue()
				return tonumber(Slider["2f"].Text)
			end


			
			-- Logic

			local isMouseDown = false
			local lastPrintTime = tick()

			do
				Slider["2a"].MouseEnter:Connect(function()
					Slider.Hover = true

					if not isMouseDown then
						Library:tween(Slider["33"], {BackgroundColor3 = Color3.fromRGB(132, 1, 1)})
					end
				end)

				Slider["2a"].MouseLeave:Connect(function()
					Slider.Hover = false

					if not isMouseDown then
						Library:tween(Slider["33"], {BackgroundColor3 = Color3.fromRGB(246, 3, 3)})
					end
				end)


				uis.InputBegan:Connect(function(input)

					
					
					if input.UserInputType == Enum.UserInputType.MouseButton1 and Slider.Hover then
						Slider.MouseDown = true
						
						if not Slider.Connection then
							Slider.Connection = runService.RenderStepped:Connect(function()
								Slider:SetValue()
							end)
						end
					end
				end)

							
							


				uis.InputEnded:Connect(function(input)
					if input.UserInputType == Enum.UserInputType.MouseButton1 then
						isMouseDown = false
						Library:tween(Slider["33"], {BackgroundColor3 = Color3.fromRGB(246, 3, 3)})
						
						
						if Slider.Connection then Slider.Connection:Disconnect() end
							Slider.Connection = nil
						end
					end)
				end
			

			
			return Slider
		end
		
		
		function Tab:Dropdown(options)
			options = Library:validate({
				title = "Preview Dropdown",
				callback = function(v) print(v) end,
				items = {}
				
			}, options or {})
			
			local Dropdown = {
				Items = {
					["id"] = {
						"value"
					}
				},
				Open = false,
				MouseDown = false,
				Hover = false,
				HoveringItem = false
			}
			
			-- Render
			
			local selectedText = "" -- Seçilen 3D öğesinin metni için bir değişken
			
			local function UpdateSelectedText(newText)
				selectedText = newText
				Dropdown["39"].Text = options.title .. " : " .. selectedText -- Dropdown metnini güncelle
			end
			do
				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Dropdown
				Dropdown["37"] = Instance.new("Frame", Tab["1e"]);
				Dropdown["37"]["BackgroundColor3"] = Color3.fromRGB(46, 46, 46);
				Dropdown["37"]["AnchorPoint"] = Vector2.new(1, 0);
				Dropdown["37"]["Size"] = UDim2.new(1, 0, 0, 34);
				Dropdown["37"]["BorderColor3"] = Color3.fromRGB(246, 3, 3);
				Dropdown["37"]["Position"] = UDim2.new(1, -14, 0, 8);
				Dropdown["37"]["Name"] = [[Dropdown]];

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Dropdown.UICorner
				Dropdown["38"] = Instance.new("UICorner", Dropdown["37"]);
				Dropdown["38"]["CornerRadius"] = UDim.new(0, 5);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Dropdown.Title
				Dropdown["39"] = Instance.new("TextLabel", Dropdown["37"]);
				Dropdown["39"]["BorderSizePixel"] = 0;
				Dropdown["39"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Dropdown["39"]["FontFace"] = Font.new([[rbxasset://fonts/families/GothamSSm.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
				Dropdown["39"]["TextSize"] = 16;
				Dropdown["39"]["TextColor3"] = Color3.fromRGB(214, 214, 214);
				Dropdown["39"]["Size"] = UDim2.new(1, -20, 0, 20);
				Dropdown["39"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Dropdown["39"]["Text"] = options.title .. ": " .. selectedText
				Dropdown["39"]["Name"] = [[Title]];
				Dropdown["39"]["BackgroundTransparency"] = 1;

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Dropdown.ImageLabel
				Dropdown["3a"] = Instance.new("ImageLabel", Dropdown["37"]);
				Dropdown["3a"]["BorderSizePixel"] = 0;
				Dropdown["3a"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Dropdown["3a"]["Image"] = [[rbxassetid://5279719038]];
				Dropdown["3a"]["Size"] = UDim2.new(0, 15, 0, 15);
				Dropdown["3a"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Dropdown["3a"]["BackgroundTransparency"] = 1;
				Dropdown["3a"]["Position"] = UDim2.new(1, -25, 0, 10);

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Dropdown.OptionHolder
				Dropdown["3b"] = Instance.new("ScrollingFrame", Dropdown["37"]);
				Dropdown["3b"]["ScrollingDirection"] = Enum.ScrollingDirection.Y;
				Dropdown["3b"]["BorderSizePixel"] = 0;
				Dropdown["3b"]["MidImage"] = [[rbxassetid://5552526748]];
				Dropdown["3b"]["ElasticBehavior"] = Enum.ElasticBehavior.Always;
				Dropdown["3b"]["TopImage"] = [[]];
				Dropdown["3b"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
				Dropdown["3b"]["VerticalScrollBarInset"] = Enum.ScrollBarInset.ScrollBar;
				Dropdown["3b"]["BackgroundTransparency"] = 1;
				Dropdown["3b"]["Size"] = UDim2.new(1, 0, 1, -28);
				Dropdown["3b"]["Selectable"] = false;
				Dropdown["3b"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Dropdown["3b"]["ScrollBarThickness"] = 8;
				Dropdown["3b"]["Position"] = UDim2.new(0, 0, 0, 26);
				Dropdown["3b"]["Visible"] = false;
				Dropdown["3b"]["Name"] = [[OptionHolder]];
				Dropdown["3b"]["BottomImage"] = [[]];
				Dropdown["3b"]["SelectionGroup"] = false;

				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Dropdown.OptionHolder.UIListLayout
				Dropdown["3c"] = Instance.new("UIListLayout", Dropdown["3b"]);
				Dropdown["3c"]["Padding"] = UDim.new(0, 6);
				Dropdown["3c"]["SortOrder"] = Enum.SortOrder.LayoutOrder;

			end
			
			--test
			

			
			-- method
			
			local  Item = {
				Hover = false,
				MouseDown = false
			}			
			
			function Dropdown:Add(id, value)
				
				if Dropdown.Items[id] ~= nil then
					return
				end
				
				Dropdown.Items[id] = {
					instance = {},
					value = value
				}
				Dropdown.Items[id].instance = {}
				
				Dropdown.Items[id].value = value
				-- StarterGui.MyLibrary.Main.ContentContainer.HomeTab.Dropdown.OptionHolder.Inactive
				Dropdown.Items[id].instance["3d"] = Instance.new("TextLabel", Dropdown["3b"]);
				Dropdown.Items[id].instance["3d"]["BorderSizePixel"] = 0;
				Dropdown.Items[id].instance["3d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
				Dropdown.Items[id].instance["3d"]["FontFace"] = Font.new([[rbxasset://fonts/families/GothamSSm.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
				Dropdown.Items[id].instance["3d"]["TextSize"] = 16;
				Dropdown.Items[id].instance["3d"]["TextColor3"] = Color3.fromRGB(166, 166, 166);
				Dropdown.Items[id].instance["3d"]["Size"] = UDim2.new(1, -20, 0, 20);
				Dropdown.Items[id].instance["3d"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
				Dropdown.Items[id].instance["3d"]["Text"] = id;
				Dropdown.Items[id].instance["3d"]["Name"] = [[Inactive]];
				Dropdown.Items[id].instance["3d"]["BackgroundTransparency"] = 1;
				
				function SetAllLabelsGray()
					for _, item in pairs(Dropdown.Items) do
						item.instance["3d"].TextColor3 = Color3.fromRGB(166, 166, 166)
					end
				end

				
				Dropdown.Items[id].instance["3d"].MouseEnter:Connect(function()
					Item.Hover = true
					Dropdown.HoveringItem = true

				end)

				Dropdown.Items[id].instance["3d"].MouseLeave:Connect(function()
					Item.Hover = false
					Dropdown.HoveringItem = false

					if not Item.MouseDown then
					end
				end)
				

				
				
				Dropdown.Items[id].instance["3d"].InputBegan:Connect(function(input, gpe)
					if gpe then return end

					if Dropdown.Items[id] == nil then return end

					if input.UserInputType == Enum.UserInputType.MouseButton1 and Item.Hover then
						Item.MouseDown = true

						-- Diğer 3D'lerin rengini gri yap
						SetAllLabelsGray()

						-- Rengi beyaz yap
						Dropdown.Items[id].instance["3d"].TextColor3 = Color3.fromRGB(255, 255, 255)

						options.callback(value)

						if not Dropdown.HoveringItem then
							Dropdown:Toggle()
						end
					end
				end)






				Dropdown.Items[id].instance["3d"].InputEnded:Connect(function(input, gpe)
					if gpe then return end
					
					if  Dropdown.Items[id] == nil  then return end
					
					if input.UserInputType == Enum.UserInputType.MouseButton1 then

						Dropdown.MouseDown = false

						if Item.Hover then
							Library:tween(Dropdown.Items[id].instance["3d"], {TextColor3 = Color3.fromRGB(253, 253, 253)})
						else
							Library:tween(Dropdown.Items[id].instance["3d"], {TextColor3 = Color3.fromRGB(166, 166, 166)})

						end

					end
				end)
				
			end
			
			
			do
			function Dropdown:Remove(id)
				if Dropdown.Items[id] ~= nil then
						
						if Dropdown.Items[id].instance ~= nil then
							for i, v in pairs(Dropdown.Items[id].instance) do
								v:Destroy()
							end
						end
					
					Dropdown.Items[id] = nil
				end
			end
			
			function Dropdown:Clear()
				for i, v in pairs(Dropdown.Items) do
					Dropdown:Remove(i)
				end
			end
			
			
				function Dropdown:Toggle()
					local targetRotation = Dropdown.Open and 0 or 180 -- Hedef rotasyon değeri (derece cinsinden)
					local tweenInfo = TweenInfo.new(0.2, Enum.EasingStyle.Quint, Enum.EasingDirection.InOut) -- Tweening ayarları

					if Dropdown.Open then
						Library:tween(Dropdown["37"], {Size = UDim2.new(1, 0, 0, 34)}, function() 
							Dropdown["3b"].Visible = false
						end)
					else
						local count = 0
						for i, v in pairs(Dropdown.Items) do
							if v ~= nil then
								count += 1
							end
						end
						Dropdown["3b"].Visible = true
						Library:tween(Dropdown["37"], {Size = UDim2.new(1, 0, 0, 20 + (count * 20) + 52)})
					end

					local tween = game:GetService("TweenService"):Create(Dropdown["3a"], tweenInfo, {Rotation = targetRotation})
					tween:Play()
					Dropdown.Open = not Dropdown.Open
				end

		
			
			-- Logic
			do
				Dropdown["37"].InputBegan:Connect(function()
					Dropdown.Hover = true

					if not Dropdown.MouseDown then
							Library:tween(Dropdown["37"], {BackgroundColor3 = Color3.fromRGB(45, 45, 45)} )
					end
				end)
			end


			Dropdown["37"].InputEnded:Connect(function()
				Dropdown.Hover = false
				if not Dropdown.MouseDown then
						Library:tween(Dropdown["37"], {BackgroundColor3 = Color3.fromRGB(45, 45, 45)} )
				end
			end)

			local isMouseDown = false

			Dropdown["37"].InputBegan:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseButton1 then
						isMouseDown = true
				end
			end)

			Dropdown["37"].InputEnded:Connect(function(input)
				if input.UserInputType == Enum.UserInputType.MouseButton1 and isMouseDown then
						isMouseDown = false
						Dropdown:Toggle()
					end
				end)
				
				
			end
			
			return Dropdown
		end
		
		return Tab
	end

	return GUI
end














