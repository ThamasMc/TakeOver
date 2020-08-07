# Tech Corp - Danidae Defenses and Operating Systems

## Design and Development
When it came to creating the first Corporation, I wanted to focus on creating an inviting entrypoint for players - here's the driving thoughts behind what that would mean:
  1. The Corporation doesn't _feel_ hostile to the player.
    - People lock down when they feel attacked by something, even gameplay mechanics, and it can make intial processing of the games mechanics more difficult to accomplish.
  2. The Players have a _single, clear, and direct_ path towards victory.
    - With future Corporations, players will have to actively maintain performance in multiple mechanical fields in order to achieve victory. For instance, with a more hostile Corporation the decision between maintaining a player's health and rate of uncovering data will be a much more tactical choice.
    - Since `digging` on a Server is how a player uncovers data, I decided that the antagonistic actions of this Corporation should essentially encourage _more_ digging.
  3. The Corporation should have a linear and definitive path towards victory
    - Sort of the inverse of #2, if it should be clear and defined how the players win, it should also be clear how they would lose.
    - I wanted to focus on the pacing of a game against this Corporation to be a steady and ominous clock. Sudden losses are rare, but I wanted to emphasize on the tension building as the Innovation counter neared completion.

With these goals in mind came prototyping and `playtesting` and `playtesting` and `playtesting` and more `playtesting`. Ultimately here we are after a dozen or so minor iterations in, and a major version update/overhaul: The Tech Corp - DDOS

## Themes and Special Mechanics
DDOS is a Corporation widely prevalant within modern society, their technology present in devices ranging from unmanned drones to toasters. DDOS isn't concerned with the growing hacktivist threat, confident that its Total Global Corporate TakeOver is only a matter of time.

A Corp like DDOS doesn't need to worry about putting an end to the hacktivists once and for all, but rather focuses on using underhanded tactics and delays to strengthen the security of the servers and protect the obscurity of their ultimate motives.

DDOS fills their server with special **Static** traps to slow down the players from uncovering the data required to expose their schemes.

Static on its own does little but take up space. In fact, when a player uncovers normal Static from the server, it immediately trashes itself, removing itself from the game.

Some Static can be a bit... _Stickier_, and will be placed into a player's discard to be shuffled back into their deck. These **Sticky Statics** act as blanks, and will immediately trash themselves upon being drawn from a player's deck.

Even the Data itself can cost additional player actions, **Tax** Data requires players to discard cards from their hand in order to successfully wrench it from the server, and if they're unable to, they'll have to watch as it disappears to the depths of the Server.

Don't get too comfortable though, a Corp is still a Corp, and even a lazy one can get nasty if player isn't careful. Few and far between, dangerous viruses and traps do still lurk within DDOS's servers, waiting for any players growing a little too complacent.

------

## Extra Notes
Something I like talking about is some of the **major** problems previous iterations of the game had, and the thought processes around identifying and overcoming them.

This Corporation has seen a lot of iteration from its initial form, and it was a lot of fun and more importantly, educational, playtesting it.

Playtesting - I can't stress enough how important it is to reduce the time between ideation and confirmation. It might be my Agile showing, but nothing shows better what's wrong (or right) about your products/ideas than the people who would use it.

Once I got a playtest together for it I'd take it to my local game shop and ask around to see if anyone wanted to try it out. Turns out, gamers are generally down to try new things, and also generally down to tell you what's wrong with it. Magic players even more willing than most!

The very first time the prototype was played I could see the first major glaring issue. It was just _too long_. I think the intial playtime of the game averaged between 3-4 hours and that was faaar longer than what I intended for this Corporation, which I have since gotten down more towards the target value of 1h 30m.

As playtesting continued, I identified that aesthetics of the Corporation where hitting about where I had wanted it, and the emergent dynamics were spot on as well. People were engaged in exploring the mechanics of the system, and felt the heat as the timer went reached `TakeOver`, but there were certain mechanical aspects that could still be improved.

For instance, initally, there was _way_ too much shuffling involved. Basically anything that altered the order of the deck was a shuffle, and for a 100 card double-sleeved thickness deck, if you weren't an experienced Commander player, you weren't having a good time shuffling.

On this point, I tried out a few different things, and ended up in the spot we're at now, where most re-ordering actions will move the card specifically to the bottom of the deck. A short, sweet style of 'getting rid' of a card, and something that opens up design space in interacting with the bottom of the server deck!

The other major offender of a mechanic exacerbating the length of the game would be a general over _stickiness_ of cards. Static used to act similarly to Sticky Static, and Sticky Static was a permanent negative within a player's Deck. Data was sent to your discard to eventually get shuffled into a players Deck to play, and Capsule data required being played twice. Due to the delayed 'cause and effect' loop that a lot of these cards had, players were having difficulty deciding what was _worth_ doing.

The biggest rework I made to TakeOver was focused on addressing this problem. I took another look at each card, and thought "When I take action X to get this card Y, I get outcome Z". From a player's perspective, the risk of action X is essentially promised a payoff of Z, and there should be a direct relationship between the two.

This way, I could really easily trace the fundamental problems of how "I take action `dig` to get `Data` and put it into my discard" did **not** match my intention of "I take action `dig` and get a payoff of `Expose 1` on the active scheme."

Using this refocused evaluation, I worked towards a huge overhaul that resulted in the present implementation of the Expose Mechanic, Data, Static, Schemes, along with newly added bonus of Schemes granting a boon upon completion.

Well, that's basically it! Those are my musings on the design challenges I've encountered with the Tech Corporation. Feedback is the best tool a designer can utilize to improve what they have, and I had some fantastic playtesters that provided even `fantasticer` feedback. I had fellow designers give their thoughts on the systems and cards as they stood, as well as some feedback on potential cards and mechanics to include! There's always a desire to keep a project entirely 'your own', but the irony is once a game, or any product/idea/artform really, is out there it's not really just for _you_ anymore. Everyone sees it differently, enjoys different things about it, and will have completely different experiences with it.

All in all, I think that's pretty cool.
