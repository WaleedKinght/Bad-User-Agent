##############################################################################
#                                )___(
#                               (o o)
#    /---------------------oOO---(_)---OOo---------------------\
#                                                              
# ██     ██  █████  ██      ███████ ███████ ██████  
# ██     ██ ██   ██ ██      ██      ██      ██   ██ 
# ██  █  ██ ███████ ██      █████   █████   ██████  
# ██ ███ ██ ██   ██ ██      ██      ██      ██   ██ 
#  ███ ███  ██   ██ ███████ ███████ ███████ ██   ██ 
#                                                                
#                       BAD USER-AGENT CUSTOM LIST             
#                                                              
#  This file is a custom blacklist & whitelist for User-Agents. 
#  It gives you full control over blocking or whitelisting      
#  specific bots and crawlers that are not covered by the main  
#  bad bot blocker.                                             
#                                                              
#  • Loads first to override the default bad bot blocker rules. 
#  • Supports BLACKLIST (3;) and WHITELIST (0;) modes.          
#  • Supports RATE LIMIT (2;) and SUPER RATE LIMIT (4;) modes.  
#  • Prevents partial matching by using Regex word boundaries.  
#                                                              
#  Enjoy ultimate control over which bots are allowed or denied!
#                                                              
#    oOO-------------------------------------------------OOo    
#   (   )                                               (   )   
#    \ (                                                 ) /    
#     \_)                                               (_/     
##############################################################################

# ---------------------	
# WHITELISTING EXAMPLES
# ---------------------
#	"~*(?:\b)someverygooduseragentname1(?:\b)"			0;
#	"~*(?:\b)someverygooduseragentname2(?:\b)"			0;
#	"~*(?:\b)some\-very\-good\-useragentname2(?:\b)"	0;

# ----------------------
# RATE LIMITING EXAMPLES
# ----------------------
#	"~*(?:\b)someverybaduseragentname1(?:\b)"			2;
#	"~*(?:\b)someverybaduseragentname2(?:\b)"			2;
#	"~*(?:\b)some\-very\-bad\-useragentname3(?:\b)"	2;

# ---------------------
# BLACKLISTING EXAMPLES
# ---------------------
#	"~*(?:\b)someverybaduseragentname4(?:\b)"			3;
#	"~*(?:\b)someverybaduseragentname5(?:\b)"			3;
#	"~*(?:\b)some\-very\-bad\-useragentname6(?:\b)"	3;

# ----------------------------
# SUPER RATE LIMITING EXAMPLES
# ----------------------------
#	"~*(?:\b)someverybaduseragentname7(?:\b)"			4;
#	"~*(?:\b)someverybaduseragentname8(?:\b)"			4;
#	"~*(?:\b)some\-very\-bad\-useragentname9(?:\b)"	4;


# ----------------------------
# MY CUSTOM BLACKLIST ENTRIES
# ----------------------------
"~*(?:\b)x22(?:\b)"					3;
"~*(?:\b){|}|{(?:\b)"				3;
"~*(?:\b)mb_ereg_replace(?:\b)"		3;
"~*(?:\b)file_put_contents(?:\b)"	3;
