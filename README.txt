|| this ahk code replaces what you type with whatever you want.
|| for it to work, you Need to have ahk set up, obvi.
||-------------------------------------------------------------
|| this is how it makes you type per deafult:
|| 
|| ᵀʰᵉ ᵠᵘᶦᶜᵏ ᵇʳᵒʷⁿ ᶠᵒˣ ʲᵘᵐᵖˢ ᵒᵛᵉʳ ᵗʰᵉ ˡᵃᶻʸ ᵈᵒᵍ.
|| (It has case sensitivity)
||
|| to Change it, open the ahk in Editor and replace
||
|| :*C:a::
|| Send {Text}ᵃ <------ this
|| return
||
|| :*C:A::
|| Send {Text}ᴬ <------ this
|| return
||
|| Example:
|| 
|| :*C:a::
|| Send {Text}ɐ
|| return
||
|| :*C:A::
|| Send {Text}∀
|| return
||
||-------------------------------------------------------------
||
|| Please take note that this is incredibly prone to Breaking all the fucking time.
||
|| For example, if you type a word with a Character that isnt in the Character database,
|| the font Change doesnt apply to the rest of the word.
||
|| Example:
|| 
|| ᵃᵇᶜᵈöabcd
||     ↑
||     |
||     | The "ö" is not in the database, so it broke the word.
||
|| To fix this, add:
||
||  :*C:ö::
||  Send {Text}ö
||  return
||
|| Result:
||
|| ᵃᵇᶜᵈöᵃᵇᶜᵈ
||
|| Also, ahk it shit at Unicode. If it types the wrong characters, open the ahk in Notepad ++.
|| Then, go on Encoding and make sure UTF-16 LE BOM is selected. It should be selected already, bc i did it 
|| but worth checking/knowing.
||
|| Have fun!


