# -first-name
 Func splitfirstlastname($sFullName)     Local $aWords = StringSplit(StringStripWS($sFullName, 7), " ");Clean out leading/trailing/double+ spaces, and Split into words     Local $sFirstnames, $sLastname     $sLastname = $aWords[$aWords[0]];Assume the last (or only) word is the last name     Select         Case $aWords[0] = 1;Assume no first name if only one word
