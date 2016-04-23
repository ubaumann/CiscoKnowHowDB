# Regex Metacharacters

- **Character**
  - Description
  - Notes
- **.**
  - Dot
  - Matches any single character. For example, **d.g** matches **dog**, **dag**, **dtg**, and any word that contains those characters, such as doggonnit.
- **(exp)**
  - Subexpression
  - A subexpression segregates characters from surrounding characters, so that you can use other metacharacters on the subexpression. For example, **d(o|a)g** matches **dog** and **dag**, but **do|ag** matches **do** and **ag**. A subexpression can also be used with repeat quantifiers to differentiate the characters meant for repetition. For example, **ab(xy){3}z** matches **abxyxyxyz**.
- **|**
  - Alternation
  - Matches either expression it separates. For example, **dog|cat** matches **dog** or **cat**.
- **?**
  - Question mark
  - A quantifier that indicates that there are 0 or 1 of the previous expression. For example, **lo?se** matches **lse** or **lose**.
  - Note You must enter **Ctrl+V** and then the question mark or else the help function is invoked.
- __*__
  - Asterisk
  - A quantifier that indicates that there are 0, 1 or any number of the previous expression. For example, **lo*se** matches **lse**, **lose**, **loose**, and so on.
- **+**
  - Plus
  - A quantifier that indicates that there is at least 1 of the previous expression. For example, **lo+se** matches **lose** and **loose**, but not lse.
- **{x} or {x,}**
  - Minimum repeat quantifier
  - Repeat at least x times. For example, **ab(xy){2,}z** matches **abxyxyz**, **abxyxyxyz**, and so on.
- **[abc]**
  - Character class
  - Matches any character in the brackets. For example, **[abc]** matches **a**, **b**, or **c**.
- **[^abc]**
  - Negated character class
  - Matches a single character that is **not** contained within the brackets. For example, **[^abc]** matches any character other than a, b, or c. **[^A-Z]** matches any single character that is not an uppercase letter.
- **[a-c]**
  - Character range class
  - Matches any character in the range. **[a-z]** matches any lowercase letter. You can mix characters and ranges: **[abcq-z]** matches **a, b, c, q, r, s, t, u, v, w, x, y, z,** and so does [a-cq-z].
  - The dash (**-**) character is literal only if it is the last or the first character within the brackets: [abc**-**] or [**-**abc].
- **""**
  - Quotation marks
  - Preserves trailing or leading spaces in the string. For example, **" test"** preserves the leading space when it looks for a match.
- **^**
  - Caret
  - Specifies the beginning of a line.
- **$**
  - end of an input
  - Matches the character or null string at the end of an input string. 
  - **123$** matches **0123**, but not 1234
- **\**
  - Escape character
  - When used with a metacharacter, matches a literal character. For example, **\[** matches the left square bracket.
- *char*
  - Character
  - When character is not a metacharacter, matches the literal character.
- **\r**
  - Carriage return
  - Matches a carriage return 0x0d.
- **\n**
  - Newline
  - Matches a new line 0x0a.
- **\t**
  - Tab
  - Matches a tab 0x09.
- **\f**
  - Formfeed
  - Matches a form feed 0x0c.
- **\xNN**
  - Escaped hexadecimal number
  - Matches an ASCII character using hexadecimal (exactly two digits).
- **\NNN**
  - Escaped octal number
  - Matches an ASCII character as octal (exactly three digits). For example, the character 040 represents a space.
  
## Examples
```
sw8262-c#show version | inc [0-9]?\.[0-9]?\(.*\).?
Cisco IOS Software, C2960C Software (C2960c405ex-UNIVERSALK9-M), Version 15.2(2a)E1, RELEASE SOFTWARE (fc1)
BOOTLDR: C2960C Boot Loader (C2960C-HBOOT-M) Version 12.2(55r)EX11, RELEASE SOFTWARE (fc1)
*    1 10    WS-C2960CG-8TC-L          15.2(2a)E1            C2960c405ex-UNIVERSALK9-M
```

```
sw8262-c#show interfaces status | i ^(Gi|Po)
Port      Name               Status       Vlan       Duplex  Speed Type
Gi0/1     Notebook 01        notconnect   122          auto   auto 10/100/1000BaseTX
Gi0/2     IP-Phone 01        notconnect   127          auto   auto 10/100/1000BaseTX
Gi0/3     Notebook 02        notconnect   122          auto   auto 10/100/1000BaseTX
Gi0/4     IP-Phone 02        connected    127        a-full  a-100 10/100/1000BaseTX
Gi0/5     lab-staging        notconnect   309          auto   auto 10/100/1000BaseTX
Gi0/6                        disabled     1            auto   auto 10/100/1000BaseTX
Gi0/7                        disabled     1            auto   auto 10/100/1000BaseTX
Gi0/8                        disabled     1            auto   auto 10/100/1000BaseTX
Gi0/9     Link to sw8067     connected    trunk      a-full a-1000 10/100/1000BaseTX
Gi0/10    Link to sw8067     connected    trunk      a-full a-1000 10/100/1000BaseTX
Po1       Link to sw8067     connected    trunk      a-full a-1000
```