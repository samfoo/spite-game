# Spite

Spite is a trick-taking card game for 3 to 9(ish) players based loosely on Big
two, but which also takes various rules and design ideas from 500, Poker, and
the Game of Mao.

The ruleset of Spite is complicated by design, and players receive penalties
and rewards for misplaying or identifying others who misplay respectively.

# The Rules

## The Deck

The Spite deck is three "six-handed 500" decks combined (63 cards each, a total
of 189 cards). Each 63 card deck includes:

* A regular 52 card deck
* A joker
* One of each suit 11s
* One of each suit 12s
* Two 13s, 13♥ and 13♦ (todo: add red formatting)

Addtionally, several cards - of any suit and face value - which come from a
deck with a different card-back design should be set aside from the main deck
for use as "fake jokers".


## Playing

The object of Spite is to get rid of all the cards in your hand as soon as
possible. This is done by playing a series of tricks in which cards may be
played. Once there is only one player with cards remaining, the round is over.

The winners and losers from each round receive rewards and penalties for the
next round.


### Starting Play

At the start of a round, each player is dealt 11 cards and play proceeds
clockwise from the first player.

Control of the first trick is determined by:

- If it is the first round being played, any player who was dealt any 3s must
  play one of more of them. The first player who plays a 3 receives control. If
  a player is dealt any 3s at least one of them must be played (unless someone
  else has played theirs first). If no one has any 3s then move on to 4s, and
  subsequently 5s and so forth.
- The player who has the most penalties applied to them (todo: link to
  explaining penalties). If multiple players have the same penalty value, then
  the player who lost the round most recently starts.

### Playing Tricks

On their turn each player must decide to play a card or cards, or pass. Once a
player passes they may no longer participate in the trick until they "buy back"
or "BB" (todo: anchor link to rules on BB'ing).

The laster player to have played before everyone else has passed in that trick
is the winner of the trick and receives conntrol of the game, allowing them to
start the next trick. If the player went out by playing the final card in their
hand while winning the trick, control is giving to the player sitting to the
winners left (clockwise).

Play starts off where any card (or cards) which is high than the current card
may be played, where 3s are the lowest possible card and 2s are the highest.


#### Valid Starting Plays

- A single card.
- Two, three, and four of a kind.
- Poker hands (i.e. exactly five cards) of a straight, full house, flushe and
  four-of-a-kind.
- A joker or joker equivalent (five or six of a kind).


#### Continuing the Trick

After a valid starting play has been placed, all plays in the trick must now
match the arity, and must be strictly better than the previous play.

For instance, if the starting play was a pair of 5s (5♠, 5♦), subsequent plays
must match the arity (i.e. pairs) and must be better than the previous play.


#### Misplays

A key feature of Spite is that all plays **must** be valid, and any action
which is not within the rules can be called out as a "misplay" by any other
player.

A player who has misplayed is penalised by

1. No longer being allowed to play in the current trick.
2. After the current trick is completed that player must pass their next turn.
   They may still buy back after that pass if play allows.
3. Any "fake jokers" that the player has are forfeited.

Misplays are called out by any player who notices them by saying "Misplay!". If
the table agrees the call was valid, the misplayer is penalised as described
above and the player who called the misplay is awarded a "fake joker".


#### Dynamic Restrictions

Throughout the trick some dynamic restrictions can come into force due to the
actions of the players. There are two types of dynamic restrictions:

1. Suited-ness (aka. suited)
2. Consecutive-ness (aka. consec)

Suited-ness occurs when three cards of the same suit have been played. After
this only cards of that suit may be played (Jokers and 13s may no longer be
played).

Consecutive-ness occurs when three cards which have an equal gap between them
have been played. The most basic case is when the cards played are of
consecutive value, e.g. the current trick has played - 3♦, 4♣, 5♣ - the next
card to be played **must** be a 6 (of any suit).

Both suited-ness and consecutive-ness can be in play *at the same time*. So if
the play has been 8♣, 9♣, 10♣, then the next valid play **must** be an 11♣.

There is one exception: 13s may not participate in or start the restrictions.
Because there are only red (♦, ♥) 13s in the deck and because they are
pseudo-wild, they are not allowed to start or participate in the dynamic
restrictions. Since they are not playable in consec or suited contexts,
consecutive card values are 11 -> 12 -> J, not 11 -> 12 -> 13

Dynamic restrictions apply to any number-of-a-kind tricks. For example,
if the play has been pair-9s -> pair-11s -> pair-Js then the next play must be
pair-Ks.

##### Special Cases

There are two special cases once dynamic rules are in play:

1. For suited-but-not-consecutive tricks, a 2 of the correct suit is unbeatable
   by any card and must be declared so by saying "Unbeatable" when played. Not
   saying "unbeatable" is a misplay.
2. For consecutive tricks, consecutive runs wrap around the highest to the
   lowest card. So if this play is K -> A -> 2, then the next valid play is a 3.


#### Card Rules Appendix

- 3 - If the previous play state was "lower", then upon playing a 3 (or any
  number of threes outside of a poker hand) the direction is reset to "higher".
- 7 - Upon playing a 7 (or any number of sevens outside of a poker hand, and
  not in combination with any 13s) a player may choose to say "lower" which
  inverts card values so that every card played must be **lower** than the
  previous card rather than higher. This change persists across tricks, but not
  across rounds.

  If the play direction is already lower, a player may choose instead to say
  "higher" and reverse in the opposite direction.

  If the previous player has played 7s (and conseq/suited are not in force)
  then next player is allowed to play a 7 also but doing so automatically
  reverses the current direction. When doing so a player **must not** declare a
  direction because it has automatically been reversed. Declaring the direction
  is a misplay.
- 13 - All 13s are "pseudo-wild" and must never be played in any consec or
  suited tricks. They can be played in combination with another card to form an
  arity or poker hand.

  Consider the following examples:

  - (13♥, 2♠) is a pair of 2s.
  - (13♠, 3♦, 4♣, 5♣, 6♠) is a poker straight of (3, 4, 5, 6, 7).

  n.b. A 13 in a poker hand **always** forms the lowest possible valid poker
  hand.
- Fake jokers - todo: explain them
- Pure jokers - todo: explain them
