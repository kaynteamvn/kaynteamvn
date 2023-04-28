- 👋 Hi, I’m @kaynteamvn
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
kaynteamvn/kaynteamvn is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

script


a=gg.getFile():match('[^/]+$')
local Vietkey = gg.getFile():gsub(a, 'Viet.key')
local Vietload = loadfile(Vietkey)
if Vietload ~= nil then
  Viet = Vietload()
  Vietload = nil
end
Viet = gg.prompt({"🕵️Tài khoản","🔐Mật Khẩu","Lưu"},Viet,{"text","text","checkbox"})
if not Viet then return else end
if Viet[3] then gg.saveVariable(Viet, Vietkey) end
if Viet[1] == "1234" and Viet[2] == "1234" then gg.toast("Key Đúng Ok♥️") else return gg.alert("Key Sai Ok💘") 
end
function Main()
menu = gg.choice({
"ANTENA TAY",
"Headshot",
"LEO TƯỜNG",
"Xóa Cây",
"THOÁT"
}, nil, 'KAYN TEAM VN🇻🇳')
if menu == nil then else
if menu == 1 then a1() end
if menu == 2 then a2() end
if menu == 3 then a3() end
if menu == 4 then a4() end
if menu == 5 then a5() end
end
XGCK = -1
end
function a1()
gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("-0.02980032004;1:5", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
    gg.refineNumber("1", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
    gg.getResults(10)
    gg.editAll("1909.4", gg.TYPE_FLOAT)
    gg.clearResults()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("0.09043131769;1:5", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
    gg.refineNumber("1", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
    gg.getResults(10)
    gg.editAll("1909.4", gg.TYPE_FLOAT)
    gg.clearResults()
    gg.toast("Antena Tay ✨")
end
function a2()
gg.clearResults()
gg.setRanges(gg.REGION_ANONYMOUS)
gg.searchNumber("96,688,289", gg.TYPE_DWORD)
gg.getResults("220")
gg.editAll("2018908708", gg.TYPE_DWORD)
gg.clearResults()
end
function a3()
gg.clearResults()
gg.setRanges(4)
gg.searchNumber("QF304353F0AD7A33D9A99993E", 1)
gg.refineNumber("Q9A99993E", 1)
gg.getResults(1000)
gg.editAll("Q00C07944", 1)
gg.clearResults()
end
function a4()
gg.setRanges(gg.REGION_CODE_APP)
  gg.searchNumber("60", gg.TYPE_FLOAT)
  gg.getResults(40)
  gg.editAll("-2.2958874e-41", gg.TYPE_FLOAT)
  gg.clearResults()
  gg.toast(" XÓA CÂY ") 
end
function a5()
os.exit()
end
while true do
if gg.isVisible(true) then
XGCK = 1
gg.setVisible(false)
end
gg.clearResults()
if XGCK == 1 then Main() end
end
 