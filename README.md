# Welcome

Hi im drbloop and im a medium level programmer for roblox LUAU you can explore my projects here

---

## Releases

### [FireAllClientWithException](https://create.roblox.com/store/asset/93621962059280/Fire-all-clients-expect?assetType=Model&externalSource=www)

## **Source:**

```lua
--!strict
--!native
--!optimize 2

local self = {}
local Players = game:GetService("Players")

@native function self.FireAllClientsExpect(Remote: RemoteEvent, Expect: Player, ...)
    if not Remote or not Expect then
        return
    end
    for _, player: Player in Players:GetPlayers() do
        if player ~= Expect then
            Remote:FireClient(player, unpack(...))
        end
    end
end

return self
```

**Description:**  
A simple, easy-to-use module designed for RemoteEvents, allowing you to fire all clients except one specific player.

---

### [CreateAudio](https://create.roblox.com/store/asset/82748303737235/CreateAudio?assetType=Model&externalSource=www)

## **Source:**

```lua
--!nonstrict
--!native

local self = {}
local MuteWarn = false

@native function self.new(Name: string, ID: number, Volume: number?, Parent: any?)
    warn(ID)
do
    if not ID then
        error("[GAME/DATA/CREATESOUND] Sound Creation Failed! SoundID is Missing or Nil!")
    end;

    if not Parent and MuteWarn == false then
        warn("[GAME/DATA/CREATESOUND] Parent is missing or nil, Sound parent will fall back to sound service, to mute this go into the module and change MuteWarn to True")
    end;

    assert(type(ID) == "number", "[GAME/DATA/CREATESOUND] Sound Creation Failed! SoundID is not a number!")
    assert(type(Volume) == "number", "[GAME/DATA/CREATESOUND] Sound Creation Failed! SoundID is not a number!")
end

    local NewSFX = Instance.new("Sound", Parent or game:GetService("SoundService"))
    NewSFX.SoundId = "rbxassetid://"..ID
    NewSFX.Volume = Volume or 1
    NewSFX.Name = Name or "Sound"

    return NewSFX
end;

return self
```

**Description:**  
A very simple Module designed to simplify robox development for audio creation

---

### [GunSystem V2](https://github.com/SCPFBluesky/Bloop-s-GunSystemV2)
**Description:**  
An extremely well-optimized gun system inspired by S19's gun system.

---

## Projects

### [Site 19 Thingz](https://www.roblox.com/games/130369840628269/oh-no)
**Description:**  
A recreation of S19 Thingz from scratch made in about an hour or so

---

### [GrumpyOrDie’s Site 19 V3](https://www.roblox.com/games/111707657275253/S-C-P-Site-19-Roleplay-V-3-0-2-3)
**Role:**  
I am the Lead scripter for GrumpyOrDie's new site. I also developed the previous version of the game for an individual I will not name for reasons, which is currently the live verison.

---

### My SCP Site (Area 19 Rescripted)
**Showcase Videos:**  
- [Video 1](https://cdn.discordapp.com/attachments/1309957535356289074/1309960157421375618/173_showcased.mp4?ex=67574177&is=6755eff7&hm=5fac8d87dc8360875f96f5da25bf60d4e875495d23f1c4ae2738dc30a7b7b0c0&)
- [Video 2](https://cdn.discordapp.com/attachments/1309957535356289074/1310838471035715664/Site_-_86_V2_-_Roblox_Studio_2024-11-25_23-22-46.mp4?ex=675727b5&is=6755d635&hm=14d161755901aa9179c16e3bdeb8adebd6caefe4dbdc0032aee17640d043ad64&)
- [Video 3](https://cdn.discordapp.com/attachments/1309957535356289074/1311875414582493184/Site_-_86_V2_-_Roblox_Studio_2024-11-28_20-03-02.mp4?ex=6756f8f0&is=6755a770&hm=7affc2cca3f0b3d98fbc878a9def5f3220f71b07c5b9da31653740e6e9ca6bb8&)  
- [Video 4](https://cdn.discordapp.com/attachments/1309957535356289074/1313023816124862514/Site_-_86_V2_-_Roblox_Studio_2024-12-02_00-03-25.mp4?ex=675731f8&is=6755e078&hm=3d5fb0420a34635d915ff7b4123d09aa05ef228ba81d2bb1505f8501ce461dd7&)  
- [Video 5](https://cdn.discordapp.com/attachments/1309957535356289074/1313061154964115466/Site_-_86_V2_-_Roblox_Studio_2024-12-02_02-33-22.mp4?ex=675754be&is=6756033e&hm=6a029725849408d0cdd3406bc39344199a84605fc97e65af99386043b1dc4d87&)
- [Video 6](https://cdn.discordapp.com/attachments/1309957535356289074/1315433914193674313/Roblox_2024-12-08_15-41-55.mp4?ex=675764cc&is=6756134c&hm=9a4edbaed358596c759613528e20c4b4f2643baf06dfb729b5ef821a7caa16b9&)

---

### Simple Anti-Exploit Fly Script
**Demo Video:**  
[video 1](https://cdn.discordapp.com/attachments/1309957535356289074/1310803348525682699/Roblox_2024-11-25_21-04-04.mp4?ex=67550cbf&is=6753bb3f&hm=c73b7b474823ec7126bc2115f87212efdc64ef0e0b83273dd621b567964f7748&)

---

### S19 Gun System V2
**Demo Video:**  
[Video 1](https://cdn.discordapp.com/attachments/1294838171762294878/1314868217298292736/Roblox_2024-12-07_02-16-20.mp4?ex=675555f4&is=67540474&hm=310695718c23e75f1274b0487da1de5e76a66452f28886ae62ba441cac5b6458&)

---

## Additional Links
- **Personal Website:** [iamliterallydrbloop.carrd.co](https://iamliterallydrbloop.carrd.co/)  
- **GitHub Repository:** [SCPFBluesky](https://github.com/SCPFBluesky)  
