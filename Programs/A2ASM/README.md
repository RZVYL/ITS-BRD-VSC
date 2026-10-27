Anw01 Loads a word from a PC-relative adress.  R0 kriegt die Speicheradresse von VariableA zugewisen Pseudocode.

Anw02 Loads a byte from memory () ldrb das b = byte lädt nur einen Byte aus [R0] (Speicheradresse) nach R2 (0xef).

Anw03 Lädt den byte mit der Speicheradresse von [R0] versetzt (sogesagt 1 step) nach R3 (0xbe).

Anw04 versetzt den im Register den Inhalt um 8 bits nach links (logical shift left) z.B.: 1110 1111 0000 0000

Anw05 Bitweise orr (oder) wird dann bennutzt damit der Byte aus R3 mit R2 zusammengefügt wird auf die 0000 0000 die wir im vorherigen Schritt erstellt haben.

Anw06 Hier wird mit nutzung des strh befehls ein halfword von R2 nach [R0] (Speicheradresse) gespeichert.

Anw07 Zieht sich 0xAffe aus #ConstbyteA raus um damit zu arbeiten auf dem Register R5. No Idea was EQU ist

Anw08 Speichert R5 als halfword in der Speicheradresse [R0]

Anw09 Speichert sich die Speicheradresse aus VariableB nach R1.Pseudocode