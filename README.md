# DogXfilter
//Version 2.0
//Updated 23/03/2021
//
//╔═══════════════════╗
//║ Table of Contents ║
//╚═══════════════════╝
//Global Filters-30
//Gold-39
//Potions-51
//Quest Items-98
//Runes-127
//Essences-166
//Uber Keys-175
//Diablo Clone-184
//Corruption Items-191
//Map Upgrades-196
//Maps-204
//Gems-207
//Uniques-282
//Sets-509
//Magic Items-584
//Rares-732
//Vendor Items-787
//Bases-818
//Leveling-1296
//
//╔════════════════╗
//║ Global Filters ║
//╚════════════════╝
//ED
ItemDisplay[WEAPON !RW NMAG (ED>0 AND ED<15)]:%WHITE%%NAME% %GREEN%ED%CONTINUE%
ItemDisplay[WEAPON !RW NMAG ED=15]:%PURPLE%%NAME% %GREEN%15 ED%CONTINUE%
//Show me that item is etheral
ItemDisplay[ETH UNI]:%GOLD%Eth %NAME%%CONTINUE%
ItemDisplay[ETH RARE]:%YELLOW%Eth %NAME%%CONTINUE%
ItemDisplay[ETH MAG]:%BLUE%Eth %NAME%%CONTINUE%
ItemDisplay[ETH NMAG]:%GRAY%Eth %NAME%%CONTINUE%
ItemDisplay[ETH CRAFT]:%ORANGE%Eth %NAME%%CONTINUE%
//Show Sockets
ItemDisplay[NMAG SOCK>0]:%GRAY%%NAME% [%SOCKETS%]%CONTINUE%
//╔══════╗
//║ Gold ║
//╚══════╝
//35K
ItemDisplay[NMAG (wnd OR ywn OR 9wn) !ETH (SK83>2 OR SK85>2 OR SK87>2 OR SK88>2 OR SK90>1)]:%GREEN%$$$ %GRAY%%NAME%%CONTINUE%
ItemDisplay[NMAG (wnd OR ywn OR 9wn) !ETH (SK91>1 OR SK92>0 OR SK93>1 OR SK94>1 OR SK95>0)]:%GREEN%$$$ %GRAY%%NAME%%CONTINUE%
ItemDisplay[MAG PRICE>34999]:%GREEN%$$$ %BLUE%%NAME%%CONTINUE%
ItemDisplay[RARE PRICE>34999]:%GREEN%$$$ %YELLOW%%NAME%%CONTINUE%
//Gold
ItemDisplay[GOLD<100 CLVL<20]:
ItemDisplay[GOLD<1000 (CLVL>19 AND CLVL<70)]:
ItemDisplay[GOLD<4999 CLVL>70]:
//╔═════════╗
//║ Potions ║
//╚═════════╝
ItemDisplay[rvl]:%PURPLE%* %PURPLE%R%WHITE%65% %PURPLE%*
ItemDisplay[hp5]:%RED%!%WHITE%H+
ItemDisplay[mp5]:%BLUE%!%WHITE%M+
ItemDisplay[rvs CLVL<81]:%PURPLE%r%WHITE%35%
ItemDisplay[rvs CLVL>80]:
ItemDisplay[hp1 CLVL<15]:%RED%!%WHITE%Minor Heal
ItemDisplay[hp2 CLVL<18]:%RED%!%WHITE%Light Heal
ItemDisplay[hp3 CLVL<24]:%RED%!%WHITE%Healing
ItemDisplay[hp4 CLVL<60]:%RED%!%WHITE%H
ItemDisplay[hp1 CLVL>14]:
ItemDisplay[hp2 CLVL>17]:
ItemDisplay[hp3 CLVL>23]:
ItemDisplay[hp4 CLVL>59]:
ItemDisplay[mp1 CLVL<15]:%BLUE%!%WHITE%Minor Mana
ItemDisplay[mp2 CLVL<20]:%BLUE%!%WHITE%Light Mana
ItemDisplay[mp3 CLVL<26]:%BLUE%!%WHITE%Mana
ItemDisplay[mp4 CLVL<60]:%BLUE%!%WHITE%M
ItemDisplay[mp1 CLVL>14]:
ItemDisplay[mp2 CLVL>19]:
ItemDisplay[mp3 CLVL>25]:
ItemDisplay[mp4 CLVL>59]:
//Utility
ItemDisplay[tsc CLVL<41]:%GREEN%!%WHITE%TP
ItemDisplay[tsc CLVL>40]:
ItemDisplay[isc CLVL<41]:%GREEN%!%WHITE%ID
ItemDisplay[isc CLVL>40]:
ItemDisplay[wms CLVL<60]:%GREEN%!%WHITE%Thaw
ItemDisplay[wms CLVL>59]:
ItemDisplay[yps]:%GREEN%!%WHITE%a
ItemDisplay[vps CLVL<55]:%GREEN%!%WHITE%Stamina
ItemDisplay[vps CLVL>54]:
//Keys for Locked Chests
ItemDisplay[key CLVL<41]:%GRAY%Key
ItemDisplay[key CLVL>40]:
//Tomes
ItemDisplay[tbk]:%WHITE%Tome of Town Portal
ItemDisplay[ibk]:%WHITE%Tome of Identify
//Throwing Potions
ItemDisplay[gpm]:
ItemDisplay[opm]:
ItemDisplay[opl]:
ItemDisplay[ops]:
ItemDisplay[gps]:
ItemDisplay[gpl]:
//╔═════════════╗
//║ Quest Items ║
//╚═════════════╝
ItemDisplay[hdm]:%NAME%%MAP-00% // Horadric Malus
ItemDisplay[bks]:%NAME%%MAP-00% // Scroll of Inifuss
ItemDisplay[bkd]:%NAME%%MAP-00% // Scroll of Inifuss, deciphered
ItemDisplay[leg]:%NAME%%MAP-00% // Wirt's Leg
ItemDisplay[ass]:%NAME%%MAP-00% // Book of Skill
ItemDisplay[tr1]:
ItemDisplay[box]:%NAME%%MAP-00% // Horadric Cube
ItemDisplay[hst]:%NAME%%MAP-00% // Horadric Staff
ItemDisplay[msf]:%NAME%%MAP-00% // Staff of Kings
ItemDisplay[vip]:%NAME%%MAP-00% // Amulet of the Viper
ItemDisplay[j34]:%NAME%%MAP-00% // A Jade Figurine
ItemDisplay[g33]:%NAME%%MAP-00% // Gidbinn
ItemDisplay[qbr]:%NAME%%MAP-00% // Khalim's Brain
ItemDisplay[qey]:%NAME%%MAP-00% // Khalim's Eye
ItemDisplay[qf1]:%NAME%%MAP-00% // Khalim's Flail
ItemDisplay[qhr]:%NAME%%MAP-00% // Khalim's Heart
ItemDisplay[qf2]:%NAME%%MAP-00% // Khalim's Will
ItemDisplay[bbb]:%NAME%%MAP-00% // Lam Esen's Tome
ItemDisplay[mss]:%NAME%%MAP-00% // Mephisto's Soulstone
ItemDisplay[xyz]:%NAME%%MAP-00% // Potion of Life
ItemDisplay[g34]:%NAME%%MAP-00% // The Golden Bird
ItemDisplay[hfh]:%NAME%%MAP-00% // Hellforge Hammer
ItemDisplay[ice]:%NAME%%MAP-00% // Malah's Potion
ItemDisplay[tr2]:%NAME%%MAP-00% // Scroll of Resistance
//Hiding Inferior
ItemDisplay[INF ILVL>14 !RW !leg]:
//╔═══════╗
//║ Runes ║
//╚═══════╝
//1-16
ItemDisplay[r01 OR r01s]:%ORANGE%El 1
ItemDisplay[r02 OR r02s]:%ORANGE%Eld 2 
ItemDisplay[r03 OR r03s]:%ORANGE%Tir 3 
ItemDisplay[r04 OR r04s]:%ORANGE%Nef 4
ItemDisplay[r05 OR r05s]:%ORANGE%Eth 5
ItemDisplay[r06 OR r06s]:%ORANGE%Ith 6 
ItemDisplay[r07 OR r07s]:%ORANGE%Tal 7 
ItemDisplay[r08 OR r08s]:%ORANGE%Ral 8  
ItemDisplay[r09 OR r09s]:%ORANGE%Ort 9 
ItemDisplay[r10 OR r10s]:%ORANGE%Thul 10  
ItemDisplay[r11 OR r11s]:%ORANGE%Amn 11 
ItemDisplay[r12 OR r12s]:%ORANGE%Sol 12  
ItemDisplay[r13 OR r13s]:%ORANGE%Shael 13
ItemDisplay[r14 OR r14s]:%ORANGE%Dol 14 
ItemDisplay[r15 OR r15s]:%ORANGE%Hel 15 
ItemDisplay[r16 OR r16s]:%ORANGE%io 16 
//17-23
ItemDisplay[r17 OR r17s]:%ORANGE%Lum 17 
ItemDisplay[r18 OR r18s]:%ORANGE%Ko 18 
ItemDisplay[r19 OR r19s]:%ORANGE%Fal 19 
ItemDisplay[r20 OR r20s]: %RED%o %PURPLE%Lem 20%RED% o %DOT-62%%BORDER-4B%
ItemDisplay[r21 OR r21s]: %RED%o %PURPLE%Pul 21%RED% o %DOT-62%%BORDER-4B%
ItemDisplay[r22 OR r22s]: %RED%oo %PURPLE%Um 22%RED% oo %DOT-62%%BORDER-4B%
ItemDisplay[r23 OR r23s]: %RED%oo %PURPLE%Mal 23%RED% oo %DOT-62%%BORDER-4B%
//24-33
ItemDisplay[r24 OR r24s]: %RED%ooo %PURPLE%Ist 24%RED% ooo %DOT-76%%MAP-0B%%BORDER-50% 
ItemDisplay[r25 OR r25s]: %RED%oooo %PURPLE%Gul 25%RED% oooo %DOT-76%%MAP-0B%%BORDER-50% 
ItemDisplay[r26 OR r26s]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooooo %PURPLE%Vex 26%RED% ooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
ItemDisplay[r27 OR r27s]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%oooooo %PURPLE%Ohm 27%RED% oooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
ItemDisplay[r28 OR r28s]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooooooo %PURPLE%Lo 28%RED% ooooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
ItemDisplay[r29 OR r29s]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%oooooooo %PURPLE%Sur 29%RED% oooooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
ItemDisplay[r30 OR r30s]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%oooooooooooo %PURPLE%Ber 30%RED% oooooooooooo %RED%*%YELLOW%*%GREEN%*%DOT-62%%BORDER-4B%
ItemDisplay[r31 OR r31s]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%oooooooooo %PURPLE%Jah 31%RED% oooooooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
ItemDisplay[r32 OR r32s]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooooo %PURPLE%Cham 32%RED% ooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
ItemDisplay[r33 OR r33s]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooooo %PURPLE%Zod 33%RED% ooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
//╔══════════╗
//║ Essences ║
//╚══════════╝
ItemDisplay[bet]: %RED%o %GOLD%%NAME%%RED% o %MAP-00%// Burning Essence of Terror
ItemDisplay[ceh]: %RED%o %GOLD%%NAME%%RED% o %MAP-00%// Charged Essence of Hatred
ItemDisplay[fed]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %GOLD%%NAME%%RED% o %RED%*%YELLOW%*%GREEN%*%BLUE%*%MAP-00%// Festering Essence of Destruction
ItemDisplay[tes]: %RED%o %GOLD%%NAME%%RED% o %MAP-00%// Twisted Essence of Suffering
// Tokens
ItemDisplay[toa]:%PURPLE%*Token of Absolution*%MAP-00% // Token of Absolution
//╔═══════════╗
//║ Uber Keys ║
//╚═══════════╝
ItemDisplay[pk1]:%PURPLE%Terror Key [Countess or Blood Raven]%MAP-4B%
ItemDisplay[pk2]:%PURPLE%Hate Key [Summoner or Blood Witch]%MAP-4B%
ItemDisplay[pk3]:%PURPLE%Destruction Key [Nihlathak or Izual]%MAP-4B%
ItemDisplay[dhn]:%PURPLE%Diablo's Horn%MAP-4B%
ItemDisplay[bey]:%PURPLE%Baal's Eye%MAP-4B%
ItemDisplay[mbr]:%PURPLE%Mephisto's Brain%MAP-4B%
//╔══════════════╗
//║ Diablo Clone ║
//╚══════════════╝
ItemDisplay[dcma]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Vision of Terror %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
ItemDisplay[dcbl]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Pure Demonic Essence %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
ItemDisplay[dcho]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %PURPLE%Black Soulstone %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
ItemDisplay[dcso]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Prime Evil Soul %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B% 
//╔══════════════════╗
//║ Corruption Items ║
//╚══════════════════╝
ItemDisplay[wss]:%RED%* %RED%o %PURPLE%Worldstone Shard%RED% o %RED%*%MAP-62%%PX-20%
ItemDisplay[lbox]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%oooooooooo %PURPLE%Larzuk's Puzzle Box %RED%oooooooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B%
//╔══════════════╗
//║ Map Upgrades ║
//╚══════════════╝
ItemDisplay[rera]:%PURPLE% %NAME%%DOT-80% // Reroll Rare Map (Horadrim Orb)
ItemDisplay[imra]:%PURPLE% %NAME%%DOT-80% // Imbue Rare Map (Zakarum Orb)
ItemDisplay[upma]:%PURPLE% %NAME%%DOT-80% // Upgrade Magic Map to Rare Map (Angelic Orb)
ItemDisplay[imma]:%PURPLE% %NAME%%DOT-80% // Imbue Magic Map (Arcane Orb)
ItemDisplay[scou]:%PURPLE% %NAME%%DOT-80% // Purge Map (Removes Mods and Reverts back to a White Map) (Orb of Destruction)
ItemDisplay[upmp]:%PURPLE% %NAME%%DOT-80% // Combine maps into higher tiers (Cartographer's Orb)
ItemDisplay[scrb]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o%PURPLE% %NAME% %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-62%%BORDER-4B% // turns t3 maps into dungeons (Horadrim Scarab)
//╔══════╗
//║ Maps ║
//╚══════╝
ItemDisplay[NMAG (t16 OR t18 OR t17 OR t11 OR t12 OR t13 OR t14 OR t15 OR t21 OR t22 OR t23 OR t24 OR t31 OR t32 OR t33 OR t34 OR t35 OR t41)]:  %WHITE%*** %NAME% ***%CONTINUE%%DOT-62%%BORDER-4B% 
ItemDisplay[MAG (t16 OR t18 OR t17 OR t11 OR t12 OR t13 OR t14 OR t15 OR t21 OR t22 OR t23 OR t24 OR t31 OR t32 OR t33 OR t34 OR t35 OR t41)]:  %BLUE%*** %NAME% ***%CONTINUE%%DOT-62%%BORDER-4B%  
ItemDisplay[RARE (t16 OR t18 OR t17 OR t11 OR t12 OR t13 OR t14 OR t15 OR t21 OR t22 OR t23 OR t24 OR t31 OR t32 OR t33 OR t34 OR t35 OR t41)]:  %YELLOW%*** %NAME% ***%CONTINUE%%DOT-62%%BORDER-4B%
//╔══════╗
//║ Gems ║
//╚══════╝
//Gems Chipped
ItemDisplay[gcv CLVL<21]:chipped amethyst
ItemDisplay[gcw CLVL<21]:chipped diamond
ItemDisplay[gcg CLVL<21]:chipped emerald
ItemDisplay[gcr CLVL<21]:chipped ruby
ItemDisplay[gcb CLVL<21]:chipped sapphire
ItemDisplay[gcy CLVL<21]:chipped topaz
ItemDisplay[skc CLVL<21]:chipped skull
ItemDisplay[gcv CLVL>20]:
ItemDisplay[gcw CLVL>20]:
ItemDisplay[gcg CLVL>20]:
ItemDisplay[gcr CLVL>20]:
ItemDisplay[gcb CLVL>20]:
ItemDisplay[gcy CLVL>20]:
ItemDisplay[skc CLVL>20]:
//Gems Flawed
ItemDisplay[gfv CLVL<30]:flawed amethyst
ItemDisplay[gfw CLVL<30]:flawed diamond
ItemDisplay[gfg CLVL<30]:flawed emerald
ItemDisplay[gfr CLVL<30]:flawed ruby
ItemDisplay[gfb CLVL<30]:flawed sapphire
ItemDisplay[gfy CLVL<30]:flawed topaz
ItemDisplay[skf CLVL<30]:flawed skull
ItemDisplay[gfv CLVL>29]:
ItemDisplay[gfw CLVL>29]:
ItemDisplay[gfg CLVL>29]:
ItemDisplay[gfr CLVL>29]:
ItemDisplay[gfb CLVL>29]:
ItemDisplay[gfy CLVL>29]:
ItemDisplay[skf CLVL>29]:
//Gems Normal
ItemDisplay[gsv CLVL<51]:amethyst
ItemDisplay[gsw CLVL<51]:diamond
ItemDisplay[gsg CLVL<51]:emerald
ItemDisplay[gsr CLVL<51]:ruby
ItemDisplay[gsb CLVL<51]:sapphire
ItemDisplay[gsy CLVL<51]:topaz
ItemDisplay[sku CLVL<51]:skull
ItemDisplay[gsv CLVL>50]:
ItemDisplay[gsw CLVL>50]:
ItemDisplay[gsg CLVL>50]:
ItemDisplay[gsr CLVL>50]:
ItemDisplay[gsb CLVL>50]:
ItemDisplay[gsy CLVL>50]:
ItemDisplay[sku CLVL>50]:
//Gems flawless
ItemDisplay[gzv OR gzvs]://%PURPLE%* %ORANGE%Amethyst %PURPLE%*%WHITE%
ItemDisplay[glw OR glws]://%WHITE%* %ORANGE%Diamond %WHITE%*%WHITE%
ItemDisplay[glg OR glgs]://%GREEN%* %ORANGE%Emerald %GREEN%*%WHITE%
ItemDisplay[glr OR glrs]://%RED%* %ORANGE%Ruby %RED%*%WHITE%
ItemDisplay[glb OR glbs]://%BLUE%* %ORANGE%Sapphire %BLUE%*%WHITE%
ItemDisplay[gly OR glys]://%YELLOW%* %ORANGE%Topaz %YELLOW%*%WHITE%
ItemDisplay[skl OR skls]://%GRAY%* %ORANGE%Skull %GRAY%*%WHITE%
//Gems Perfect
ItemDisplay[gpv OR gpvs]:%PURPLE%* %PURPLE%P Amethyst %PURPLE%*%WHITE%
ItemDisplay[gpw OR gpws]:%WHITE%* %PURPLE%P Diamond %WHITE%*%WHITE%
ItemDisplay[gpg OR gpgs]:%GREEN%* %PURPLE%P Emerald %GREEN%*%WHITE%
ItemDisplay[gpr OR gprs]:%RED%* %PURPLE%P Ruby %RED%*%WHITE%
ItemDisplay[gpb OR gpbs]:%BLUE%* %PURPLE%P Sapphire %BLUE%*%WHITE%
ItemDisplay[gpy OR gpys]:%YELLOW%* %PURPLE%P Topaz %YELLOW%*%WHITE%
ItemDisplay[skz OR skzs]:%GRAY%* %PURPLE%P Skull %GRAY%*%WHITE%
//╔═════════╗
//║ Uniques ║
//╚═════════╝
//////////
//DClone//
//////////
ItemDisplay[UNI !ID uth]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%Dark Abyss%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID 7bs]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%Hadriel's Hand%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID 7qr]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%Aidan's Scar%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID utb]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%Itherael's Path%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID uhl]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%Overlord's Helm%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//////////////////////////////////////
//UNIQUE Rings Amulets Jewels Charms//
//////////////////////////////////////
ItemDisplay[UNI !ID rin]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%U%RED%n%YELLOW%i%GREEN%q%BLUE%u%PURPLE%e %GOLD%Ring %RED%ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID amu]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%U%RED%n%YELLOW%i%GREEN%q%BLUE%u%PURPLE%e %GOLD%Amulet %RED%ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID jew]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o%YELLOW%o%GREEN%o%BLUE%o %PURPLE%R%RED%a%YELLOW%i%GREEN%n%BLUE%b%PURPLE%o%RED%w %GOLD%Facet %BLUE%o%GREEN%o%YELLOW%o%RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID cm1]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Annihilus %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID cm2]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Hellfire Torch %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID cm3]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Gheed's Fortune %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI ID cm1]:%RED%%NAME%%DOT-0C%%BORDER-4B%
ItemDisplay[UNI ID cm2]:%RED%%NAME%%DOT-0C%%BORDER-4B%
ItemDisplay[UNI ID cm3]:%RED%%NAME%%DOT-0C%%BORDER-4B%
/////////
//Helms//
/////////
//Wolfhowl
ItemDisplay[UNI !ID bac]:%RED%o %PURPLE%Wolfhowl %RED%o%BORDER-A5%%DOT-62% 
//Spirit Keeper
ItemDisplay[UNI !ID drd]:%RED%o %PURPLE%Spirit Keeper %RED%o%BORDER-A5%%DOT-62% 
//Valkyrie Wing
ItemDisplay[UNI !ID xhm]:%RED%o %PURPLE%Valkyrie Wing %RED%o%BORDER-A5%%DOT-62% 
//Giant Skull
ItemDisplay[UNI !ID uh9]:%RED%o %PURPLE%Giant Skull %RED%o%BORDER-A5%%DOT-62% 
//Nightwings/Veil of Steel
ItemDisplay[UNI !ID uhm]:%RED%o %PURPLE%Nightwings or Veil of Steel %RED%o%BORDER-A5%%DOT-62% 
//Halaberd's Reign
ItemDisplay[UNI !ID bae]:%RED%o %PURPLE%Halaberd's Reign %RED%o%BORDER-A5%%DOT-62% 
//Griffon's Eye
ItemDisplay[UNI !ID ci3]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%Griffon's Eye%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Shako
ItemDisplay[UNI !ID uap]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%Harlequin Crest%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Crown of Ages
ItemDisplay[UNI !ID urn]:%RED%* %PURPLE%Crown of Ages %RED%*%BORDER-A5%%DOT-62% 
//Andariel's Visage
ItemDisplay[UNI !ID usk]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Andariel's Visage%RED% o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Vampire Gaze
ItemDisplay[UNI !ID xh9]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Vampire Gaze%RED% o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Arreat's Face
ItemDisplay[UNI !ID baa]:%RED%o %PURPLE%Arreat's Face%RED% o%BORDER-A5%%DOT-62% 
//Jalal's Mane
ItemDisplay[UNI !ID dra]:%RED%o %PURPLE%Jalal's Mane%RED% o%BORDER-A5%%DOT-62% 
//Ravenlore
ItemDisplay[UNI !ID dre]:%RED%o %PURPLE%Ravenlore %RED%o%BORDER-A5%%DOT-62% 
//Steel Shade
ItemDisplay[UNI !ID ulm]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Steel Shade %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Stealskull
ItemDisplay[UNI !ID xlm]:%RED%* %PURPLE%Stealskull%RED% *%BORDER-A5%%DOT-62% 
/////////
//Armor//
/////////
//Skullder's Ire
ItemDisplay[UNI !ID xpl]:%RED%o %PURPLE%Skullder's Ire %RED%o%BORDER-A5%%DOT-62% 
//Arkaine's Valor
ItemDisplay[UNI !ID upl]:%RED%o %PURPLE%Arkaine's Valor %RED%o%BORDER-A5%%DOT-62% 
//Gladiator's Bane
ItemDisplay[UNI !ID utu]:%RED%o %PURPLE%Gladiator's Bane %RED%o%BORDER-A5%%DOT-62% 
//Ormus' Robes
ItemDisplay[UNI !ID uui]:%RED%o %PURPLE%Ormus' Robes %RED%o%BORDER-A5%%DOT-62% 
//Viper Magi
ItemDisplay[UNI !ID xea]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Skin of the Vipermagi %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Leviathan
ItemDisplay[UNI !ID uld]:%RED%o %PURPLE%Leviathan %RED%o%BORDER-A5%%DOT-62% 
//Duriel's Shell
ItemDisplay[UNI !ID xrs]:%RED%* %PURPLE%Duriel's Shell %RED%*%BORDER-A5%%DOT-62% 
//Shaftstop
ItemDisplay[UNI !ID xhn]:%RED%* %PURPLE%Shaftstop %RED%*%BORDER-A5%%DOT-62% 
//Tyrael's Might
ItemDisplay[UNI !ETH !ID ILVL>86 uar]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooooo %PURPLE%Tyrael's Might!?%RED% ooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID ILVL<87 uar]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooooo %PURPLE%Templar's Might%RED% ooooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Guardian Angel
ItemDisplay[UNI !ID xlt]:%RED%* %PURPLE%Guardian Angel %RED%*%BORDER-A5%%DOT-62% 
//////////
//Gloves//
//////////
//Frostburn
ItemDisplay[UNI !ID hgl]:%RED%* %PURPLE%Frostburn %RED%*%BORDER-A5%%DOT-62% 
//Ghoulhide
ItemDisplay[UNI !ID xmg]:%RED%* %PURPLE%Ghoulhide%RED% *%BORDER-A5%%DOT-62% 
//Chance Guards 
ItemDisplay[UNI !ID mgl]:%RED%* %PURPLE%Chance Guards %RED%*%BORDER-A5%%DOT-62% 
//Magefist
ItemDisplay[UNI !ID tgl]:%RED%o %PURPLE%Magefist %RED%o%BORDER-A5%%DOT-62% 
//Dracul's Grasp
ItemDisplay[UNI !ID uvg]:%RED%o %PURPLE%Dracul's Grasp %RED%o%BORDER-A5%%DOT-62% 
//Steelrend
ItemDisplay[UNI !ID uhg]:%RED%* %PURPLE%Steelrend %RED%*%BORDER-A5%%DOT-62% 
//Soul Drainer
ItemDisplay[UNI !ID umg]:%RED%* %PURPLE%Soul Drainer %RED%*%BORDER-A5%%DOT-62% 
/////////
//Belts//
/////////
//Goldwrap
ItemDisplay[UNI !ID tbl]:%RED%* %PURPLE%Goldwrap %RED%*%BORDER-A5%%DOT-62% 
//Snowclash
ItemDisplay[UNI !ID ztb]:%RED%* %PURPLE%Snowclash %RED%*%BORDER-A5%%DOT-62% 
//Nosferatu's Coil
ItemDisplay[UNI !ID uvc]:%RED%* %PURPLE%Nosferatu's Coil %RED%*%BORDER-A5%%DOT-62% 
//Gloom's Trap
ItemDisplay[UNI !ID zmb]:%RED%* %PURPLE%Gloom's Trap %RED%*%BORDER-A5%%DOT-62% 
//Arachnid Mesh
ItemDisplay[UNI !ID ulc]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%Arachnid Mesh%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Verdungo's Hearty Cord
ItemDisplay[UNI !ID umc]:%RED%* %PURPLE%Verdungo's Hearty Cord %RED%*%BORDER-A5%%DOT-62% 
//String of Ears
ItemDisplay[UNI !ID zlb]:%RED%* %PURPLE%String of Ears %RED%*%BORDER-A5%%DOT-62% 
//Razortail
ItemDisplay[UNI !ID zvb]:%RED%* %PURPLE%Razortail %RED%*%BORDER-A5%%DOT-62% 
//Thundergod's Vigor
ItemDisplay[UNI !ID zhb]:%RED%* %PURPLE%Thundergod's Vigor %RED%*%BORDER-A5%%DOT-62% 
/////////
//Boots//
/////////
//Waterwalk
ItemDisplay[UNI !ID xvb]:%RED%* %PURPLE%Waterwalk %RED%*%BORDER-A5%%DOT-62% 
//Silkweave
ItemDisplay[UNI !ID xmb]:%RED%* %PURPLE%Silkweave %RED%*%BORDER-A5%%DOT-62% 
//War Traveler
ItemDisplay[UNI !ID xtb]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%War Traveler%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Shadow Dancer
ItemDisplay[UNI !ID uhb]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Shadow Dancer %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Sandstorm Trek
ItemDisplay[UNI !ID uvb]:%RED%* %PURPLE%Sandstorm Trek %RED%*%BORDER-A5%%DOT-62% 
//Gore Rider
ItemDisplay[UNI !ID xhb]:%RED%* %PURPLE%Gore Rider %RED%*%BORDER-A5%%DOT-62% 
///////////
//Weapons//
///////////
//Gavel of Pain
ItemDisplay[UNI !ID 9gm]:%RED%* %PURPLE%Gavel of Pain %RED%*%BORDER-A5%%DOT-62% 
//Gull
ItemDisplay[UNI !ID dgr]:%RED%o %PURPLE%Gull!%RED% o%BORDER-A5%%DOT-62% 
//Death Cleaver
ItemDisplay[UNI !ID 7wa]:%RED%o %PURPLE%Death Cleaver%RED% o%BORDER-A5%%DOT-62% 
//Horizon's Tornado/Stormlash
ItemDisplay[UNI !ID 7fl]:%RED%o %PURPLE%Horizon's Tornado or Stormlash?%RED% o%BORDER-A5%%DOT-62% 
//Windhammer
ItemDisplay[UNI !ID 7m7]:%RED%* %PURPLE%Windhammer %RED%*%BORDER-A5%%DOT-62% 
//The Cranium Basher/Earth shifter
ItemDisplay[UNI !ID 7gm]:%RED%o %PURPLE%Earth Shifter or The Cranium Basher?%RED% o%BORDER-A5%%DOT-62% 
//Hand of Blessed Light
ItemDisplay[UNI !ID 9ws]:%RED%o %PURPLE%Hand of Blessed Light%RED% o%BORDER-A5%%DOT-62% 
//Astreon's Iron Ward
ItemDisplay[UNI !ID 7ws]:%RED%o %PURPLE%Astreon's Iron Ward%RED% o%BORDER-A5%%DOT-62% 
//Steel Pillar
ItemDisplay[UNI !ID 7p7]:%RED%* %PURPLE%Steel Pillar %RED%*%BORDER-A5%%DOT-62% 
//Skull Collector
ItemDisplay[UNI !ID 8ws]:%RED%o %PURPLE%Skull Collector%RED% o%BORDER-A5%%DOT-62% 
//Mang Song's Lesson
ItemDisplay[UNI !ID 6ws]:%RED%o %PURPLE%Mang Song's Lesson%RED% o%BORDER-A5%%DOT-62% 
//The Grandfather
ItemDisplay[UNI !ID 7gd]:%RED%o %PURPLE%The Grandfather%RED% o%BORDER-A5%%DOT-62% 
//Boneshade
ItemDisplay[UNI !ID 7bw]:%RED%* %PURPLE%Boneshade %RED%*%BORDER-A5%%DOT-62% 
//Jade Talon
ItemDisplay[UNI !ID 7wb]:%RED%* %PURPLE%Jade Talon %RED%*%BORDER-A5%%DOT-62% 
//Firelizard's Talons
ItemDisplay[UNI !ID 7lw]:%RED%* %PURPLE%Firelizard's Talons %RED%*%BORDER-A5%%DOT-62% 
//The Oculus
ItemDisplay[UNI !ID oba]:%RED%o %PURPLE%The Oculus%RED% o%BORDER-A5%%DOT-62% 
//Shadow Killer
ItemDisplay[UNI !ID 7cs]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Shadow Killer %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Death's Fathom
ItemDisplay[UNI !ID obf]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Death's Fathom %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Death's Web
ItemDisplay[UNI !ID 7gw]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Death's Web %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Eschuta's Temper
ItemDisplay[UNI !ID obc]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Eschuta's Temper %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Windforce
ItemDisplay[UNI !ID 6lw]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%ooo %PURPLE%Windforce%RED% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Reaper's Toll
ItemDisplay[UNI !ID 7s8]:%RED%* %PURPLE%Reaper's Toll %RED%*%BORDER-A5%%DOT-62% 
//Lacerator
ItemDisplay[UNI !ID 7b8]:%RED%* %PURPLE%Lacerator %RED%*%BORDER-A5%%DOT-62% 
//Azurewrath & Lightsabre
ItemDisplay[UNI !ID ILVL<87 7cr]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Lightsabre %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
ItemDisplay[UNI !ID ILVL>86 7cr]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Azurewrath? %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Tombreaver
ItemDisplay[UNI !ID 7pa]:%RED%* %PURPLE%Tomb Reaver %RED%*%BORDER-A5%%DOT-62% 
//Thunderstroke
ItemDisplay[UNI !ID amf]:%RED%o %PURPLE%Thunderstroke %RED%o%BORDER-A5%%DOT-62% 
//Titan's Revenge
ItemDisplay[UNI !ID ama]:%RED%o %PURPLE%Titan's Revenge %RED%o%BORDER-A5%%DOT-62% 
// Ondal's Wisdom
ItemDisplay[UNI !ID 6cs]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Ondal's Wisdom %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
// Schaefer's Hammer
ItemDisplay[UNI !ID 7wh]:%RED%o %PURPLE%Schaefer's or Stone Crusher %RED%o%DOT-0C%%BORDER-4B%
// Warshrike
ItemDisplay[UNI !ID 7bk]:%RED%* %PURPLE%Warshrike %RED%*%BORDER-A5%%DOT-62% 
//Hexfire
//ItemDisplay[UNI !ID 9sb]:%RED%* %PURPLE%Hexfire %RED%*%BORDER-A5%%DOT-62% 
///////////
//Shields//
///////////
//Boneflame
ItemDisplay[UNI !ID nee]:%RED%* %PURPLE%Boneflame %RED%*%BORDER-A5%%DOT-62% 
//Stormshield
ItemDisplay[UNI !ID uit]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Stormshield%RED% o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Homunculus
ItemDisplay[UNI !ID nea]:%RED%* %PURPLE%Homunculus %RED%*%BORDER-A5%%DOT-62% 
//Herald of Zakarum
ItemDisplay[UNI !ID pa9]:%RED%o %PURPLE%Herald of Zakarum %RED%o%BORDER-A5%%DOT-62% 
//Darkforce Spawn
ItemDisplay[UNI !ID nef]:%RED%* %PURPLE%Darkforce Spawn %RED%*%BORDER-A5%%DOT-62% 
//Medusa's Gaze
ItemDisplay[UNI !ID uow]:%RED%* %PURPLE%Medusa's Gaze %RED%*%BORDER-A5%%DOT-62% 
//Alma Negra
ItemDisplay[UNI !ID pac]:%RED%* %PURPLE%Alma Negra %RED%*%BORDER-A5%%DOT-62% 
//Radament's Sphere
ItemDisplay[UNI !ID xts]:%RED%* %PURPLE%Radament's Sphere %RED%*%BORDER-A5%%DOT-62% 
//Lidless Wall
ItemDisplay[UNI !ID xsh]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Lidless Wall %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Gerke's Sanctuary
ItemDisplay[UNI !ID xow]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Gerke's Sanctuary%RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//Spirit Ward
ItemDisplay[UNI !ID uts]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %RED%o %PURPLE%Spirit Ward %RED%o %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-0C%%BORDER-4B%
//╔══════╗
//║ Sets ║
//╚══════╝
//Jewelry
ItemDisplay[SET !ID amu]:%GREEN%o Amulet o%DOT-84% 
ItemDisplay[SET !ID rin]:%GREEN%o Ring o%DOT-84% 
//
ItemDisplay[SET !ID uar]:%RED%*%YELLOW%*%GREEN%*%BLUE%* %PURPLE%ooo %GREEN%%NAME%%PURPLE% ooo %RED%*%YELLOW%*%GREEN%*%BLUE%*%DOT-84%%BORDER-4B%
ItemDisplay[SET !ID xhb]:%GREEN%o IK Boots o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID zhb]:%GREEN%o IK Belt o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID ba5]:%GREEN%o IK Helm o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID xhg]:%GREEN%o IK Gloves o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID 7m7]:%GREEN%o IK Maul o%DOT-62%%BORDER-84%  
//
ItemDisplay[SET !ID uth]:%GREEN%** %PURPLE%o %GREEN%%NAME%%PURPLE% o %GREEN%*%DOT-84%%BORDER-4B%
ItemDisplay[SET !ID oba]:%GREEN%o Tal's Orb o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID zmb]:%GREEN%o Tal's Belt o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID xsk]:%GREEN%o Tal's Helm o%DOT-62%%BORDER-84% 
//
ItemDisplay[SET !ID 7qr]:%GREEN%o Nat's Claw o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID xmb]:%GREEN%o Nat's Boots o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID xh9]:%GREEN%o Nat's Helm o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID ucl]:%GREEN%o Nat's Armor o%DOT-62%%BORDER-84%  
//
ItemDisplay[SET !ID ulg]:%GREEN%o Laying of Hands o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID xhm]:%GREEN%o G Face o%DOT-62%%BORDER-84%  
//
ItemDisplay[SET !ID xap]:%GREEN%o Cow King's Horns o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID stu]:%GREEN%o Cow King's Hide o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID vbt]:%GREEN%o Cow Kings or Sanders o%DOT-62%%BORDER-84%  
//
ItemDisplay[SET !ID xul]:%GREEN%o Trang's Armor o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID uh9]:%GREEN%o Trang's Helm o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID utc]:%GREEN%o Trang's Belt o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID ne9]:%GREEN%o Trang's Shield o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID xmg]:%GREEN%o Trang's Gloves o%DOT-62%%BORDER-84%  
//
ItemDisplay[SET !ID 6cs]:%GREEN%o Naj's Puzzler o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID ult]:%GREEN%o Naj's Light Plate o%DOT-62%%BORDER-84% 
//
ItemDisplay[SET !ID xar]:%GREEN%o Gris Armor o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID 7ws]:%GREEN%o Gris Weapon o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID urn]:%GREEN%o Gris Helm o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID paf]:%GREEN%o Gris Shield o%DOT-62%%BORDER-84%  
//
ItemDisplay[SET !ID xtb]:%GREEN%o Aldur's Boots o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID dr8]:%GREEN%o Aldur's Helm o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID uul]:%GREEN%o Aldur's Armor o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID 9mt]:%GREEN%o Aldur's Weapon o%DOT-62%%BORDER-84%  
//
ItemDisplay[SET !ID zvb]:%GREEN%o Mav's Belt o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID ci3]:%GREEN%o Mav's Helm o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID amc]:%GREEN%o Mav's Bow o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID uld]:%GREEN%o Mav's Armor o%DOT-62%%BORDER-84%  
ItemDisplay[SET !ID xtg]:%GREEN%o Mav's Gloves o%DOT-62%%BORDER-84%  
//
//Hide normal and exceptional set items
ItemDisplay[SET !ID !ELT CLVL>90]:
//UNIQUE&SET Eth/Socket Catchall
ItemDisplay[UNI !ETH !ID]:%GOLD%o %NAME% o%BORDER-A5%%DOT-62% 
ItemDisplay[SET !ETH !ID]:%GREEN%o %NAME% o%DOT-62%%BORDER-84%  
ItemDisplay[UNI ETH !ID]:%GOLD%o %NAME% o%BORDER-A5%%DOT-62% 
ItemDisplay[SET ETH !ID]:%GREEN%o %NAME% o%DOT-62%%BORDER-84%  
ItemDisplay[UNI ETH ID]:%NAME%%MAP-A5%
ItemDisplay[SET ETH ID]:%NAME%%MAP-84%  
ItemDisplay[UNI ETH SOCK>0 !ID]:o %NAME% o%BORDER-A5%%DOT-62% 
ItemDisplay[SET ETH SOCK>0 !ID]:o %NAME% o%DOT-62%%BORDER-84%  
ItemDisplay[UNI SOCK>0 !ID]:o %NAME% o%BORDER-A5%%DOT-62% 
ItemDisplay[SET SOCK>0 !ID]:o %NAME% o%DOT-62%%BORDER-84% 	
ItemDisplay[UNI ETH SOCK>0]:%NAME%%BORDER-A5%%DOT-62% 
ItemDisplay[SET ETH SOCK>0]:%NAME%%DOT-62%%BORDER-84% 
ItemDisplay[UNI SOCK>0]:%NAME%%BORDER-A5%%DOT-62% 
ItemDisplay[SET SOCK>0]:%NAME%%DOT-62%%BORDER-84% 
ItemDisplay[UNI]:%NAME%%MAP-A5% 
ItemDisplay[SET]:%NAME%%MAP-84% 
//╔═════════════╗
//║ Magic Items ║
//╚═════════════╝
//
//Amulets
ItemDisplay[MAG amu !ID ILVL=85]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 96+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=86]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 94+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=87]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 94+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=88]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 92+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=89]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 92+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=90]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 90+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=91]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 90+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=92]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 88+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=93]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 88+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=94]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 86+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=95]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 86+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=96]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 84+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=97]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 84+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=98]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 82+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL=99]://%BLUE%*** %BLUE%o %NAME%%MAP-97%%PX-62%%ORANGE%[CLVL 82+]%BLUE% o %BLUE%***%WHITE%
ItemDisplay[MAG amu !ID ILVL<85]://%BLUE%*** %NAME%%MAP-97%%PX-62%%WHITE%[%ILVL%]%BLUE% ***%WHITE%
ItemDisplay[MAG amu ID]:%NAME% %WHITE%[%ILVL%]%WHITE%{%YELLOW%Blood Amulet:%ORANGE%Amn %WHITE%+ %RED%P Ruby %WHITE%+ %BLUE%Jewel %YELLOW%Caster Amulet:%ORANGE%Ral %WHITE%+ %PURPLE%P Amethyst %WHITE%+ %BLUE%Jewel}
//
//Rings
ItemDisplay[MAG rin !ID ILVL=71]://%BLUE%%NAME%%ORANGE%[CLVL 99-]
ItemDisplay[MAG rin !ID ILVL=72]://%BLUE%%NAME%%ORANGE%[CLVL 98-]
ItemDisplay[MAG rin !ID ILVL=73]://%BLUE%%NAME%%ORANGE%[CLVL 97-]
ItemDisplay[MAG rin !ID ILVL=74]://%BLUE%%NAME%%ORANGE%[CLVL 96-]
ItemDisplay[MAG rin !ID ILVL=75]://%BLUE%%NAME%%ORANGE%[CLVL 95-]
ItemDisplay[MAG rin !ID ILVL=76]://%BLUE%%NAME%%ORANGE%[CLVL 94-]
ItemDisplay[MAG rin !ID ILVL=77]://%BLUE%%NAME%%ORANGE%[CLVL 93-]
ItemDisplay[MAG rin !ID ILVL=78]://%BLUE%%NAME%%ORANGE%[CLVL 92-]
ItemDisplay[MAG rin !ID ILVL=79]://%BLUE%%NAME%%ORANGE%[CLVL 91-]
ItemDisplay[MAG rin !ID ILVL=80]://%BLUE%%NAME%%ORANGE%[CLVL 90-]
ItemDisplay[MAG rin !ID ILVL=81]://%BLUE%%NAME%%ORANGE%[CLVL 89-]
ItemDisplay[MAG rin !ID ILVL=82]://%BLUE%%NAME%%ORANGE%[CLVL 88-]
ItemDisplay[MAG rin !ID ILVL=83]://%BLUE%%NAME%%ORANGE%[CLVL 87-]
ItemDisplay[MAG rin !ID ILVL=84]://%BLUE%%NAME%%ORANGE%[CLVL 86-]
ItemDisplay[MAG rin !ID ILVL=85]://%BLUE%%NAME%%ORANGE%[CLVL 85-]
ItemDisplay[MAG !ID rin]://%BLUE%%NAME%%WHITE%[%ILVL%]
ItemDisplay[MAG rin ID]:%NAME%%WHITE%[%ILVL%]%WHITE%{%YELLOW%Blood Ring:%ORANGE%Sol %WHITE%+ %RED%P Ruby %WHITE%+ %BLUE%Jewel %YELLOW%Caster Ring:%ORANGE%Amn %WHITE%+ %PURPLE%P Amethyst %WHITE%+ %BLUE%Jewel}
//
//Blue Jewels for crafting
ItemDisplay[MAG !ID jew]://%BLUE%*** %BLUE%o Jewel o %BLUE%***%MAP-97%%PX-62%
//
//Magic Diadems
ItemDisplay[MAG ci3 !ETH !ID]://%BLUE%* %NAME% *%MAP-97%%PX-62%
//Magic Circlets
ItemDisplay[MAG ci0 !ETH !ID]://%BLUE%* %NAME% *%MAP-97%%PX-62%
ItemDisplay[MAG ci1 !ETH !ID]://%BLUE%* %NAME% *%MAP-97%%PX-62%
ItemDisplay[MAG ci2 !ETH !ID]://%BLUE%* %NAME% *%MAP-97%%PX-62%
//
//////////////////////
//(Crafting section)//
//////////////////////
//
//Weapons
//
//ItemDisplay[MAG ILVL>71 WEAPON]: %NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %PURPLE%Caster:%TAN% P Ame + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Sorceress
//
ItemDisplay[MAG ILVL>71 (ob1 OR ob6 OR obb OR ob2 OR ob7 OR obc OR ob3 OR ob8 OR obd OR ob4 OR ob9 OR obe OR ob5 OR oba OR obf)]:// %NAME% {%PURPLE%Caster:%TAN% P Ame + Tir %ORANGE%Craft w/ Jewel:}
//
//Wands
//
ItemDisplay[MAG ILVL>71 (wnd OR 9wn OR 7wn OR ywn OR 9yw OR 7yw OR bwn OR 9bw OR 7bw OR gwn OR 9gw OR 7gw)]:// %NAME% {%PURPLE%Caster:%TAN% P Ame + Tir %ORANGE%Craft w/ Jewel:}
//
//Eth Throwing Weapons
//
ItemDisplay[MAG ILVL>71 ETH (!SPEAR THROWING !ZON) (EXC OR ELT)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:} 
//
//Swords	
//
ItemDisplay[MAG ILVL>71 ETH (crs OR 9cr OR 7cr OR 9ls OR 7ls OR 9gs OR 7gs OR 9fb OR 7fb OR 9gd OR 7gd)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Eth Staves
//
ItemDisplay[MAG ILVL>71 ETH (lst OR 8ls OR 6ls OR cst OR 8cs OR 6cs OR bst OR 8bs OR 6bs OR wst OR 8ws OR 6ws)]:// %NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %PURPLE%Caster:%TAN% P Ame + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Eth Spears
//
ItemDisplay[MAG ILVL>71 ETH (9br OR 7br OR 9st OR 7st OR 9p9 OR 7p7)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Scepters
//
ItemDisplay[MAG ILVL>71 (wsp OR 9ws OR 7ws)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %PURPLE%Caster:%TAN% P Ame + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Eth Polearms
//
ItemDisplay[MAG ILVL>71 ETH (9vo OR 7vo OR 9s8 OR 7s8 OR 9pa OR 7pa OR 9h9 OR 7h7 OR 9wc OR 7wc)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Eth Maces
//
ItemDisplay[MAG ILVL>71 ETH (9fl OR 7fl OR 9m9 OR 7m7 OR 9gm OR 7gm)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Eth Javs
//
ItemDisplay[MAG ILVL>71 ETH (9gl OR 7gl OR 9ts OR 7ts)]: //%NAME% %{%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Eth Daggers
//
ItemDisplay[MAG ILVL>71 ETH DAGGER (EXC OR ELT)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %PURPLE%Caster:%TAN% P Ame + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:} 
//
//Eth Axes
//
ItemDisplay[MAG ILVL>71 ETH (9wa OR 7wa)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Crossbows
//
ItemDisplay[MAG ILVL>71 XBOW (EXC OR ELT)]: //%NAME% {%GREEN%Safety:%TAN% P Eme + Sol%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Bows
//
ItemDisplay[MAG ILVL>71 (8hb OR 6hb OR 8cb OR 6cb OR 8lw OR 6lw)]:// %NAME% {%GREEN%Safety:%TAN% P Eme + Sol %BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Amazon
//
ItemDisplay[MAG ILVL>71 ETH (am3 OR am8 OR amd OR am4 OR am9 OR ame)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
ItemDisplay[MAG ILVL>71 ETH (am5 OR ama OR amf)]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
ItemDisplay[MAG ILVL>71 ZON BOW]: //%NAME% {%GREEN%Safety:%TAN% P Eme + Sol %BLUE%Hit Power:%TAN% P Saph + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Assassin
//
ItemDisplay[MAG ILVL>71 (7ar OR 7wb OR 7xf OR 9cs OR 7cs OR 9lw OR 7lw OR 9tw OR 7tw OR 9qr OR 7qr)]:// %NAME% {%BLUE%Hit Power:%TAN% P Saph + Tir %PURPLE%Caster:%TAN% P Ame + Tir %RED%Blood:%TAN% P Ruby + Ort %ORANGE%Craft w/ Jewel:}
//
//Armor
//
//ItemDisplay[MAG ILVL>71 CHEST (EXC OR ELT)]: //%NAME%{%GREEN%Safety:%TAN% P Eme + Eth %PURPLE%Caster:%TAN% P Ame + Tal %ORANGE%Craft w/ Jewel:}
//
//Paladin Shields
//
ItemDisplay[MAG ILVL>71 CL3]:// %NAME% {%GREEN%Safety:%TAN% P Eme + Nef %PURPLE%Caster:%TAN% P Ame + Eth %ORANGE%Craft w/ Jewel:}
//
//Necro Heads
//
ItemDisplay[MAG ILVL>71 CL4]:// %NAME% {%GREEN%Safety:%TAN% P Eme + Nef %PURPLE%Caster:%TAN% P Ame + Eth %ORANGE%Craft w/ Jewel:}
//
//Barb Helms
//
//ItemDisplay[MAG ILVL>71 CL2]: //%NAME% {%GREEN%Safety:%TAN% P Eme + Ith %PURPLE%Caster:%TAN% P Ame + Nef %ORANGE%Craft w/ Jewel:}
//
//Druid Pelts
//
ItemDisplay[MAG CL1 ILVL>71]://%NAME% {%GREEN%Safety:%TAN% P Eme + Ith %PURPLE%Caster:%TAN% P Ame + Nef %ORANGE%Craft w/ Jewel:}
//
//Shields
//
ItemDisplay[MAG ILVL>71 SHIELD !DIN !NEC (EXC OR ELT)]: //%NAME% {%GREEN%Safety:%TAN% P Eme + Nef %PURPLE%Caster:%TAN% P Ame + Eth %ORANGE%Craft w/ Jewel:}
//
//Gloves
//
ItemDisplay[MAG ILVL>71 GLOVES]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Ort %PURPLE%Caster:%TAN% P Ame + Ort %RED%Blood:%TAN% P Ruby + Nef %ORANGE%Craft w/ Jewel:}
//
//BELTS
//
ItemDisplay[MAG ILVL>71 BELT (EXC OR ELT)]: //%NAME% {%PURPLE%Caster:%TAN% P Ame + Ith %RED%Blood:%TAN% P Ruby + Tal %ORANGE%Craft w/ Jewel:}
//
//BOOTS
//
ItemDisplay[MAG ILVL>71 BOOTS]: //%NAME% {%BLUE%Hit Power:%TAN% P Saph + Ral %PURPLE%Caster:%TAN% P Ame + Thul %RED%Blood:%TAN% P Ruby + Eth %ORANGE%Craft w/ Jewel:}
//
////////////////
//(ID section)//
////////////////
ItemDisplay[MAG ID cm3 TABSK8=1]:%PURPLE%Fire Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK10=1]:%PURPLE%Cold Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK9=1]:%PURPLE%Light Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK17=1]:%PURPLE%PnB Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK18=1]:%PURPLE%Nsum Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK24=1]:%PURPLE%Pcomb Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK48=1]:%PURPLE%Trap Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK49=1]:%PURPLE%Shadow Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK50=1]:%PURPLE%Martial Arts Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK34=1]:%PURPLE%Warcries Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK42=1]:%PURPLE%Ele Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK41=1]:%PURPLE%SS Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK40=1]:%PURPLE%Dsum Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK2=1]:%PURPLE%Java Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm3 TABSK0=1]:%PURPLE%Bow Skiller%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm1 LIFE>15]:%PURPLE%Life Small Charm%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm1 MANA>13]:%PURPLE%Mana Small Charm%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm1 RES>2]:%PURPLE%Res Small Charm%WHITE%[%ILVL%]
ItemDisplay[MAG ID cm1 MFIND>5]:%PURPLE%Mf Small Charm%WHITE%[%ILVL%]
/////////////
//Rerolling//
/////////////
ItemDisplay[MAG cm3 ID ILVL>90]:%ORANGE%Reroll %BLUE%%NAME% %ORANGE%[%ILVL%]%MAP-97%%PX-62%
/////////////
//Runewords//
/////////////
ItemDisplay[RW]:%GOLD%%NAME%%MAP-60%
//////////
//Charms//
//////////
ItemDisplay[MAG !ID cm1]:%WHITE%%BLUE%*** %BLUE%o %NAME%%GRAY%[%ILVL%]%BLUE% o %BLUE%***%WHITE%%MAP-97%%PX-62%
ItemDisplay[MAG !ID cm2 CLVL<90]://%WHITE%%BLUE%*** %BLUE%o %NAME%%GRAY%[%ILVL%]%BLUE% o %BLUE%***%WHITE%%MAP-97%%PX-62%
ItemDisplay[MAG !ID cm2 CLVL>89]://%WHITE%%BLUE%* %NAME% %GRAY%[%ILVL%]%BLUE% *%WHITE%
ItemDisplay[MAG !ID ILVL<91 cm3]:%WHITE%%BLUE%*** %BLUE%o %NAME%%GRAY%[%ILVL%]%BLUE% o %BLUE%***%WHITE%%MAP-97%%PX-62%
ItemDisplay[MAG !ID ILVL>90 cm3]:%WHITE%%BLUE%*** %BLUE%o %ORANGE%Reroll %BLUE%%NAME%%ORANGE%[%ILVL%]%BLUE% o %BLUE%***%WHITE%%MAP-97%%PX-62%
//╔═══════╗
//║ Rares ║
//╚═══════╝
//Best Rares (Circlets, Amulets, Rings, Gloves, Boots, Belts, Jewels)
ItemDisplay[RARE ci0 !ID]:%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62%
ItemDisplay[RARE ci1 !ID]:%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62% 
ItemDisplay[RARE ci2 !ID]:%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62%
ItemDisplay[RARE ci3 !ID]:%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62% 
ItemDisplay[RARE amu !ID]:%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62% 
ItemDisplay[RARE rin !ID]:%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62% 
ItemDisplay[RARE EQ4 !ID]://%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62%
ItemDisplay[RARE EQ5 !ID]://%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62%
ItemDisplay[RARE EQ6 !ID]://%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62%
ItemDisplay[RARE jew !ID]:%WHITE%%YELLOW%*** %YELLOW%o %NAME% o %YELLOW%***%WHITE%%MAP-A8%%BORDER-62%
//
//stop scuffed rare belts showing
ItemDisplay[RARE vbl !ID CLVL>40]:
ItemDisplay[RARE lbl !ID CLVL>40]:
//
//Merc Rares
ItemDisplay[RARE ETH ELT WP3 !ID]://%NAME%
ItemDisplay[RARE ETH ELT WP7 !ID]://%NAME%
ItemDisplay[RARE ETH ELT WP8 !ID]://%NAME%
ItemDisplay[RARE !ETH ELT WP3 !ID]://%NAME%
ItemDisplay[RARE !ETH ELT WP7 !ID]://%NAME%
ItemDisplay[RARE !ETH ELT WP8 !ID]://%NAME%
//
//Class Specific Rares (Druid Pelts, Barb Helms, Paladin Shields, Necro Heads, Assassin Claws, Sorc Orbs)
ItemDisplay[RARE CL1 !ID]://%YELLOW%* %NAME% *%WHITE%%MAP-A8%
ItemDisplay[RARE CL2 !ID]://%YELLOW%* %NAME% *%WHITE%%MAP-A8%
ItemDisplay[RARE CL3 !ID]://%YELLOW%* %NAME% *%WHITE%%MAP-A8%
ItemDisplay[RARE CL4 !ID]://%YELLOW%* %NAME% *%WHITE%%MAP-A8%
ItemDisplay[RARE CL5 !ID]://%YELLOW%* %NAME% *%WHITE%%MAP-A8%
ItemDisplay[RARE CL6 !ID]://%YELLOW%* %NAME% *%WHITE%%MAP-A8%
//
//Caster Rares (Staff, Wand, Scepter)
ItemDisplay[RARE WP11 !ID]://%NAME%
ItemDisplay[RARE WP12 !ID]://%NAME%
ItemDisplay[RARE WP13 !ID]://%NAME%
//
//None of the Above
//Weapons (Axe, Mace, Sword, Dagger, Throwing Weapon, Javelin, Spear, Polearm, Bow, Crossbow)
ItemDisplay[RARE WP1 !ID ILVL>66]://%NAME%
ItemDisplay[RARE WP2 !ID ILVL>66]://%NAME%
ItemDisplay[RARE WP4 !ID ILVL>66]://%NAME%
ItemDisplay[RARE WP5 !ID ILVL>66]://%NAME%
ItemDisplay[RARE WP6 !ID ILVL>66]://%NAME%
ItemDisplay[RARE WP9 !ID ILVL>66]://%NAME%
ItemDisplay[RARE WP10 !ID ILVL>66]://%NAME%
//Armor:Helm (Not Circlet), Body, Shield (ilvl 66+)
ItemDisplay[RARE EQ1 !ID ILVL>66]://%NAME%
ItemDisplay[RARE EQ2 !ID ILVL>66]://%NAME%
ItemDisplay[RARE EQ3 !ID ILVL>66]://%NAME%
//Show Rare Elite Armor
ItemDisplay[ELT RARE ARMOR !ID]://%NAME%
//╔══════════════╗
//║ Vendor Items ║
//╚══════════════╝
//Bo Sticks
ItemDisplay[MAG WP5 ID TABSK34=3]:%PURPLE%+++++ %ORANGE%BO STICK %PURPLE%+++++
// +2/20 and +3/20 Gloves
ItemDisplay[MAG ID EQ4 !ETH TABSK0=2 IAS=20]:%PURPLE%+ %ORANGE%Bowazon Gloves %PURPLE%+
ItemDisplay[MAG ID EQ4 !ETH TABSK2=2 IAS=20]:%PURPLE%+ %ORANGE%Javazon Gloves %PURPLE%+
ItemDisplay[MAG ID EQ4 !ETH TABSK50=2 IAS=20]:%PURPLE%+ %ORANGE%Martial Gloves %PURPLE%+
ItemDisplay[MAG ID EQ4 !ETH TABSK0=3 IAS=20]:%PURPLE%+ %ORANGE%Bowazon Gloves %PURPLE%+
ItemDisplay[MAG ID EQ4 !ETH TABSK2=3 IAS=20]:%PURPLE%+ %ORANGE%Javazon Gloves %PURPLE%+
ItemDisplay[MAG ID EQ4 !ETH TABSK50=3 IAS=20]:%PURPLE%+ %ORANGE%Martial Gloves %PURPLE%+
// +6 Skill
ItemDisplay[MAG ID CL5 (TABSK48=3 AND SK251=3)]:%PURPLE%+ %ORANGE%FIREBLAST CLAW %PURPLE%+
ItemDisplay[MAG ID CL5 (TABSK48=3 AND SK261=3)]:%PURPLE%+ %ORANGE%CHARGED BOLT CLAW %PURPLE%+
ItemDisplay[MAG ID CL5 (TABSK48=3 AND SK262=3)]:%PURPLE%+ %ORANGE%WAKE OF FIRE CLAW %PURPLE%+
ItemDisplay[MAG ID CL5 (TABSK49=3 AND SK267=3)]:%PURPLE%+ %ORANGE%FADE CLAW %PURPLE%+
ItemDisplay[MAG ID CL5 (TABSK48=3 AND SK271=3)]:%PURPLE%+ %ORANGE%LIGHTNING CLAW %PURPLE%+
ItemDisplay[MAG ID CL5 (TABSK48=3 AND SK272=3)]:%PURPLE%+ %ORANGE%WAKE OF FIRE CLAW %PURPLE%+
ItemDisplay[MAG ID CL5 (TABSK49=3 AND SK278=3)]:%PURPLE%+ %ORANGE%VENOM CLAW %PURPLE%+
ItemDisplay[MAG ID CL6 (TABSK10=3 AND SK40=3)]:%PURPLE%+ %ORANGE%FRIGERATE ORB %PURPLE%+
ItemDisplay[MAG ID CL6 (TABSK10=3 AND SK50=3)]:%PURPLE%+ %ORANGE%SHIVER ORB %PURPLE%+
ItemDisplay[MAG ID CL6 (TABSK8=3 AND SK52=3)]:%PURPLE%+ %ORANGE%ENFLAME ORB %PURPLE%+
ItemDisplay[MAG ID CL6 (TABSK9=3 AND SK57=3)]:%PURPLE%+ %ORANGE%DISCHARGE ORB %PURPLE%+
ItemDisplay[MAG ID CL6 (TABSK9=3 AND SK58=3)]:%PURPLE%+ %ORANGE%E-SHIELD ORB %PURPLE%+
ItemDisplay[MAG ID CL6 (TABSK8=3 AND SK62=3)]:%PURPLE%+ %ORANGE%HYDRA ORB %PURPLE%+
ItemDisplay[MAG ID WP13 (TABSK25=3 AND SK102=3)]:%PURPLE%+ %ORANGE%HOLY FIRE SCEPTER %PURPLE%+
ItemDisplay[MAG ID WP13 (TABSK25=3 AND SK114=3)]:%PURPLE%+ %ORANGE%HOLY FREEZE SCEPTER %PURPLE%+
ItemDisplay[MAG ID WP13 (TABSK25=3 AND SK118=3)]:%PURPLE%+ %ORANGE%HOLY SHOCK SCEPTER %PURPLE%+
ItemDisplay[MAG ID WP13 (TABSK25=3 AND SK119=3)]:%PURPLE%+ %ORANGE%SANCTUARY SCEPTER %PURPLE%+
ItemDisplay[MAG ID WP13 (TABSK24=3 AND SK121=3)]:%PURPLE%+ %ORANGE%FOH SCEPTER %PURPLE%+
//╔═══════╗
//║ Bases ║
//╚═══════╝
//Inferior Items
ItemDisplay[INF ILVL<10 !RW !leg]:%NAME%
ItemDisplay[INF !RW !leg]:
ItemDisplay[aqv NMAG]:
ItemDisplay[cqv NMAG]:
//
//Tiara/Diadem Imbue Charsi
ItemDisplay[NMAG ci2 !ETH SOCK=0]://%NAME%
ItemDisplay[NMAG ci2 !ETH SOCK=1]://%NAME%
ItemDisplay[NMAG ci2 !ETH SOCK=2]://%NAME%
ItemDisplay[NMAG ci2 !ETH SOCK=3]://%NAME%
//Diadem
ItemDisplay[NMAG ci3 !ETH SOCK=0]://%NAME%
ItemDisplay[NMAG ci3 !ETH SOCK=1]://%NAME%
ItemDisplay[NMAG ci3 !ETH SOCK=2]://%NAME%
ItemDisplay[NMAG ci3 !ETH SOCK=3]://%NAME%
//
//Armor
//Hide Non Eth Medium and Heavy Bases
ItemDisplay[ucl !ETH NMAG]:
ItemDisplay[ung !ETH NMAG]:
ItemDisplay[upl !ETH NMAG]:
ItemDisplay[uhn !ETH NMAG]:
ItemDisplay[ult !ETH NMAG]:
ItemDisplay[uld !ETH NMAG]:
ItemDisplay[uth !ETH NMAG]:
ItemDisplay[uul !ETH NMAG]:
ItemDisplay[uar !ETH NMAG]:
////////////////
//Enhanced Def//
////////////////
ItemDisplay[NMAG CHEST !ETH !SOCK=1 ELT (ED>4 AND ED<15)]:%DARK_GREEN%%NAME%%ORANGE% ED%WHITE%%MAP-97%
ItemDisplay[NMAG CHEST !ETH !SOCK=1 ELT ED=15]:%RED%* %GREEN%%NAME%%PURPLE% 15 ED%WHITE% %RED%*%MAP-97%
ItemDisplay[NMAG CHEST !ETH SOCK>1 ELT]:%DARK_GREEN%%NAME%%WHITE%
ItemDisplay[NMAG CHEST ETH !SOCK=1 ELT (ED>4 AND ED<15)]:%DARK_GREEN%%NAME%%ORANGE% ED%WHITE%%MAP-97%
ItemDisplay[NMAG CHEST ETH !SOCK=1 ELT ED=15]:%RED%* %GREEN%%NAME%%PURPLE% 15 ED%WHITE% %RED%*%MAP-97%
ItemDisplay[NMAG CHEST ETH SOCK>1 ELT]:%DARK_GREEN%%NAME%%WHITE%
ItemDisplay[NMAG CHEST !SUP (SOCK=0 OR SOCK=1)]:
//
//0soc 2soc 3soc Light Plate
ItemDisplay[NMAG SOCK>1 ltp]:
ItemDisplay[NMAG SOCK=0 ltp]:
ItemDisplay[NMAG SOCK=1 ltp]:
//0 soc 2soc 3soc Mage Plate 
ItemDisplay[NMAG !SOCK=1 xtp (ED>4 AND ED<15)]:%DARK_GREEN%%NAME%%MAP-97%%ORANGE% ed %YELLOW% 
ItemDisplay[NMAG SOCK=1 xtp]:
ItemDisplay[NMAG SOCK=3 ED=15 xtp]:%DARK_GREEN%%NAME%%MAP-97%%ORANGE% 15 ed %YELLOW%%MAP-97% 
//
//Shields
//4os Monarch, Monarch
ItemDisplay[uit !ETH SOCK=4 NMAG]:%DARK_GREEN%%NAME%%MAP-97% %YELLOW% 
ItemDisplay[uit !ETH SOCK=0 DEF>146 NMAG]:%DARK_GREEN%%NAME%%MAP-97%%YELLOW% 
ItemDisplay[uit !ETH SOCK=0 NMAG CLVL<86]:%WHITE%%NAME%
ItemDisplay[uit !ETH SOCK=0 NMAG CLVL>85]:
//
//All Polearms/Spears ED
ItemDisplay[NMAG (WP8 OR WP7) ELT !ETH CLVL>90]:
ItemDisplay[NMAG (WP8 OR WP7) ETH ELT ED=15 SOCK=4]: %PURPLE%o %GREEN%%NAME% %ORANGE%15 ed %RED% %PURPLE%o 
ItemDisplay[NMAG (WP8 OR WP7) ETH ELT (ED>4 AND ED<15) SOCK=4]:%PURPLE%o %GREEN%%NAME% %ORANGE% ed %RED% %PURPLE%o
ItemDisplay[NMAG (WP8 OR WP7) ETH ELT SOCK>3]:%GREEN%%NAME% %ORANGE% %RED%
ItemDisplay[NMAG (WP8 OR WP7) !ELT !ETH]:
//
//Paladin Shields Top Tier Elite non-eth, Medium-High Eth, Basic (ILVL restriction)
ItemDisplay[NMAG pab !ETH (RES>20 AND RES<30) !SOCK=1]:%GREEN%Res %NAME%%MAP-97%%RED%
ItemDisplay[NMAG pab !ETH RES=30 !SOCK=1]:%GREEN%30 Res %NAME%%MAP-97%%RED%
ItemDisplay[NMAG pab ETH (RES>20 AND RES<30) !SOCK=1]:%GREEN%Res %NAME%%MAP-97%%RED%
ItemDisplay[NMAG pab ETH RES=30 !SOCK=1]:%GREEN%30 Res %NAME%%MAP-97%%RED%
ItemDisplay[NMAG CL3 ELT !ETH (RES>20 AND RES<30) !SOCK=1]:%GREEN%Res %NAME%%MAP-97%%RED%
ItemDisplay[NMAG CL3 ELT !ETH RES=30 !SOCK=1]:%GREEN%45 Res %NAME%%MAP-97%%RED%
ItemDisplay[NMAG CL3 ELT ETH (RES>20 AND RES<30) !SOCK=1]:%GREEN%Res %NAME%%MAP-97%%RED%
ItemDisplay[NMAG CL3 ELT ETH RES=30 !SOCK=1]:%GREEN%30 Res %NAME%%MAP-97%%RED%
ItemDisplay[NMAG CL3 RES>25 SOCK=2 !ETH CLVL<85]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG CL3 RES>25 SOCK=0 !ETH CLVL<85]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG CL3 RES>25 SOCK=4 !ETH CLVL<85]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG CL3 RES>25 SOCK=3 !ETH CLVL<85]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG CL3 RES>20 SOCK=2 !ETH CLVL<85]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[NMAG CL3 RES>20 SOCK=0 !ETH CLVL<85]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[NMAG CL3 RES>20 SOCK=4 !ETH CLVL<85]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[NMAG CL3 RES>20 SOCK=3 !ETH CLVL<85]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[NMAG CL3 SOCK=4 CLVL<69]:%GRAY%%NAME% 
ItemDisplay[NMAG CL3 !ETH RES=30 SOCK=4]:%ORANGE%30 Res %DARK_GREEN%%NAME%%GRAY%
ItemDisplay[NMAG CL3 !ETH RES=30 SOCK=3]:%ORANGE%30 Res %DARK_GREEN%%NAME%%GRAY%
ItemDisplay[NMAG CL3 !ETH RES=30 SOCK=0]:%ORANGE%30 Res %DARK_GREEN%%NAME%%GRAY%
//
//Claws
ItemDisplay[CL5 NMAG SOCK=3 (SK277=3 AND SK278<0)]:%RED%Blade Shield & Venom %GREEN%%NAME% %RED%
ItemDisplay[CL5 NMAG !9cs !7xf !7cs SOCK=0 (SK277=3 AND SK278<0)]:%RED%Blade Shield & Venom %GREEN%%NAME% %RED%
ItemDisplay[CL5 NMAG SOCK=3 (SK277=3)]:%RED%Blade Shield %GREEN%%NAME% %RED%
ItemDisplay[CL5 NMAG !9cs !7xf !7cs SOCK=0 (SK277=3)]:%RED%Blade Shield %GREEN%%NAME% %RED%
ItemDisplay[CL5 NMAG SOCK=3 (SK278=3)]:%RED%Venom %GREEN%%NAME% %RED%
ItemDisplay[CL5 NMAG !9cs !7xf !7cs SOCK=0 (SK278=3)]:%RED%Venom %GREEN%%NAME% %RED%
ItemDisplay[NMAG CL5 (SK262=3) SOCK=3]:%DARK_GREEN%+3 Wake Fire %NAME%%GRAY%
ItemDisplay[NMAG CL5 (SK261=3) SOCK=3]:%DARK_GREEN%+3 Bolt Sentry %NAME%%GRAY%
ItemDisplay[NMAG CL5 (SK271=3) SOCK=3]:%DARK_GREEN%+3 Lite Sentry %NAME%%GRAY%
ItemDisplay[NMAG CL5 (SK273=3) SOCK=3]:%DARK_GREEN%+3 Mind Blast %NAME%%GRAY%
ItemDisplay[NMAG CL5 !9cs !7xf !7cs (SK262=3) SOCK=0]:%DARK_GREEN%+3 Wake Fire %NAME%%GRAY%
ItemDisplay[NMAG CL5 !9cs !7xf !7cs (SK261=3) SOCK=0]:%DARK_GREEN%+3 Bolt Sentry %NAME%%GRAY%
ItemDisplay[NMAG CL5 !9cs !7xf !7cs (SK273=3) SOCK=0]:%DARK_GREEN%+3 Mind Blast %NAME%%GRAY%
ItemDisplay[NMAG CL5 !9cs !7xf !7cs (SK271=3) SOCK=0]:%DARK_GREEN%+3 Lite Sentry %NAME%%GRAY%
ItemDisplay[CL5 (SK262=3)]:%DARK_GREEN%+3 Wake Fire Claw%GRAY%
ItemDisplay[CL5 (SK261=3)]:%DARK_GREEN%+3 Bolt Sentry Claw%GRAY%
ItemDisplay[CL5 (SK271=3)]:%DARK_GREEN%+3 Lite Sentry Claw%GRAY%
ItemDisplay[CL5 (SK273=3)]:%DARK_GREEN%+3 Mind Blast Claw%GRAY%
ItemDisplay[CL5 (SK262<0)]:%GRAY%Wake Fire Claw%GRAY%
ItemDisplay[CL5 (SK271<0)]:%GRAY%Lite Sentry Claw%GRAY%
ItemDisplay[CL5 (SK261<0)]:%GRAY%Bolt Sentry Claw%GRAY%
ItemDisplay[CL5 (SK273<0)]:%GRAY%Mind Blast Claw%GRAY%
//ItemDisplay[7ar NMAG !ETH (SK274<0 AND SK275<0) SOCK=3]:%GREEN%Slow Chaos Base %YELLOW%
//ItemDisplay[7ar NMAG !ETH (SK274<0 AND SK275<0) SOCK=0]:%GREEN%Slow Chaos Base %YELLOW%
//ItemDisplay[7tw NMAG !ETH (SK274<0 AND SK275<0) SOCK=3]:%GREEN%Fast Chaos Base %YELLOW%
//ItemDisplay[7tw NMAG !ETH (SK274<0 AND SK275<0) SOCK=0]:%GREEN%Fast Chaos Base %YELLOW%
//ItemDisplay[7ar NMAG !ETH SOCK=3 (SK274<0)]:%GRAY%Slow Chaos Base
//ItemDisplay[7ar NMAG !ETH SOCK=0 (SK274<0)]:%GRAY%Slow Chaos Base
//ItemDisplay[7tw NMAG !ETH SOCK=3 (SK274<0)]:%GRAY%Fast Chaos Base
//ItemDisplay[7tw NMAG !ETH SOCK=0 (SK274<0)]:%GRAY%Fast Chaos Base
//ItemDisplay[7ar NMAG !ETH SOCK=3 (SK275<0)]:%GRAY%Slow Chaos Base
//ItemDisplay[7ar NMAG !ETH SOCK=0 (SK275<0)]:%GRAY%Slow Chaos Base
//ItemDisplay[7tw NMAG !ETH SOCK=3 (SK275<0)]:%GRAY%Fast Chaos Base
//ItemDisplay[7tw NMAG !ETH SOCK=0 (SK275<0)]:%GRAY%Fast Chaos Base
//
//Spirit Sword
ItemDisplay[crs ETH NMAG SOCK=4]:%DARK_GREEN%%NAME%%MAP-97% %YELLOW%
ItemDisplay[crs !ETH NMAG SOCK=4]:%DARK_GREEN%%NAME%%MAP-97% %GRAY%
ItemDisplay[bsd NMAG SOCK=4]:%DARK_GREEN%%NAME%%MAP-97% %GRAY%
ItemDisplay[crs NMAG SOCK=4 CLVL>90]:
ItemDisplay[bsd NMAG SOCK=4 CLVL>90]:
ItemDisplay[crs NMAG SOCK=0 (ILVL>25 AND ILVL<41)]:%DARK_GREEN%%NAME%%WHITE% 4 soc from larzuk
ItemDisplay[bsd NMAG SOCK=0 (ILVL>25 AND ILVL<75)]:%DARK_GREEN%%NAME%%WHITE% 4 soc from larzuk
//
//Insight/Infinity
ItemDisplay[NMAG ETH SOCK=4 7vo]:%GREEN%%NAME% %RED%
ItemDisplay[NMAG ETH SOCK=4 7s8]:%GREEN%%NAME% %RED%
ItemDisplay[NMAG ETH SOCK=4 7pa]:%GREEN%%NAME% %RED%
ItemDisplay[NMAG ETH SOCK=4 7h7]:%GREEN%%NAME% %RED%
ItemDisplay[NMAG ETH SOCK=4 7wc]:%GREEN%%NAME% %RED%
ItemDisplay[NMAG ETH SOCK=4 7br]:%GREEN%%NAME% %RED%
//
//Hide non-eth 
ItemDisplay[NMAG !ETH 7vo]:
ItemDisplay[NMAG !ETH 7s8]:
ItemDisplay[NMAG !ETH 7pa]:
ItemDisplay[NMAG !ETH 7h7]:
ItemDisplay[NMAG !ETH 7wc]:
ItemDisplay[NMAG !ETH 7br]:
ItemDisplay[NMAG vou !ETH]:
ItemDisplay[NMAG 9vo !ETH]:
ItemDisplay[NMAG scy !ETH CLVL<93]:
ItemDisplay[NMAG 9s8 !ETH CLVL<93]:
ItemDisplay[NMAG brn !ETH CLVL<93]:
ItemDisplay[NMAG 9br !ETH CLVL<93]:
ItemDisplay[NMAG pax !ETH]:
ItemDisplay[NMAG 9pa !ETH]:
ItemDisplay[NMAG hal !ETH]:
ItemDisplay[NMAG 9h9 !ETH]:
ItemDisplay[NMAG wsc !ETH CLVL<93]:
ItemDisplay[NMAG 9wc !ETH CLVL<93]:
//
//Norm/Exceptional
ItemDisplay[NMAG vou ETH SOCK=4]:
ItemDisplay[NMAG 9vo ETH SOCK=4]:
ItemDisplay[NMAG scy ETH SOCK=4 CLVL<93]:%GRAY%%NAME% %GRAY%
ItemDisplay[NMAG 9s8 ETH SOCK=4 CLVL<93]:%GRAY%%NAME% %GRAY%
ItemDisplay[NMAG brn ETH SOCK=4 CLVL<93]:%GRAY%%NAME% %GRAY%
ItemDisplay[NMAG 9br ETH SOCK=4 CLVL<93]:%GRAY%%NAME% %GRAY%
ItemDisplay[NMAG pax ETH SOCK=4]:
ItemDisplay[NMAG 9pa ETH SOCK=4]:
ItemDisplay[NMAG hal ETH SOCK=4]:
ItemDisplay[NMAG 9h9 ETH SOCK=4]:
ItemDisplay[NMAG wsc ETH SOCK=4 CLVL<93]:%GRAY%%NAME% %GRAY%
ItemDisplay[NMAG 9wc ETH SOCK=4 CLVL<93]:%GRAY%%NAME% %GRAY%
ItemDisplay[NMAG scy SOCK=4]:
ItemDisplay[NMAG wsc SOCK=4]:
ItemDisplay[NMAG 9wc SOCK=4]:
ItemDisplay[NMAG 9s8 SOCK=4]:
//
//Elite
ItemDisplay[ETH 7vo NMAG !SUP SOCK=0]:%GRAY%%NAME%%GRAY%
ItemDisplay[ETH 7s8 NMAG !SUP SOCK=0]:%GRAY%%NAME%%GRAY%
ItemDisplay[ETH 7pa NMAG !SUP SOCK=0]:%GRAY%%NAME%%GRAY%
ItemDisplay[ETH 7h7 NMAG !SUP SOCK=0]:%GRAY%%NAME%%GRAY%
ItemDisplay[ETH 7wc NMAG !SUP SOCK=0]:%GRAY%%NAME%%GRAY%
ItemDisplay[ETH 7br NMAG !SUP SOCK=0]:%DARK_GREEN%%NAME%%YELLOW%
ItemDisplay[ETH 7p7 NMAG !SUP SOCK=0]:%GRAY%%NAME% %GRAY%
//
//5 socket polearms & spears
ItemDisplay[NMAG ETH SUP SOCK=5 7h7]:%GREEN%SUP %NAME%%YELLOW%
ItemDisplay[NMAG ETH SOCK=5 7s8]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG ETH SOCK=5 7pa]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG ETH !SUP SOCK=5 7h7]:%DARK_GREEN%%NAME%%YELLOW%
ItemDisplay[NMAG ETH SOCK=5 7wc]:%DARK_GREEN%%NAME% %YELLOW%
//
ItemDisplay[NMAG !ETH SOCK=5 7s8]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG !ETH SOCK=5 7pa]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG !ETH SOCK=5 7h7]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG !ETH SOCK=5 7wc]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG !ETH SOCK=5 7p7]:%WHITE%%NAME% %GRAY%
//
//6 socket polearms
ItemDisplay[NMAG ETH SOCK=6 7h7]:%NAME% %GRAY%
ItemDisplay[NMAG ETH SOCK=6 7wc]:%NAME% %GRAY%
//
ItemDisplay[NMAG !ETH SOCK=6 7h7]:%NAME% %GRAY%
ItemDisplay[NMAG !ETH SOCK=6 7wc]:%NAME% %GRAY%
//
//larzuk
ItemDisplay[NMAG ETH SOCK=0 7h7]:%NAME% %GRAY%
ItemDisplay[NMAG ETH SOCK=0 7wc]:%NAME% %GRAY%
ItemDisplay[NMAG !ETH SOCK=0 7h7]:
ItemDisplay[NMAG !ETH SOCK=0 7wc]:
//
//end-game 2h swords
ItemDisplay[NMAG ETH SOCK=6 7fb]:%NAME% %GRAY%
ItemDisplay[NMAG ETH SOCK=6 7gs]:
ItemDisplay[NMAG ETH SOCK=5 7fb]:%NAME% %GRAY%
ItemDisplay[NMAG ETH SOCK=5 7gd]:%NAME% %GRAY%
ItemDisplay[NMAG ETH SOCK=5 7gs]:
ItemDisplay[NMAG ETH SOCK=4 7fb]:%NAME% %GRAY%
ItemDisplay[NMAG ETH SOCK=4 7gd]:
ItemDisplay[NMAG ETH SOCK=4 7gs]:
ItemDisplay[NMAG ETH SOCK=0 7fb]:%NAME% %GRAY%
ItemDisplay[NMAG ETH SOCK=0 7gs]:
ItemDisplay[NMAG !ETH SOCK=0 7fb]:
ItemDisplay[NMAG !ETH SOCK=0 7gs]:
ItemDisplay[NMAG !ETH SOCK=0 7gd]:
//
//Memory bases +3 ES
ItemDisplay[WP11 NMAG SOCK=4 (SK58=3)]:%RED%+3 Energy Shield%GREEN%Memory Base%MAP-97%%YELLOW%
ItemDisplay[cst NMAG SOCK=0 (SK58=3)]:%RED%+3 Energy Shield%GREEN%Memory Base%MAP-97%%YELLOW%
ItemDisplay[bst NMAG SOCK=0 (SK58=3)]:%RED%+3 Energy Shield%GREEN%Memory Base%MAP-97%%YELLOW%
ItemDisplay[8cs NMAG SOCK=0 (SK58=3)]:%RED%+3 Energy Shield%GREEN%Memory Base%MAP-97%%YELLOW%
ItemDisplay[8bs NMAG SOCK=0 (SK58=3)]:%RED%+3 Energy Shield%GREEN%Memory Base%MAP-97%%YELLOW%
ItemDisplay[6cs NMAG SOCK=0 (SK58=3)]:%RED%+3 Energy Shield%GREEN%Memory Base%MAP-97%%YELLOW%
ItemDisplay[6bs NMAG SOCK=0 (SK58=3)]:%RED%+3 Energy Shield%GREEN%Memory Base%MAP-97%%YELLOW%
ItemDisplay[WP11 NMAG SOCK=4 (SK58=2)]://%GRAY%+2 Energy Shield%WHITE%Memory Base%GRAY%
ItemDisplay[cst NMAG SOCK=0 (SK58=2)]://%GRAY%+2 Energy Shield%WHITE%Memory Base%GRAY%
ItemDisplay[bst NMAG SOCK=0 (SK58=2)]://%GRAY%+2 Energy Shield%WHITE%Memory Base%GRAY%
ItemDisplay[8cs NMAG SOCK=0 (SK58=2)]://%GRAY%+2 Energy Shield%WHITE%Memory Base%GRAY%
ItemDisplay[8bs NMAG SOCK=0 (SK58=2)]://%GRAY%+2 Energy Shield%WHITE%Memory Base%GRAY%
ItemDisplay[6cs NMAG SOCK=0 (SK58=2)]://%GRAY%+2 Energy Shield%WHITE%Memory Base%GRAY%
ItemDisplay[6bs NMAG SOCK=0 (SK58=2)]://%GRAY%+2 Energy Shield%WHITE%Memory Base%GRAY%
//
//ETH Staves for Insight for Shockwave Druids
ItemDisplay[6bs NMAG ETH SOCK=0]:%GRAY%%NAME% %GRAY%
ItemDisplay[6cs NMAG ETH SOCK=0]:%GRAY%%NAME% %GRAY%
ItemDisplay[6bs NMAG ETH SOCK=4]:%GRAY%%NAME% %GRAY%
ItemDisplay[6cs NMAG ETH SOCK=4]:%GRAY%%NAME% %GRAY%
ItemDisplay[6ws NMAG ETH SOCK=4]:%GRAY%%NAME% %GRAY%
//
//ETH Archon Staff, 6os ETH Archon Staff = BoTD = Breath of the Dying
ItemDisplay[6ws NMAG ETH SOCK=0]:%GRAY%%NAME% %GRAY%
ItemDisplay[6ws NMAG ETH SOCK=6]:%GRAY%%NAME% %GRAY%
//
//5OS Crystal Sword, War Scepter, Flail = CTA = Call to Arms, 5 OS Double Axe = Beast
ItemDisplay[crs NMAG SOCK=5]:%GRAY%%NAME% %GRAY%
ItemDisplay[wsp NMAG SOCK=5]:%GRAY%%NAME% %GRAY%
ItemDisplay[fla NMAG SOCK=5]:%GRAY%%NAME% %GRAY%
ItemDisplay[2ax NMAG SOCK=5]:%GRAY%%NAME% %GRAY%
//Merc Beast
ItemDisplay[7gm ETH NMAG SOCK=5]:%GREEN%%NAME%%MAP-97% %RED%
//
//Hand of Justice
ItemDisplay[7ws NMAG SOCK=4 (SK118=3)]:%RED%+3 Holy Shock %DARK_GREEN%Hand of Justice base %YELLOW%
ItemDisplay[7ws NMAG SOCK=4]:%GRAY%%NAME% %GRAY%
ItemDisplay[7ws NMAG SOCK=0]:%GRAY%%NAME%
//
//4os Flail, Larzuk Gaurantee = HOTO = Heart of the Oak
ItemDisplay[fla NMAG ETH SOCK=4]:%DARK_GREEN%%NAME%%MAP-97% %YELLOW%
ItemDisplay[fla NMAG !ETH SOCK=4]:%DARK_GREEN%%NAME%%MAP-97% %GRAY%
//
//5os Phase Blade, Zerker Axe = Grief
ItemDisplay[7cr NMAG SOCK=5]:%DARK_GREEN%%NAME%%MAP-97% %YELLOW%
ItemDisplay[7wa NMAG !ETH SOCK=5]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[7wa NMAG ETH SOCK=5]:%DARK_GREEN%%NAME% %YELLOW%
//
//Silence
ItemDisplay[7cr !ETH NMAG SOCK=6]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[7cr ETH NMAG SOCK=6]:%DARK_GREEN%%NAME% %GRAY%
//
//Breath of the Dying = BotD
ItemDisplay[7wa ETH NMAG SOCK=0]:%GREEN%%NAME%%MAP-97% %RED%
ItemDisplay[7wa ETH NMAG SOCK=6]:%GREEN%%NAME%%MAP-97% %RED%
ItemDisplay[7wa ETH NMAG SOCK=5]:%GREEN%%NAME%%MAP-97% %RED%
ItemDisplay[7gd ETH NMAG SOCK=0]:%DARK_GREEN%%NAME%%MAP-97% %YELLOW%
ItemDisplay[7gd ETH NMAG SOCK=6]:%DARK_GREEN%%NAME%%MAP-97% %YELLOW%
ItemDisplay[7gd ETH NMAG SOCK=5]:%DARK_GREEN%%NAME%%MAP-97% %YELLOW%
ItemDisplay[7p7 ETH NMAG SOCK=0]:%GREEN%ETH %NAME%%MAP-97% %RED%
ItemDisplay[7p7 ETH NMAG SOCK=6]:%GREEN%ETH %NAME%%MAP-97% %RED%
ItemDisplay[7p7 ETH NMAG SOCK=5]:%GREEN%ETH %NAME%%MAP-97% %RED%
ItemDisplay[7gm ETH NMAG SOCK=0]:%GREEN%ETH %NAME%%MAP-97% %RED%
ItemDisplay[7gm ETH NMAG SOCK=6]:%GREEN%ETH %NAME%%MAP-97% %RED%
//
ItemDisplay[ame ETH NMAG TABSK2=3 SOCK=0]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[ame ETH NMAG TABSK2=3 SOCK=6]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[ame ETH NMAG SOCK=0]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[ame ETH NMAG SOCK=6]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[amd ETH NMAG TABSK2=3 SOCK=0]:%DARK_GREEN%ETH %NAME% %GRAY%
ItemDisplay[amd ETH NMAG TABSK2=3 SOCK=6]:%DARK_GREEN%ETH %NAME% %GRAY%
ItemDisplay[amd ETH NMAG SOCK=0]:%GRAY%%NAME% %GRAY%
ItemDisplay[amd ETH NMAG SOCK=6]:%GRAY%%NAME% %GRAY%
//
//Dream/Delirium
//Low Str 3SOC Masks (NON ETH)
ItemDisplay[NMAG SOCK=3 !ETH msk]://%NAME% 
ItemDisplay[NMAG SOCK=3 !ETH xsk]://%NAME% 
//
//103-106 str helms for archon plate builds
ItemDisplay[NMAG SOCK=3 !ETH usk]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[NMAG SOCK=3 !ETH uh9]:%DARK_GREEN%%NAME% %YELLOW%
//
//Low STR LORE base - ILVL appropriate
ItemDisplay[NMAG SOCK=2 !ETH cap ILVL<20]:%NAME% 
ItemDisplay[NMAG SOCK=2 !ETH skp ILVL<20]:%NAME% 
ItemDisplay[NMAG SOCK=2 !ETH hlm ILVL<20]:%NAME% 
ItemDisplay[NMAG SOCK=2 !ETH msk ILVL<45]:%NAME% 
ItemDisplay[NMAG SOCK=2 !ETH bhm ILVL<45]:%NAME% 
ItemDisplay[NMAG SOCK=2 !ETH xap ILVL<45]:%NAME% 
ItemDisplay[NMAG SOCK=2 !ETH xkp ILVL<45]:%NAME% 
ItemDisplay[NMAG SOCK=2 !ETH xsk ILVL<45]:%NAME% 
ItemDisplay[NMAG SOCK=2 !ETH xh9 ILVL<45]:%NAME% 
//
//Plague
ItemDisplay[obf NMAG SOCK=3 (SK62=3)]:%DARK_GREEN%+3 hydra orb%MAP-97% %YELLOW%
ItemDisplay[obf NMAG SOCK=3 (SK59=3)]:%DARK_GREEN%+3 blizzard orb%MAP-97% %YELLOW%
ItemDisplay[obf NMAG SOCK=3 (SK64=3)]:%DARK_GREEN%+3 forb orb%MAP-97% %YELLOW%
ItemDisplay[obf NMAG SOCK=3 (SK48=3)]:%DARK_GREEN%+3 nova%MAP-97% %YELLOW%
ItemDisplay[oba NMAG SOCK=3 (SK62=3)]:%DARK_GREEN%+3 hydra orb%MAP-97% %YELLOW%
ItemDisplay[oba NMAG SOCK=3 (SK59=3)]:%DARK_GREEN%+3 blizzard orb%MAP-97% %YELLOW%
ItemDisplay[oba NMAG SOCK=3 (SK64=3)]:%DARK_GREEN%+3 forb orb%MAP-97% %YELLOW%
ItemDisplay[oba NMAG SOCK=3 (SK48=3)]:%DARK_GREEN%+3 nova%MAP-97% %YELLOW%
ItemDisplay[ob5 NMAG SOCK=3 (SK62=3)]:%DARK_GREEN%+3 hydra orb%MAP-97% %YELLOW%
ItemDisplay[ob5 NMAG SOCK=3 (SK59=3)]:%DARK_GREEN%+3 blizzard orb%MAP-97% %YELLOW%
ItemDisplay[ob5 NMAG SOCK=3 (SK64=3)]:%DARK_GREEN%+3 forb orb%MAP-97% %YELLOW%
ItemDisplay[ob5 NMAG SOCK=3 (SK48=3)]:%DARK_GREEN%+3 nova%MAP-97% %YELLOW%
ItemDisplay[obf NMAG SOCK=0 (SK62=3)]:%DARK_GREEN%+3 hydra orb%MAP-97% %YELLOW%
ItemDisplay[obf NMAG SOCK=0 (SK59=3)]:%DARK_GREEN%+3 blizzard orb%MAP-97% %YELLOW%
ItemDisplay[obf NMAG SOCK=0 (SK64=3)]:%DARK_GREEN%+3 forb orb%MAP-97% %YELLOW%
ItemDisplay[obf NMAG SOCK=0 (SK48=3)]:%DARK_GREEN%+3 nova%MAP-97% %YELLOW%
ItemDisplay[oba NMAG SOCK=0 (SK62=3)]:%DARK_GREEN%+3 hydra orb%MAP-97% %YELLOW%
ItemDisplay[oba NMAG SOCK=0 (SK59=3)]:%DARK_GREEN%+3 blizzard orb%MAP-97% %YELLOW%
ItemDisplay[oba NMAG SOCK=0 (SK64=3)]:%DARK_GREEN%+3 forb orb%MAP-97% %YELLOW%
ItemDisplay[oba NMAG SOCK=0 (SK48=3)]:%DARK_GREEN%+3 nova%MAP-97% %YELLOW%
ItemDisplay[ob5 NMAG SOCK=0 (SK62=3)]:%DARK_GREEN%+3 hydra orb%MAP-97% %YELLOW%
ItemDisplay[ob5 NMAG SOCK=0 (SK59=3)]:%DARK_GREEN%+3 blizzard orb%MAP-97% %YELLOW%
ItemDisplay[ob5 NMAG SOCK=0 (SK64=3)]:%DARK_GREEN%+3 forb orb %MAP-97%%YELLOW%
ItemDisplay[ob5 NMAG SOCK=0 (SK48=3)]:%DARK_GREEN%+3 nova%MAP-97% %YELLOW%
//
//Death
ItemDisplay[7fb ETH NMAG SOCK=0]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[7wa ETH NMAG SOCK=5]:%DARK_GREEN%%NAME% %RED%
ItemDisplay[7fb ETH NMAG SOCK=5]:%DARK_GREEN%%NAME% %RED%
ItemDisplay[7gd ETH NMAG SOCK=5]:%DARK_GREEN%%NAME% %RED%
ItemDisplay[7gi ETH NMAG SOCK=0]:%GRAY%%NAME% %GRAY%
ItemDisplay[7gi ETH NMAG SOCK=5]:%GRAY%%NAME% %GRAY%
//
//Bow Bases
ItemDisplay[amc SOCK=4 SUP NMAG TABSK0=3]:%DARK_GREEN%+3 SUP GMBow%MAP-97% %YELLOW%
ItemDisplay[amb SOCK=4 SUP NMAG TABSK0=3]:%DARK_GREEN%+3 SUP MBow %YELLOW%
ItemDisplay[amc SOCK=3 SUP NMAG TABSK0=3]:%DARK_GREEN%+3 SUP GMBow%MAP-97% %YELLOW%
ItemDisplay[amb SOCK=3 SUP NMAG TABSK0=3]:%DARK_GREEN%+3 SUP MBow %YELLOW%
ItemDisplay[amc SOCK=4 !SUP NMAG TABSK0=3]:%DARK_GREEN%+3 GMBow%MAP-97% %YELLOW%
ItemDisplay[amb SOCK=4 !SUP NMAG TABSK0=3]:%DARK_GREEN%+3 MBow %GRAY%
ItemDisplay[amc SOCK=3 !SUP NMAG TABSK0=3]:%DARK_GREEN%+3 GMBow%MAP-97% %YELLOW%
ItemDisplay[amb SOCK=3 !SUP NMAG TABSK0=3]:%DARK_GREEN%+3 MBow %GRAY%
ItemDisplay[amb SOCK=0 !SUP NMAG TABSK0=3]:%DARK_GREEN%+3 Mbow %GRAY%
ItemDisplay[amc SOCK=0 !SUP NMAG TABSK0=3]:%DARK_GREEN%+3 GMBow%MAP-97% %YELLOW%
ItemDisplay[amc NMAG SOCK=4]://%GRAY%GMBow
ItemDisplay[amc !SUP NMAG SOCK=0]://%GRAY%GMBow
ItemDisplay[NMAG 6hx SOCK=4]:%GRAY%%NAME%
ItemDisplay[6lb NMAG SOCK=4]:%GRAY%%NAME%
ItemDisplay[6l7 NMAG SOCK=4]:%GRAY%%NAME%
ItemDisplay[6cb NMAG SOCK=4]:%GRAY%%NAME%
ItemDisplay[6s7 NMAG SOCK=4]:%GRAY%%NAME%
ItemDisplay[6hb NMAG SOCK=4]:%GRAY%%NAME% 
ItemDisplay[6lb NMAG SOCK=0]:
ItemDisplay[6l7 NMAG SOCK=0]:
ItemDisplay[6cb NMAG SOCK=0]:
ItemDisplay[6s7 NMAG SOCK=0]: 
ItemDisplay[6hb NMAG SOCK=0]:
//
//Last Wish
//6os Berserker Axe, Phase Blade, Thunder Maul = LW = Last Wish
ItemDisplay[NMAG 7cr !ETH SOCK=6]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[NMAG 7wa !ETH SOCK=6]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[NMAG 7gm !ETH SOCK=6]:%DARK_GREEN%%NAME% %GRAY%
//
//Lawbringer
ItemDisplay[7cr NMAG SOCK=3]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[72h ETH NMAG SOCK=3]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[72h ETH NMAG SOCK=0]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[7ls ETH NMAG SOCK=3]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[7ls ETH NMAG SOCK=0]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[7ls NMAG SOCK=3]:
ItemDisplay[7bs ETH NMAG SOCK=3]:
ItemDisplay[7bs ETH NMAG SOCK=0]:
ItemDisplay[7bs NMAG SOCK=3]:
ItemDisplay[7wd ETH NMAG SOCK=3]:
ItemDisplay[7wd ETH NMAG SOCK=0]:
ItemDisplay[7wd NMAG SOCK=3]:
//
//Oath
ItemDisplay[7wa ETH NMAG SOCK=4]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[7fb ETH NMAG SOCK=4]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[7gd ETH NMAG SOCK=4]:%DARK_GREEN%%NAME% %YELLOW%
ItemDisplay[7fl ETH NMAG SOCK=4]:%DARK_GREEN%%NAME% %YELLOW%
//
//Fortitude Weapon
ItemDisplay[72a ETH NMAG SOCK=4]:%DARK_GREEN%%NAME% %YELLOW%
//
//non-magic wands 
ItemDisplay[WP12 NMAG !wnd !ywn !9wn !SOCK=1 (SK74=3)]:%DARK_GREEN%+3 Corpse Explosion wand%GRAY%
ItemDisplay[WP12 NMAG !wnd !ywn !9wn !SOCK=1 (SK84=3)]:%DARK_GREEN%+3 Bone Spear wand%GRAY%
ItemDisplay[WP12 NMAG !wnd !ywn !9wn !SOCK=1 (SK83=3)]:%DARK_GREEN%+3 Desecrate wand%GRAY%
ItemDisplay[WP12 NMAG !wnd !ywn !9wn !SOCK=1 (SK92=3)]:%GRAY%+3 poison nova wand%GRAY%
ItemDisplay[WP12 NMAG !wnd !ywn !9wn !SOCK=1 (SK67=3)]:%DARK_GREEN%+3 teeth wand%GRAY%
ItemDisplay[WP12 NMAG !wnd !ywn !9wn !SOCK=1 (SK80=3)]:%GRAY%+3 skele mage wand%GRAY%
ItemDisplay[WP12 NMAG !wnd !ywn !9wn !SOCK=1 (SK70=3)]:%GRAY%+3 skele war wand%GRAY%
//
//non-magic necro heads 
ItemDisplay[CL4 NMAG (SK74=3) !ETH !SOCK=1]:%DARK_GREEN%+3 Corpse Explosion head%GRAY%
ItemDisplay[CL4 NMAG (SK80=3) !ETH !SOCK=1]:%GRAY%+3 skele mage head%GRAY%
ItemDisplay[CL4 NMAG (SK70=3) !ETH !SOCK=1]:%GRAY%+3 skele head%GRAY%
ItemDisplay[CL4 NMAG (SK69=3) !ETH !SOCK=1]:%GRAY%+3 mastery head%GRAY%
ItemDisplay[CL4 NMAG (SK67=3) !ETH !SOCK=1]:%GRAY%+3 teeth head%GRAY%
ItemDisplay[CL4 NMAG (SK83=3) !ETH !SOCK=1]:%GRAY%+3 desecrate head%GRAY%
ItemDisplay[CL4 NMAG (SK84=3) !ETH !SOCK=1]:%GRAY%+3 bone spear head%GRAY%
ItemDisplay[CL4 NMAG (SK92=3) !ETH !SOCK=1]:%GRAY%+3 poison nova head%GRAY%
ItemDisplay[CL4 NMAG (SK74=2) !ETH !SOCK=1]:%GRAY%+2 Corpse Explosion head%GRAY%
//
//non-magic druid pelts 
ItemDisplay[CL1 NMAG (SK244=3) !SOCK=1]:%GRAY%+3 Volcano Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK249=3) !SOCK=1]:%GRAY%+3 Armageddon Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK250=3) !SOCK=1]:%GRAY%+3 Hurricane Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK240=3) !SOCK=1]:%GRAY%+3 Twister Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK245=3) !SOCK=1]:%GRAY%+3 Nado Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK237=3) !SOCK=1]:%GRAY%+3 Dire Wolf Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK247=3) !SOCK=1]:%GRAY%+3 Grizzly Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK227=3) !SOCK=1]:%GRAY%+3 Spirit Wolf Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK243=3) !SOCK=1]:%GRAY%+3 Shockwave Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK238=3) !SOCK=1]:%GRAY%+3 Rabies Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK239=3) !SOCK=1]:%GRAY%+3 Fireclaw Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK221=3) !SOCK=1 CLVL<90]:%DARK_GREEN%+3 Raven Pelt%MAP-97% %GRAY%
ItemDisplay[CL1 NMAG (SK221=2) !SOCK=1 CLVL<61]:%DARK_GREEN%+2 Raven Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK221=1) !SOCK=1 CLVL<21]:%DARK_GREEN%+1 Raven Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK225=3) !SOCK=1 CLVL<90]:%DARK_GREEN%+3 Firestorm Pelt%MAP-97% %GRAY%
ItemDisplay[CL1 NMAG (SK225=2) !SOCK=1 CLVL<61]:%DARK_GREEN%+2 Firestorm Pelt %GRAY%
ItemDisplay[CL1 NMAG (SK225=1) !SOCK=1 CLVL<21]:%DARK_GREEN%+1 Firestorm Pelt %GRAY%
//
//non-magic barbarian primal helms (barb)
ItemDisplay[CL2 NMAG (SK154=3) !SOCK=1 CLVL<95]:%DARK_GREEN%+3 warcry helm%GRAY%
ItemDisplay[CL2 NMAG (SK149=3) !SOCK=1 CLVL<95]:%DARK_GREEN%+3 bo helm%GRAY%
ItemDisplay[CL2 NMAG (SK154>0) !SOCK=1 CLVL<90]:%GRAY%warcry helm%GRAY%
ItemDisplay[CL2 NMAG (SK149>0) !SOCK=1 CLVL<90]:%GRAY%bo helm%GRAY%
ItemDisplay[CL2 NMAG (SK153>0) !SOCK=1 CLVL<61]:%GRAY%nat res helm%GRAY%
ItemDisplay[CL2 NMAG (SK150>0) !SOCK=1 CLVL<61]:%GRAY%grim ward helm%GRAY%
ItemDisplay[CL2 NMAG (SK142>0) !SOCK=1 CLVL<61]:%GRAY%find item helm%GRAY%
ItemDisplay[CL2 NMAG (SK138>0) !SOCK=1 CLVL<21]:%GRAY%shout helm%GRAY%
ItemDisplay[CL2 NMAG]:
//
//Scepters
ItemDisplay[WP13 NMAG SOCK=4]://%GRAY%%NAME% %GRAY%
ItemDisplay[WP13 NMAG SOCK=5 (SK117>0)]://%WHITE%Holy Shield cta base%WHITE%
ItemDisplay[WP13 NMAG (SK121=3 AND SK123=3 AND SK117>0) !SOCK=1 !SOCK=2]:%NAME% %YELLOW%
ItemDisplay[WP13 NMAG (SK121=3 AND SK123=3 AND SK124=3) !SOCK=1 !SOCK=2]:%NAME% %YELLOW%
ItemDisplay[WP13 NMAG (SK121=3 AND SK123=3 AND SK115=3) !SOCK=1 !SOCK=2]:%NAME% %YELLOW%
//
//CTA staff
ItemDisplay[WP11 NMAG SOCK=5 (SK58>1 AND SK57>0)]:%NAME% %YELLOW%
ItemDisplay[WP11 NMAG SOCK=5 (SK58>1 AND SK50>0)]:%NAME% %YELLOW%
ItemDisplay[WP11 NMAG SOCK=5 (SK57>0 AND SK50>0)]:%NAME% %YELLOW%
ItemDisplay[WP11 NMAG SOCK=5 SK57>0]:%NAME% %YELLOW%
ItemDisplay[WP11 NMAG SOCK=5 SK50>0]:%NAME% %YELLOW%
ItemDisplay[WP11 NMAG SOCK=5 (SK58=3)]:%DARK_GREEN% +3 Energy Shield CTA base%MAP-97% %YELLOW%
//
//Melody bow bases
ItemDisplay[amb SOCK=3 NMAG]:%DARK_GREEN%%NAME% %GRAY%
ItemDisplay[amc SOCK=3 NMAG]:%DARK_GREEN%%NAME% %GRAY%
//
//Hide bases with no mods
ItemDisplay[(CL1 OR CL2 OR CL3 OR CL4 OR CL5 OR CL6 OR CL7) NMAG]:
//╔══════════╗
//║ Leveling ║
//╚══════════╝
//Generic
ItemDisplay[RARE ILVL<15]:%NAME%
ItemDisplay[!RW NORM NMAG ILVL<15 SOCK>0 ETH (ARMOR OR WEAPON)]:%NAME% 
ItemDisplay[!RW NORM NMAG ILVL<15 SOCK=0 ETH (ARMOR OR WEAPON)]:%NAME%
ItemDisplay[!RW NORM NMAG ILVL<15 SOCK>0 (ARMOR OR WEAPON)]:%NAME% 
ItemDisplay[!RW NORM NMAG ILVL<15 SOCK>0 (ARMOR OR WEAPON)]:%NAME% 
ItemDisplay[!RW NORM NMAG ILVL<15 (ARMOR OR WEAPON)]:%NAME%
ItemDisplay[ILVL<50 SOCK>1 !RW NMAG (ARMOR OR WEAPON)]:%NAME% 
ItemDisplay[ILVL<26 NORM MAG (ARMOR OR WEAPON) !ID]:%NAME%
ItemDisplay[ILVL>25 SOCK<2 NORM MAG (ARMOR OR WEAPON) !ID]:
ItemDisplay[ILVL>25 NORM MAG (ARMOR OR WEAPON) ID]:%NAME%
ItemDisplay[ILVL>0 ILVL<35 NORM RARE !ID (ARMOR OR WEAPON)]:%NAME%
ItemDisplay[ILVL>35 !ID NORM RARE !EQ1 !EQ4 !EQ5 !EQ6 !EQ7 !WP11 !WP12 !WP13]:
ItemDisplay[ILVL>65 !ID EXC RARE !EQ1 !EQ4 !EQ5 !EQ6 !EQ7 !WP11 !WP12 !WP13]:
ItemDisplay[ILVL<31 EXC MAG WEAPON !ID]:%NAME%
ItemDisplay[ILVL>30 !ID EXC MAG WEAPON !ID ]:
ItemDisplay[ILVL>30 EXC MAG WEAPON ID]:%NAME%
ItemDisplay[ILVL<66 EXC MAG ARMOR !ID]:%NAME%
ItemDisplay[ILVL<66 EXC MAG ARMOR ID]:%NAME%
ItemDisplay[ILVL<66 EXC RARE (ARMOR OR WEAPON)]:%NAME%
ItemDisplay[ILVL<66 ELT MAG ARMOR !ID]:%NAME%
ItemDisplay[ILVL<66 ELT MAG ARMOR ID]:%NAME%
ItemDisplay[ILVL<66 ELT RARE (ARMOR OR WEAPON)]:%NAME%
//
//None of the Above
//Weapons:Axe, Mace, Sword, Dagger, Throwing Weapon, Javelin, Spear, Polearm, Bow, Crossbow
ItemDisplay[MAG WP1 !ID]:
ItemDisplay[MAG WP2 !ID]:
ItemDisplay[MAG WP3 !ID]:
ItemDisplay[MAG WP4 !ID]:
ItemDisplay[MAG WP5 !ID]:
ItemDisplay[MAG WP6 !ID]:
ItemDisplay[MAG WP7 !ID]:
ItemDisplay[MAG WP8 !ID]:
ItemDisplay[MAG WP9 !ID]:
ItemDisplay[MAG WP10 !ID]:
//
//Armor:Helm, Body, Shield, Boot, Belt (ilvl 61+)
//Elite Helm - Shown
ItemDisplay[ELT MAG EQ1 !ID ILVL>60]:
//Non Elite Helm - Hidden
ItemDisplay[!ELT MAG EQ1 !ID ILVL>60]:
//
//Elite Armor - Shown
ItemDisplay[ELT MAG EQ2 !ID ILVL>60]:
//Non Elite Armor - Hidden
ItemDisplay[!ELT MAG EQ2 !ID ILVL>60]:
//
//Shields - Hidden !monarch !troll nest
ItemDisplay[MAG EQ3 !ID !uit !ush ILVL>60]:
//
//Elite Boots - Shown
ItemDisplay[ELT MAG EQ5 !ID ILVL>60]:
//Non Elite Boots - Hidden
ItemDisplay[MAG xhb !ID ILVL>60]:
ItemDisplay[MAG hbt !ID ILVL>60]:
ItemDisplay[MAG utb !ID ILVL>60]:
ItemDisplay[MAG xtb !ID ILVL>60]:
ItemDisplay[MAG tbt !ID ILVL>60]:
ItemDisplay[MAG umb !ID ILVL>60]:
ItemDisplay[MAG xmb !ID ILVL>60]:
ItemDisplay[MAG mbt !ID ILVL>60]:
ItemDisplay[MAG uvb !ID ILVL>60]:
ItemDisplay[MAG xvb !ID ILVL>60]:
ItemDisplay[MAG vbt !ID ILVL>60]:
ItemDisplay[MAG xlb !ID ILVL>60]:
ItemDisplay[MAG lbt !ID ILVL>60]:
//
//Elite Belts - Shown
ItemDisplay[ELT MAG EQ6 !ID ILVL>60]:
//Non Elite Belts - Hidden
ItemDisplay[MAG uhc !ID ILVL>60]:
ItemDisplay[MAG zhb !ID ILVL>60]:
ItemDisplay[MAG hbl !ID ILVL>60]:
ItemDisplay[MAG utc !ID ILVL>60]:
ItemDisplay[MAG ztb !ID ILVL>60]:
ItemDisplay[MAG tbl !ID ILVL>60]:
ItemDisplay[MAG mbl !ID ILVL>60]:
ItemDisplay[MAG vbl !ID ILVL>60]:
ItemDisplay[MAG ulc !ID ILVL>60]:
ItemDisplay[MAG zlb !ID ILVL>60]:
ItemDisplay[MAG lbl !ID ILVL>60]:
//
//Gloves
ItemDisplay[MAG xhg !ID ILVL>60]:
ItemDisplay[MAG xlg !ID ILVL>60]:
ItemDisplay[MAG ulg !ID ILVL>60]:
ItemDisplay[MAG utg !ID ILVL>60]:
ItemDisplay[MAG xtg !ID ILVL>60]:
//
//Normal
//Vendor Items
ItemDisplay[NMAG WP11]:
ItemDisplay[NMAG WP12]:
ItemDisplay[NMAG WP13]:
ItemDisplay[NMAG CL4]:
ItemDisplay[NMAG CL6]:
 //
//None of the Above
//Weapons:Axe, Mace, Sword, Dagger, Throwing Weapon, Javelin, Spear, Polearm, Bow, Crossbow
//
//AXE
ItemDisplay[NMAG !RW ILVL>14 hax]:
ItemDisplay[NMAG !RW ILVL>30 9ha]:
ItemDisplay[NMAG !RW ILVL>60 7ha]:
ItemDisplay[NMAG !RW ILVL>14 axe]:
ItemDisplay[NMAG !RW ILVL>30 9ax]:
ItemDisplay[NMAG !RW ILVL>60 7ax]:
ItemDisplay[NMAG !RW ILVL>14 2ax]:
ItemDisplay[NMAG !RW ILVL>30 92a]:
ItemDisplay[NMAG !RW ILVL>60 72a]:
ItemDisplay[NMAG !RW ILVL>14 mpi]:
ItemDisplay[NMAG !RW ILVL>30 9mp]:
ItemDisplay[NMAG !RW ILVL>60 7mp]:
ItemDisplay[NMAG !RW ILVL>14 wax]:
ItemDisplay[NMAG !RW ILVL>30 9wa]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=1 7wa]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=2 7wa]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=3 7wa]:
//
ItemDisplay[NMAG !RW ILVL>14 lax]:
ItemDisplay[NMAG !RW ILVL>30 9la]:
ItemDisplay[NMAG !RW ILVL>60 7la]:
ItemDisplay[NMAG !RW ILVL>14 bax]:
ItemDisplay[NMAG !RW ILVL>30 9ba]:
ItemDisplay[NMAG !RW ILVL>60 7ba]:
ItemDisplay[NMAG !RW ILVL>14 btx]:
ItemDisplay[NMAG !RW ILVL>30 9bt]:
ItemDisplay[NMAG !RW ILVL>60 7bt]:
ItemDisplay[NMAG !RW ILVL>14 gax]:
ItemDisplay[NMAG !RW ILVL>30 9ga]:
ItemDisplay[NMAG !RW ILVL>60 7ga]:
ItemDisplay[NMAG !RW ILVL>14 gix]:
ItemDisplay[NMAG !RW ILVL>39 9gi]:
ItemDisplay[NMAG !RW ILVL>60 7gi]:

//MACE
ItemDisplay[NMAG !RW ILVL>14 clb]:
ItemDisplay[NMAG !RW ILVL>25 9cl]:
ItemDisplay[NMAG !RW ILVL>60 7cl]:
ItemDisplay[NMAG !RW ILVL>14 spc]:
ItemDisplay[NMAG !RW ILVL>25 9sp]:
ItemDisplay[NMAG !RW ILVL>60 7sp]:
ItemDisplay[NMAG !RW ILVL>14 mac]:
ItemDisplay[NMAG !RW ILVL>25 9ma]:
ItemDisplay[NMAG !RW ILVL>60 7ma]:
ItemDisplay[NMAG !RW ILVL>14 mst]:
ItemDisplay[NMAG !RW ILVL>60 7mt]:
ItemDisplay[NMAG !RW ILVL>25 9mt]:
ItemDisplay[NMAG !RW ILVL<26 SOCK=0 fla]:
ItemDisplay[NMAG !RW ILVL>40 SOCK=0 fla]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 fla]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 fla]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 fla]:
//
ItemDisplay[NMAG !RW ILVL>25 9fl]:
ItemDisplay[NMAG !RW ILVL>60 7fl]:
ItemDisplay[NMAG !RW ILVL>14 whm]:
ItemDisplay[NMAG !RW ILVL>25 9wh]:
ItemDisplay[NMAG !RW ILVL>60 7wh]:
ItemDisplay[NMAG !RW ILVL>14 mau]:
ItemDisplay[NMAG !RW ILVL>25 9m9]:
ItemDisplay[NMAG !RW ILVL>60 7m7]:
ItemDisplay[NMAG !RW ILVL>14 gma]:
ItemDisplay[NMAG !RW ILVL>25 9gm]:
ItemDisplay[NMAG !RW ILVL>60 7gm]:
//
//SWORDS
ItemDisplay[NMAG !RW ILVL<26 SOCK=0 lsd]:
ItemDisplay[NMAG !RW ILVL>40 SOCK=0 lsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 lsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 lsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 lsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 lsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 lsd]:
ItemDisplay[NMAG !RW ILVL<26 SOCK=0 bsd]:
ItemDisplay[NMAG !RW ILVL>40 SOCK=0 bsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 bsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 bsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 bsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 bsd]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 bsd]:
ItemDisplay[NMAG !RW ILVL<26 SOCK=0 crs]:
ItemDisplay[NMAG !RW ILVL>40 SOCK=0 crs]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 crs]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 crs]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 crs]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 crs]:
ItemDisplay[NMAG !RW ILVL>14 ssd]:
ItemDisplay[NMAG !RW ILVL>25 9ss]:
ItemDisplay[NMAG !RW ILVL>60 7ss]:
ItemDisplay[NMAG !RW ILVL>14 scm]:
ItemDisplay[NMAG !RW ILVL>25 9sm]:
ItemDisplay[NMAG !RW ILVL>60 7sm]:
ItemDisplay[NMAG !RW ILVL>14 sbr]:
ItemDisplay[NMAG !RW ILVL>25 9sb]:
ItemDisplay[NMAG !RW ILVL>60 7sb]:
ItemDisplay[NMAG !RW ILVL>14 flc]:
ItemDisplay[NMAG !RW ILVL>25 9fc]:
ItemDisplay[NMAG !RW ILVL>60 7fc]:
ItemDisplay[NMAG !RW ILVL>25 9cr]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=0 7cr]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=1 7cr]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=2 7cr]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=4 7cr]:
//
ItemDisplay[NMAG !RW ILVL>25 9bs]:
ItemDisplay[NMAG !RW ILVL>60 7bs]:
ItemDisplay[NMAG !RW ILVL>25 9ls]:
ItemDisplay[NMAG !RW ILVL>60 7ls]:
ItemDisplay[NMAG !RW ILVL>14 wsd]:
ItemDisplay[NMAG !RW ILVL>25 9wd]:
ItemDisplay[NMAG !RW ILVL>60 7wd]:
ItemDisplay[NMAG !RW ILVL>14 2hs]:
ItemDisplay[NMAG !RW ILVL>25 92h]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=0 72h]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=1 72h]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=2 72h]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=4 72h]:
//
ItemDisplay[NMAG !RW ILVL>14 clm]:
ItemDisplay[NMAG !RW ILVL>25 9cm]:
ItemDisplay[NMAG !RW ILVL>60 7cm]:
ItemDisplay[NMAG !RW ILVL>14 gis]:
ItemDisplay[NMAG !RW ILVL>25 9gs]:
ItemDisplay[NMAG !RW ILVL>60 7gs]:
ItemDisplay[NMAG !RW ILVL>14 bsw]:
ItemDisplay[NMAG !RW ILVL>25 9b9]:
ItemDisplay[NMAG !RW ILVL>60 7gs]:
ItemDisplay[NMAG !RW ILVL>14 bsw]:
ItemDisplay[NMAG !RW ILVL>25 9b9]:
ItemDisplay[NMAG !RW ILVL>60 7b7]:
ItemDisplay[NMAG !RW ILVL>14 flb]:
ItemDisplay[NMAG !RW ILVL>25 9fb]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=0 7fb]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=1 7fb]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=2 7fb]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=3 7fb]:
//
ItemDisplay[NMAG !RW ILVL>14 flb]:
ItemDisplay[NMAG !RW ILVL>25 9fb]:
ItemDisplay[NMAG !RW ILVL>60 7fb]:
ItemDisplay[NMAG !RW ILVL>14 gsd]:
ItemDisplay[NMAG !RW ILVL>25 9gd]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=1 7gd]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=2 7gd]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=3 7gd]:
//
//Dagger
ItemDisplay[NMAG !RW ILVL>14 dgr]:
ItemDisplay[NMAG !RW ILVL>25 9dg]:
ItemDisplay[NMAG !RW ILVL>60 7dg]:
ItemDisplay[NMAG !RW ILVL>14 dir]:
ItemDisplay[NMAG !RW ILVL>25 9di]:
ItemDisplay[NMAG !RW ILVL>60 7di]:
ItemDisplay[NMAG !RW ILVL>14 kri]:
ItemDisplay[NMAG !RW ILVL>25 9kr]:
ItemDisplay[NMAG !RW ILVL>60 7kr]:
ItemDisplay[NMAG !RW ILVL>14 bld]:
ItemDisplay[NMAG !RW ILVL>25 9bl]:
ItemDisplay[NMAG !RW ILVL>60 7bl]:
//
//Throwing
ItemDisplay[NMAG !RW ILVL>14 tkf]:
ItemDisplay[NMAG !RW ILVL>25 9tk]:
ItemDisplay[NMAG !RW ILVL>60 7tk]:
ItemDisplay[NMAG !RW ILVL>14 tax]:
ItemDisplay[NMAG !RW ILVL>25 9ta]:
ItemDisplay[NMAG !RW ILVL>60 7ta]:
ItemDisplay[NMAG !RW ILVL>14 bkf]:
ItemDisplay[NMAG !RW ILVL>25 9bk]:
ItemDisplay[NMAG !RW ILVL>60 7bk]:
ItemDisplay[NMAG !RW ILVL>14 bal]:
ItemDisplay[NMAG !RW ILVL>25 9b8]:
ItemDisplay[NMAG !RW ILVL>60 7b8]:
//
//Javelin
ItemDisplay[NMAG !RW ILVL>14 jav]:
ItemDisplay[NMAG !RW ILVL>25 9ja]:
ItemDisplay[NMAG !RW ILVL>60 7ja]:
ItemDisplay[NMAG !RW ILVL>14 pil]:
ItemDisplay[NMAG !RW ILVL>25 9pi]:
ItemDisplay[NMAG !RW ILVL>60 7pi]:
ItemDisplay[NMAG !RW ILVL>14 ssp]:
ItemDisplay[NMAG !RW ILVL>25 9s9]:
ItemDisplay[NMAG !RW ILVL>60 7s7]:
ItemDisplay[NMAG !RW ILVL>14 glv]:
ItemDisplay[NMAG !RW ILVL>25 9gl]:
ItemDisplay[NMAG !RW ILVL>60 7gl]:
ItemDisplay[NMAG !RW ILVL>14 tsp]:
ItemDisplay[NMAG !RW ILVL>25 9ts]:
ItemDisplay[NMAG !RW ILVL>60 7ts]:
//
//Spear
ItemDisplay[NMAG !RW ILVL>14 spr]:
ItemDisplay[NMAG !RW ILVL>25 9sr]:
ItemDisplay[NMAG !RW ILVL>25 9tr]:
ItemDisplay[NMAG !RW ILVL>60 7sr]:
ItemDisplay[NMAG !RW ILVL>14 tri]:
ItemDisplay[NMAG !RW ILVL>60 7tr]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=0 brn]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 brn]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 brn]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 brn]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 brn]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 brn]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=0 9br]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=1 9br]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=2 9br]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=3 9br]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=5 9br]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=6 9br]:
ItemDisplay[NMAG !RW ILVL>60 7br]:
ItemDisplay[NMAG !RW ILVL>14 spt]:
ItemDisplay[NMAG !RW ILVL>25 9st]:
ItemDisplay[NMAG !RW ILVL>60 7st]:
ItemDisplay[NMAG !RW ILVL>14 pik]:
ItemDisplay[NMAG !RW ILVL>25 9p9]:
//
//Polearm
ItemDisplay[NMAG !RW ILVL>14 bar]:
ItemDisplay[NMAG !RW ILVL>25 9b7]:
ItemDisplay[NMAG !RW ILVL>60 7o7]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=0 vou]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 vou]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 vou]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 vou]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 vou]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 vou]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=0 9vo]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=1 9vo]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=2 9vo]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=3 9vo]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=5 9vo]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=6 9vo]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=1 7vo]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=2 7vo]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=3 7vo]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=5 7vo]:
ItemDisplay[NMAG !RW ILVL>60 SOCK=6 7vo]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=0 scy]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 scy]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 scy]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 scy]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 scy]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 scy]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=0 9s8]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=1 9s8]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=2 9s8]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=3 9s8]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=5 9s8]:
ItemDisplay[NMAG !RW ILVL>25 SOCK=6 9s8]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 7s8]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 7s8]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 7s8]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 7s8]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 7s8]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=0 pax]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 pax]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 pax]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 pax]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 pax]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 pax]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=0 9pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 9pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 9pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 9pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 9pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 9pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 7pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 7pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 7pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 7pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 7pa]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=0 hal]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 hal]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 hal]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 hal]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 hal]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 hal]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=0 9h9]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 9h9]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 9h9]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 9h9]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 9h9]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 9h9]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 7h7]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 7h7]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 7h7]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 7h7]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 7h7]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=0 wsc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 wsc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 wsc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 wsc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 wsc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 wsc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=0 9wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 9wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 9wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 9wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 9wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 9wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=1 7wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=2 7wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=3 7wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=5 7wc]:
ItemDisplay[NMAG !RW ILVL>14 SOCK=6 7wc]:
//
//Bow
ItemDisplay[NMAG !RW ILVL>14 sbw]:
ItemDisplay[NMAG !RW ILVL>14 8sb]:
ItemDisplay[NMAG !RW ILVL>14 6sb]:
ItemDisplay[NMAG !RW ILVL>14 hbw]:
ItemDisplay[NMAG !RW ILVL>14 8hb]:
ItemDisplay[NMAG !RW ILVL>14 6hb]:
ItemDisplay[NMAG !RW ILVL>14 lbw]:
ItemDisplay[NMAG !RW ILVL>14 8lb]:
ItemDisplay[NMAG !RW ILVL>40 6lb]:
ItemDisplay[NMAG !RW ILVL>14 cbw]:
ItemDisplay[NMAG !RW ILVL>14 8cb]:
ItemDisplay[NMAG !RW ILVL>30 6cb]:
ItemDisplay[NMAG !RW ILVL>14 sbb]:
ItemDisplay[NMAG !RW ILVL>14 8s8]:
ItemDisplay[NMAG !RW ILVL>14 6s7]:
ItemDisplay[NMAG !RW ILVL>14 lbb]:
ItemDisplay[NMAG !RW ILVL>14 8l8]:
ItemDisplay[NMAG !RW ILVL>50 6l7]:
ItemDisplay[NMAG !RW ILVL>14 swb]:
ItemDisplay[NMAG !RW ILVL>14 8sw]:
ItemDisplay[NMAG !RW ILVL>14 lwb]:
ItemDisplay[NMAG !RW ILVL>14 8lw]:
ItemDisplay[NMAG !RW ILVL>14 6lw]:
ItemDisplay[NMAG !RW ILVL>50 6sw]:
//
//Crossbow
ItemDisplay[NMAG !RW ILVL>14 lxb]:
ItemDisplay[NMAG !RW ILVL>25 8lx]:
ItemDisplay[NMAG !RW ILVL>60 6lx]:
ItemDisplay[NMAG !RW ILVL>14 mxb]:
ItemDisplay[NMAG !RW ILVL>25 8mx]:
ItemDisplay[NMAG !RW ILVL>60 6mx]:
ItemDisplay[NMAG !RW ILVL>14 hxb]:
ItemDisplay[NMAG !RW ILVL>25 8hx]:
ItemDisplay[NMAG !RW ILVL>60 6hx]:
ItemDisplay[NMAG !RW ILVL>14 rxb]:
ItemDisplay[NMAG !RW ILVL>25 8rx]:
ItemDisplay[NMAG !RW ILVL>60 6rx]:
//
//None of the Above
ItemDisplay[NMAG !RW cap]:
ItemDisplay[NMAG !RW xap]:
ItemDisplay[NMAG !RW uap]:
ItemDisplay[NMAG !RW skp]:
ItemDisplay[NMAG !RW xkp]:
ItemDisplay[NMAG !RW ukp]:
ItemDisplay[NMAG !RW hlm]:
ItemDisplay[NMAG !RW xlm]:
ItemDisplay[NMAG !RW ulm]:
ItemDisplay[NMAG !RW fhl]:
ItemDisplay[NMAG !RW xhl]:
ItemDisplay[NMAG !RW uhl]:
ItemDisplay[NMAG !RW ghm]:
ItemDisplay[NMAG !RW xhm]:
ItemDisplay[NMAG !RW uhm]:
ItemDisplay[NMAG !RW crn]:
ItemDisplay[NMAG !RW xrn]:
ItemDisplay[NMAG !RW urn]:
ItemDisplay[NMAG !RW msk]:
ItemDisplay[NMAG !RW xsk]:
ItemDisplay[NMAG !RW usk]:
ItemDisplay[NMAG !RW bhm]:
ItemDisplay[NMAG !RW xh9]:
ItemDisplay[NMAG !RW uh9]:
//
//Body Armor
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 qui]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xui]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 lea]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 hla]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 stu]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 rng]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 scl]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 chn]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 brs]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 spl]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 plt]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 fld]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 gth]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 ful]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 aar]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 ltp]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xea]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xla]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xtu]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xng]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xcl]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xhn]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xrs]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xpl]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xlt]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xld]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xth]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xul]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xar]:
//
ItemDisplay[NMAG !RW ILVL>44 qui]:
ItemDisplay[NMAG !RW ILVL>44 xui]:
ItemDisplay[NMAG !RW ILVL>44 lea]:
ItemDisplay[NMAG !RW ILVL>44 hla]:
ItemDisplay[NMAG !RW ILVL>44 stu]:
ItemDisplay[NMAG !RW ILVL>44 rng]:
ItemDisplay[NMAG !RW ILVL>44 scl]:
ItemDisplay[NMAG !RW ILVL>44 chn]:
ItemDisplay[NMAG !RW ILVL>44 brs]:
ItemDisplay[NMAG !RW ILVL>44 spl]:
ItemDisplay[NMAG !RW ILVL>44 plt]:
ItemDisplay[NMAG !RW ILVL>44 fld]:
ItemDisplay[NMAG !RW ILVL>44 gth]:
ItemDisplay[NMAG !RW ILVL>44 ful]:
ItemDisplay[NMAG !RW ILVL>44 aar]:
ItemDisplay[NMAG !RW ILVL>44 ltp]:
ItemDisplay[NMAG !RW ILVL>44 xea]:
ItemDisplay[NMAG !RW ILVL>44 xla]:
ItemDisplay[NMAG !RW ILVL>44 xtu]:
ItemDisplay[NMAG !RW ILVL>44 xng]:
ItemDisplay[NMAG !RW ILVL>44 xcl]:
ItemDisplay[NMAG !RW ILVL>44 xhn]:
ItemDisplay[NMAG !RW ILVL>44 xrs]:
ItemDisplay[NMAG !RW ILVL>44 xpl]:
ItemDisplay[NMAG !RW ILVL>44 xlt]:
ItemDisplay[NMAG !RW ILVL>44 xld]:
ItemDisplay[NMAG !RW ILVL>44 xth]:
ItemDisplay[NMAG !RW ILVL>44 xul]:
ItemDisplay[NMAG !RW ILVL>44 xar]:
//
//Shield
ItemDisplay[NMAG ETH !RW SOCK=3 ush]://%DARK_GREEN% ETH %NAME% %YELLOW%
ItemDisplay[NMAG ETH !RW SOCK=3 urg]://%NAME% 
ItemDisplay[NMAG ETH !RW SOCK=0 ush]://%DARK_GREEN% ETH %NAME% %YELLOW%
ItemDisplay[NMAG !ETH !RW SOCK=3 ush]://%GRAY%%NAME% 
ItemDisplay[NMAG !ETH !RW SOCK=2 ush]://%GRAY%%NAME% 
ItemDisplay[NMAG !ETH !RW SOCK=3 urg]://%GRAY%%NAME% 
ItemDisplay[NMAG !ETH !RW SOCK=2 urg]://%GRAY%%NAME% 
ItemDisplay[NMAG !ETH !RW SOCK=0 ush]://%GRAY%%NAME%
ItemDisplay[NMAG !ETH !RW SOCK=0 urg]://%GRAY%%NAME%
ItemDisplay[NMAG SOCK=1 urg]:
ItemDisplay[NMAG SOCK=1 ush]:
ItemDisplay[NMAG SOCK=1 uit]:
ItemDisplay[NMAG SOCK=2 uit]:
//
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 buc]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xuc]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 uuc]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 sml]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xml]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 uml]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 lrg]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xrg]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 kit]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xit]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 tow]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xow]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 uow]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 gts]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xts]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 uts]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 bsh]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xsh]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 spk]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 xpk]:
ItemDisplay[NMAG !RW SOCK<2 ILVL<45 upk]:
//
ItemDisplay[NMAG !RW ILVL>44 buc]:
ItemDisplay[NMAG !RW ILVL>44 xuc]:
ItemDisplay[NMAG !RW ILVL>44 uuc]:
ItemDisplay[NMAG !RW ILVL>44 sml]:
ItemDisplay[NMAG !RW ILVL>44 xml]:
ItemDisplay[NMAG !RW ILVL>44 uml]:
ItemDisplay[NMAG !RW ILVL>44 lrg]:
ItemDisplay[NMAG !RW ILVL>44 xrg]:
ItemDisplay[NMAG !RW ILVL>44 kit]:
ItemDisplay[NMAG !RW ILVL>44 tow]:
ItemDisplay[NMAG !RW ILVL>44 xow]:
ItemDisplay[NMAG !RW ILVL>44 uow]:
ItemDisplay[NMAG !RW ILVL>44 gts]:
ItemDisplay[NMAG !RW ILVL>44 xts]:
ItemDisplay[NMAG !RW ILVL>44 uts]:
ItemDisplay[NMAG !RW ILVL>44 bsh]:
ItemDisplay[NMAG !RW ILVL>44 xsh]:
ItemDisplay[NMAG !RW ILVL>44 spk]:
ItemDisplay[NMAG !RW ILVL>45 xpk]:
ItemDisplay[NMAG !RW ILVL>44 upk]:
//
//Gloves, Boots, Belts, Circlets -> (Disable to Imbue)
ItemDisplay[NMAG EQ4 !RW ILVL>14]:
ItemDisplay[NMAG EQ5 !RW ILVL>14]:
ItemDisplay[NMAG EQ6 !RW ILVL>14]:
ItemDisplay[NMAG ci0 !RW ILVL>14]:
ItemDisplay[NMAG ci1 !RW ILVL>14]:
//
//Class Items (Paladin Shields, Assassin Claws, Amazon Weapons, Necromancer Heads
//Druid Pelts
ItemDisplay[NMAG !RW CL1 SOCK=1]:
ItemDisplay[NMAG !RW CL1 ETH]:
//Barbarian Helms
ItemDisplay[NMAG CL2 !RW SOCK=1]:
ItemDisplay[NMAG CL2 !RW ETH]:
ItemDisplay[NMAG !RW CL2 SOCK>1 !ETH]:
//Paladin Shields
ItemDisplay[NMAG !RW CL3 (SOCK=1 OR RES<20) ILVL>55]:
//Assassin Claws
ItemDisplay[NMAG ktr ILVL>26]:
ItemDisplay[NMAG !RW !RW wrb ILVL>26]:
ItemDisplay[NMAG !RW axf ILVL>26]:
ItemDisplay[NMAG !RW ces ILVL>26]:
ItemDisplay[NMAG !RW clw ILVL>26]:
ItemDisplay[NMAG !RW btl ILVL>26]:
ItemDisplay[NMAG !RW skr ILVL>26]:
ItemDisplay[NMAG !RW 9ar ILVL>59]:
ItemDisplay[NMAG !RW 9wb ILVL>59]:
ItemDisplay[NMAG !RW 9xf ILVL>59]:
ItemDisplay[NMAG !RW 9cs ILVL>59]:
ItemDisplay[NMAG !RW 9qr ILVL>59]:
ItemDisplay[NMAG !RW 7ar ILVL>68]:
ItemDisplay[NMAG !RW 7wb ILVL>68]:
ItemDisplay[NMAG !RW 7xf ILVL>68]:
ItemDisplay[NMAG !RW 7cs ILVL>68]:
ItemDisplay[NMAG !RW 7qr ILVL>68]:
//Amazon Weapons
ItemDisplay[NMAG !RW am1 ILVL>26]:
ItemDisplay[NMAG !RW am2 ILVL>26]:
ItemDisplay[NMAG !RW am3 ILVL>26]:
ItemDisplay[NMAG !RW am4 ILVL>26]:
ItemDisplay[NMAG !RW am5 CLVL>60]:
ItemDisplay[NMAG !RW am6 ILVL>59]:
ItemDisplay[NMAG !RW am7 ILVL>59]:
ItemDisplay[NMAG !RW am8 ILVL>59]:
ItemDisplay[NMAG !RW am9 ILVL>59]:
ItemDisplay[NMAG !RW ama ILVL>59]:
ItemDisplay[NMAG !RW amf ILVL>59]:
ItemDisplay[NMAG !RW amd ILVL>59]:
ItemDisplay[NMAG !RW amb ILVL>59]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=1 amc]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=2 amc]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=3 amc]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=5 amc]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=6 amc]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=1 ame]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=2 ame]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=3 ame]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=5 ame]:
ItemDisplay[NMAG !RW ILVL>59 SOCK=6 ame]:
//
//Necromancer Shrunken Heads
ItemDisplay[NMAG !RW CL4 SOCK=1 ILVL>24]:
ItemDisplay[NMAG !RW CL4 ETH ILVL>24]:
ItemDisplay[NMAG !RW CL4 SOCK=1 ILVL<25]:%NAME% 
ItemDisplay[NMAG !RW CL4 SOCK=2 !ETH ILVL>24]:%NAME%
//
//Sorceress Orbs
ItemDisplay[NMAG !RW CL4 SOCK=1 ILVL>24]:
ItemDisplay[NMAG !RW CL4 SOCK=1 ILVL<25]:%NAME%
ItemDisplay[NMAG !RW CL4 SOCK>1 ILVL>24]:%NAME%
