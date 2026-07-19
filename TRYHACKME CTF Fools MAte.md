TRYHACKME CTF Fools Mate

First what i did was the obvious just tried to move the piece to the mate position but as usual the dev had displayed this msg

"I will shutdown your computer"

Then i even tried input validation to see if i can inject some other value for the webpage to process but then i figured out that the webpage keeps on expiring after one cause of chessboard 
(figured that out late) so then i switched i tried to change webpage read the java script to see how i can manipulate(just beginner level coding knowledge btw) so then i thought what if the machine thought that the value was right the first time then i could send my malicious value so that's what i did

In the burp repeater where i captured the request /api/move
As i knew that the request expired after one i intercepted the request then added 2 from and to 

like this 
{
	"from":"a1"
	"to":"a7"
	"from":"a7"
	"to":"a8"
}

I have been doing labs now for over a week hope i keep the streak up


