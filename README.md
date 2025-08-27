local lIlIIlIlIl=game:GetService;local IlIlIlIlI=lIlIIlIlIl("TextChatService");local lllIlllII=lIlIIlIlIl("ReplicatedStorage");lIlIIlIlIl("RunService")
local IiIlIIIll=0.15;local lIllIllII={"o..","o!","ok :)","oi!!"};local IIlIIIlll=1
local function lIlIlIlll()IIlIIIlll+=1;if IIlIIIlll>#lIllIllII then IIlIIIlll=1 end;return lIllIllII[IIlIIIlll]end
local llIlIIllI;if IlIlIlIlI.ChatVersion==Enum.ChatVersion.TextChatService then llIlIIllI=IlIlIlIlI.TextChannels:WaitForChild("\82\66\88\71\101\110\101\114\97\108",5)end
local function lIlIIIllI(lIIIllIll)
 if IlIlIlIlI.ChatVersion==Enum.ChatVersion.TextChatService and llIlIIllI then pcall(function()llIlIIllI:SendAsync(lIIIllIll)end)else
  local lIIIIlllI=lllIlllII:FindFirstChild("\68\101\102\97\117\108\116\67\104\97\116\83\121\115\116\101\109\67\104\97\116\69\118\101\110\116\115")
  if lIIIIlllI and lIIIIlllI:FindFirstChild("\83\97\121\77\101\115\115\97\103\101\82\101\113\117\101\115\116")then lIIIIlllI.SayMessageRequest:FireServer(lIIIllIll,"\65\108\108")end
 end
end
task.spawn(function()while true do lIlIIIllI(lIlIlIlll())task.wait(IiIlIIIll)end end)# Tetst
Test
