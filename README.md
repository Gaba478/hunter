function onGiveLootHunter(thePlayer)
	account = getPlayerAccount(source)
	if getElementData(player,"VIP") then --ACL group
		if type(getAccountData(account,"usevipHUNTER")) ~= "number" then setAccountData(account,"usevipHUNTER",0) end
		if not getAccountData(account,"usevipHUNTER") or getAccountData(account,"usevipHUNTER") <= 0 then
			setAccountData(account,"usevipHUNTER",12) --kd
				setElementData(thePlayer,"winchester_1866",1) 
				setElementData(thePlayer,"winchester_1866_mag", 200) 
				setElementData(thePlayer,"m4a1_rco", 1) 
				setElementData(thePlayer,"m4a1_rco_mag", 200) 
				setElementData(thePlayer,"mp5a5",1) 
				setElementData(thePlayer,"mp5a5_mag",500) 
				setElementData(thePlayer,"m67", 15) 
				setElementData(thePlayer, "mokorons_p", 5) 
				setElementData(thePlayer, "flask", 5) 
				setElementData(thePlayer,"helmet_adh5",2) 
				setElementData(thePlayer,"armortors_adbv4",2) 
				setElementData(thePlayer, "helmetOn", 5) 
				setElementData(thePlayer, "armorOn", 4) 
				setElementData(thePlayer,"armlet_l",1) 
				setElementData(thePlayer,"armlet_r",1) 
				setElementData(thePlayer,"armleg_l",1) 
				setElementData(thePlayer,"armleg_r",1) 
				setElementData(thePlayer,"armass",1) 
				setElementData(thePlayer, "armorTazOn", 1) 
				setElementData(thePlayer, "armorLNarOn", 1) 
				setElementData(thePlayer, "armorRNarOn", 1) 
				setElementData(thePlayer, "armorLNogOn", 1) 
				setElementData(thePlayer, "armorRNogOn", 1) 
				setElementData(thePlayer, "pole_bag", 1) 
				setElementData(thePlayer, "MAX_Slots", 150) 
				setElementData(thePlayer, "medkit", 7) 
				setElementData(thePlayer, "bint", 5) 
				setElementData(thePlayer, "painkiller", 10) 
				setElementData(thePlayer, "morphine", 10) 
				setElementData(thePlayer, "woman_skin", 1) 
				setElementData(thePlayer,"map",1) 
				setElementData(thePlayer,"gps",1) 
				setElementData(thePlayer,"inf_glass",1) 
				setElementData(thePlayer,"tools",1) 
				setElementData(thePlayer,"pnv",1) 
				setElementData(thePlayer,"radio",1) 
				setElementData(thePlayer,"bankmoney",getElementData(thePlayer,"bankmoney")+10000) 
				end
		else
			outputChatBox("Вы уже получили набор охотника. Попробуйте ещё раз через "..getAccountData(account,"usevipHUNTER").." мин.",source,255,255,255)
		end
	-- end
end
addCommandHandler ( "hunter", onGiveLootTitan)
