-- 클라이언트 스크립트
local Players = game:GetService("Players")
local UserInputService = game:GetService("UserInputService")
local LocalPlayer = Players.LocalPlayer

-- GUI 생성
local ScreenGui = Instance.new("ScreenGui", game.CoreGui)
local Hub = Instance.new("Frame", ScreenGui)
Hub.Size = UDim2.new(0.375, 0, 0.65, 0)
Hub.Position = UDim2.new(0.3125, 0, 0.35, 0)
Hub.BackgroundColor3 = Color3.new(0, 0, 0)
Hub.BackgroundTransparency = 0.5
Hub.Active = true
Hub.Draggable = true

-- 상단 검은색 바 + "콘솔x허브" 라벨
local TitleBar = Instance.new("Frame", Hub)
TitleBar.Size = UDim2.new(1, 0, 0.1, 0)
TitleBar.Position = UDim2.new(0, 0, 0, 0)
TitleBar.BackgroundColor3 = Color3.new(0, 0, 0) -- 검은색 바

local TitleLabel = Instance.new("TextLabel", TitleBar)
TitleLabel.Size = UDim2.new(1, 0, 1, 0)
TitleLabel.Position = UDim2.new(0, 0, 0, 0)
TitleLabel.Text = "콘솔x허브"
TitleLabel.TextColor3 = Color3.new(1, 1, 1) -- 흰색 텍스트
TitleLabel.BackgroundTransparency = 1
TitleLabel.Font = Enum.Font.SourceSansBold
TitleLabel.TextScaled = true
