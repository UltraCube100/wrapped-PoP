Wrapped PoP is a spin-off of the Palace of Points that is similar to cryptocurrency but is allowable by the Scratch Team as a "mall simulator". Wrapped PoP has NFTs, and the exchange rate is 1 PoP = 1 wPoP. Precision of wPoP is 10^-2 (0.01)

# Exchange
Exchange of PoP for wPoP is done by purchasing a NFT from a shop for PoP. In return, you get 1 wPoP for each PoP you spend, and you also get ownership of the NFT you bought on the wPoP chain. You can also exchange your wPoP back to PoP. 

Unlike other mall simulators on Scratch, when you sign up for wPoP in the studio, you do not start off with any "points". You must exchange PoP for wPoP and send it to your account.

# NFTs
An NFT (non fungible token) is a link on the blockchain to a file that can be a text file, an image, a video, etc. In the context of Wrapped PoP, a NFT is a costume of a sprite, or simply a image.

# Transcations and Staking
An wPoP address is similar to PoP's. It is a number followed by a randomly generated string of 5 hex numbers (0-f) seperated by "-0x". Example: 1-0x6ce52, 1572-0xb59bc.
Unlike the Palace of Points, a user may have multiple addresses/accounts (up to 4).

Sending a transcation is simple, as you can only send to other users. You can also put a short PUBLIC transcation message. No proof required.

All Transcations are stored on the ledger.

# Guide to reading the ledger
Each transcation uses this format (without the curly brackets):

 #{transcation number} {sender's address} == {recipent's address} 
 +{amount being sent} 
 SENDER_BAL BF {sender's balance before transcation}
 SENDER_BAL AFT {sender's balance after transcation}
 RECIPENT_BAL BF {recipent's address before transcation}
 RECIPENT_BAL AFT {recipent's address before transcation}
 MSG = {transcation message} 

 Note that after the "+", "wPoP" is NOT placed, and that the transcation amount is to the precision of 0.01, even if the transcation amount is a whole number or it is only to the precision of 0.1. If there is no transcation message, the message is left as "NA"
 Example:

 #1 1-0x6ce52 == 1572-0xb59bc
 +25.00
 SENDER_BAL BF 150.00
 SENDER_BAL AFT 125.00
 RECIPENT_BAL BF 0.00
 RECIPENT_BAL AFT 25.00
 MSG = NA
 
