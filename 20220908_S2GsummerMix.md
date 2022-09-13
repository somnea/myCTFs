# S2G summer mix

## Web: (3/6 solved)
### Challenge Title: I wanted an iPad, but I instead got an iDor :(
  http://10.212.138.23:26296
  	IDOR = Insecure Direct Object Reference
  	click on anything until url changes from "http://10.212.138.23:26296/index.html" to "http://10.212.138.23:26296/index.html?id=1"
  	change the end to "id=0"
	= S2G{ID0r_vu1nerAbilities_<<<333}

### Challenge Title: Find the flag, need I say more?
  http://10.212.138.23:32023
  	view page source
  	= S2G{C0ngr4tul4t10n5_4nd_c3l3br4t10n5}

### Challenge Title: Second time is the charm
  http://10.212.138.23:10721
  	inspect site
  	find script (javascript)
  	before running it in browser console add return in function
  	returns a base64 encrypted flag
  	= S2G{b15c0771_50n0_bu0n1}


Miscellaneous: (1/5 solved)
- H4sIAGGiGGMA/xXFsQlAIQwE0JVOzQ4O4ADXiSCkCPeLj7h7sHqj9qNlvvnj40Q8gyY1V4HfBA0IQK8hAAAA==
	CyberChef
	From Base64
	press magic wand
	= S2G{th4nk_y0u_f0r_y0ur_4tt3nt10n}

Steganography (1/2 solved)
- I was out hiking yesterday and I found this beautiful plant in among the heather. I_wond3r_wh4t might be contained inside?
  + microScopic.jpg image was given
	https://futureboy.us/stegano/decinput.html
	put password "I_wond3r_wh4t"
	search for flag-format "s2g"
	= S2G{d0n't_m1s5_y0ur_gr4duat1on,_b4rry}

Reverse Engineering (1/1 solved)
### Challenge Title: I was tangled in.. in.. strings
  Tony Stark's suit has crashed, and needs to be rebooted so he can deal with Ultron.
  However, time is running out, and he can't remember his password. Can you help him?
  given file: legionnaire
  	run command "file legionnaire" to find filetype -> ELF file
  	run command "strings legionnaire" to read file in strings
  	run command "chmod +x legionnaire" to run ELF-file
  	paste found password in string
  	= CTF{1_h4d_str1ngz_but_n0w_1m_fre3ee3e}
