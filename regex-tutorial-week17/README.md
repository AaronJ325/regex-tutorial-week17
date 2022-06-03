Regex Tutorial
Regular expressions can be used to find certain patterns of characters within a string. You can also find and replace a character or sequence of characters within a string. They are also frequently used to validate input. This regex matches character information for valid e-mail addresses.

Regex code: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Topics:
Anchors
Quantifiers
Character Classes
Grouping and Capturing

Anchors:
Used to contain this regular expression are: ^ to start, and $ to finish.

Quantifiers:
In this example, we used + to communicate there is another sequence to be matched as a greedy quantifier. We also used {2,6} as another greedy quantifer to specify the input should be a minimum of 2 characrtors to a maximum of 6 characters.

Character Classes:
In this regular expression, the charactor class /d is used which in Javasctipt classifies the use of any digit from 0 to 9.

Grouping and Capturing:
There are three groups being captured in this example. Group #1 is the username of the e-mail account [a-z0-9_\.-]. The second group captures the domain name or e-mail service being used [\da-z\.-]. Lastly, the third group captures the domain extention (i.e .com or .net) [a-z\.]{2,6}