-- Made by Impulse https://youtube.com/c/ImpulseExploits

uis = game:GetService("UserInputService")

game:GetService("RunService").RenderStepped:Connect(function()

	for i, plr in pairs(game.Players:GetChildren()) do		if plr ~= game.Players.LocalPlayer then

			if plr.Character:FindFirstChild("Humanoid") then

				if plr.Character.Humanoid.Health>0 then

					if plr.Character.Head:FindFirstChild("BillboardGui") then

						if plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("d") then

							if plr.TeamColor == game.Players.LocalPlayer.TeamColor then

								plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("d").TextColor3 = Color3.new(0.180392, 1, 0)

								plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("name").TextColor3 = Color3.new(0.180392, 1, 0)

								plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("square").TextColor3 = Color3.new(0.180392, 1, 0)

							else

								plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("d").TextColor3 = Color3.new(1, 0, 0.0156863)

								plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("name").TextColor3 = Color3.new(1, 0, 0.0156863)

								plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("square").TextColor3 = Color3.new(1, 0, 0.0156863)

							end

							if plr.Character.Head.Velocity.Magnitude<5 then

								if plr.Character.Head.Velocity.Magnitude<0.4 then

									plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("d").Text = "Not Moving"

								else

									plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("d").Text = "Moving Slowly"

								end

							else

								plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("d").Text = "Moving"

							end

						end

						if plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("name") then

							plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("name").Text = (plr.Name)

						end

						if plr.Character.Head.Velocity.Magnitude<1.2 then

							for i, plro in pairs(game.Players:GetChildren()) do

								if plro ~= plr then

									if plro.Character:FindFirstChild("Head") then

										

									if (plr.Character.Head.Position - plro.Character.Head.Position).Magnitude<7 then

											if game.Workspace:FindFirstChild("Epos") then

												if plr.Character:FindFirstChild("Humanoid") then

													if plr.Character.Humanoid.Health>0 then

													else

														game.Workspace:FindFirstChild("Epos"):Destroy()

													end

												else

													game.Workspace:FindFirstChild("Epos"):Destroy()

												end

												if plro.Character:FindFirstChild("Humanoid") then

													if plro.Character.Humanoid.Health>0 then

													else

														game.Workspace:FindFirstChild("Epos"):Destroy()

													end

												else

													game.Workspace:FindFirstChild("Epos"):Destroy()

												end

												if plr.TeamColor ~= game.Players.LocalPlayer.TeamColor then

													game.Workspace:FindFirstChild("Epos").Position = (plr.Character.Head.Position + plro.Character.Head.Position)/2

													end

										else

												if plro.Character.Head.Velocity.Magnitude<3 then

													if plr.TeamColor ~= game.Players.LocalPlayer.TeamColor then

											local e = Instance.new("Part")

											e.Parent = game.Workspace

											e.Anchored = true

											e.Transparency = 1

											e.CanCollide = false

											e.Name = "Epos"

											e.Position = (plr.Character.Head.Position + plro.Character.Head.Position)/2

											local a = Instance.new("BillboardGui")

											a.Parent = e

											a.Size = UDim2.new(3,0,3,0)

											a.AlwaysOnTop = true

											local f = Instance.new("TextLabel")

											f.Parent = a

												f.Size = UDim2.new(1,0,1,0)

												f.TextColor3 = Color3.new(1, 1, 0)

												f.TextStrokeTransparency = 0.5

											f.Text = ""

											f.BackgroundTransparency = 1

											f.TextScaled = true

											f.Name = "es"

														f.Position = UDim2.new(0,0,-0.7,0)

														if plr.Character:FindFirstChild("Humanoid") then

															if plr.Character.Humanoid.Health>0 then

															else

																game.Workspace:FindFirstChild("Epos"):Destroy()

															end

														else

															game.Workspace:FindFirstChild("Epos"):Destroy()

														end

														if plro.Character:FindFirstChild("Humanoid") then

															if plro.Character.Humanoid.Health>0 then

															else

																game.Workspace:FindFirstChild("Epos"):Destroy()

															end

														else

															game.Workspace:FindFirstChild("Epos"):Destroy()

														end

													end

													end

										end

										end

										end

								end

							end

						end

					else

						local e = Instance.new("BillboardGui")

						e.Parent = plr.Character.Head

						e.Size = UDim2.new(1.5,0,1.5,0)

						e.AlwaysOnTop = true

						local a = Instance.new("TextLabel")

						a.Parent = e

						a.Size = UDim2.new(1,0,1,0)

						a.Text = (plr.Name)

						a.BackgroundTransparency = 1

						a.TextScaled = true

						a.Name = "name"

						a.Position = UDim2.new(0,0,-0.7,0)

						if plr.TeamColor == game.Players.LocalPlayer.TeamColor then

							a.TextColor3 = Color3.new(0.180392, 1, 0)

						else

							a.TextColor3 = Color3.new(1, 0, 0.0156863)

						end

						a.Font = Enum.Font.SciFi

						local b = Instance.new("TextLabel")

						b.Parent = e

						b.Size = UDim2.new(1,0,1,0)

						b.BorderSizePixel = 0

						b.Name = "square"

						b.BackgroundTransparency = 1

						b.TextColor3 = Color3.new(1, 1, 1)

						b.TextScaled = true

						b.Text = "O"

						a.Position = UDim2.new(0,0,-0.7,0)

						if plr.TeamColor == game.Players.LocalPlayer.TeamColor then

							b.BackgroundColor3 = Color3.new(0.180392, 1, 0)

						else

							b.BackgroundColor3 = Color3.new(1, 0, 0.0156863)

						end

						if plr.Character.Head:FindFirstChild("BillboardGui") then

							if plr.Character.Head:FindFirstChild("BillboardGui"):FindFirstChild("d") then

								

							else

								local r = Instance.new("TextLabel")

								r.Parent = e

								r.Name = "d"

								r.BackgroundTransparency = 1

								r.TextScaled = true

								r.Size = UDim2.new(1,0,1,0)

								r.Position = UDim2.new(0,0,0.85,0)

							end

						end

					end

				else

					if plr.Character.Head:FindFirstChild("BillboardGui") then

						plr.Character.Head:FindFirstChild("BillboardGui"):Destroy()

					end

				end

			else

				if plr.Character.Head:FindFirstChild("BillboardGui") then

					plr.Character.Head:FindFirstChild("BillboardGui"):Destroy()

				end

			end

		end

	end

end)

-- by deconsecrated

while true do

	wait()

	if game.Workspace:FindFirstChild("Epos") then

		local pos = game.Workspace:FindFirstChild("Epos").Position

		wait(0.56)

		if (pos - game.Workspace:FindFirstChild("Epos").Position).Magnitude>4 then

			game.Workspace:FindFirstChild("Epos"):Destroy()

		else

			

			game.Workspace:FindFirstChild("Epos").BillboardGui.es.Text = "Enemies taking cover"

		end

	end

end

-- Made by impulse https://youtube.com/c/ImpulseExploits




