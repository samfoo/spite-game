---
layout: page
title:  "Spite"
date:   2023-03-11 16:42:11 +1100
---

# Spite

Spite is a trick-taking/shedding card game for 3 to 9(ish) players based loosely
on [Big Two][big2], but which also takes various rules and design ideas from
[500][500], [Poker][poker], and [Mao][mao].

[big2]: https://en.wikipedia.org/wiki/Big_two
[500]: https://en.wikipedia.org/wiki/500_(card_game)
[poker]: https://en.wikipedia.org/wiki/Poker
[mao]: https://en.wikipedia.org/wiki/Mao_(card_game)

The ruleset of Spite is complicated by design, and players receive penalties
and rewards for misplaying or identifying others who misplay respectively.

# Objective

In a round of Spite, the winners and losers are determined by the ordering in
which players got rid of all the cards in their hands, through playing valid
combinations of cards in a series of tricks. The round is played until there
is only one player with cards remaining.

The winners and losers from each round receive rewards and penalties for the
next round. Therefore, the typical objective is to finish each round amongst
the winners, although sometimes players may choose to lose for strategic or
spiteful reasons.

In keeping with the name and spirit of the game, players should endeavour to
make spiteful plays whenever possible for maximum comedic effect.

# The Deck

The Spite deck is approximately 3 "six-handed 500" decks combined (63 cards
each, a total of 189 cards). Each 63-card deck includes:

- A regular 52-card deck
- 11s and 12s of each suit
- 13♥ and 13♦
- A joker

Addtionally, approximately 5 cards (of arbitrary suits and face values) from a
deck with a different card-back design should be set aside from the main deck
for use as [fake jokers](#fake-jokers).

# Game Play

## The Initial Deal

At the start of a round, each player is dealt 11 cards face down. The top card
of the deck is revealed as the [bounty card](#the-bounty-card), then game play
proceeds clockwise from the first player.

## The First Player

The first player is determined by:

- If it is the first round being played: any player who was dealt any 3s may
  play a hand that includes one of more of them. The first player who plays
  such a hand becomes the lead of the first trick. If no player has any 3s (or
  those with 3s do not wish to play them) then the round may begin by applying
  the same rule to 4s, then 5s, and so forth, until someone is willing to lead.
- Otherwise: the player with the most negative [score](#scoring) shall lead the
  first trick by playing any valid hand. If there are multiple players with the
  same negative score, the player who most recently lost a round shall lead.

## Playing Tricks

On their turn, each player must decide to play or pass. Once a player passes,
they may no longer participate in the trick unless they [buy back](#buy-back).

A player has 5 seconds to make a decision when it is their turn. If the player
has just picked up extra cards, they get one extra second for each card they
picked up. Any player at the table may start a countdown, and if the player
fails to play a valid hand before the countdown finishes then they shall be
deemed to have passed.

The last player to have played before everyone else has passed in that trick
is the winner of that trick and shall lead the next trick. If that player has
gone out by playing their final card(s) while winning the trick, then the next
player in clockwise sequence shall lead the next trick.

### Valid Leading Hands

- A single card.
- Two, three, or four cards of the same value (pairs, trips, or quads).
- Poker hands (i.e. exactly five cards) of a straight, full house, flush, or
  four-of-a-kind (i.e. four cards of the same value, plus another card of a
  different value).
- A [joker hand](#joker-hands).

### Valid Following Hands

After a valid leading hand has been played, all plays in the trick must follow
the arity, and must be strictly better than the previous hand, unless permitted
elsewhere within these rules.

For example, if the leading play was a pair of 5s (5♠, 5♦), subsequent plays
must be a better pair.

## Buy Back

If a player who has passed during a trick wishes to re-enter into play of that
trick, they must "buy back" by picking up additional cards. They must first
announce "buy back X" or "BB X" where X is the number of cards they intend to
pick up, play the hand they wish to play, then pick up the additional cards
from the deck. In other words, the buy-back cards shall not be used to allow
them to re-enter into play.

The number of additional cards they must pick up is a global counter shared by
all players on the table and follows the [Fibonacci sequence][fib] (1, 1, 2, 3,
5, 8, ..., and so on). The count resets at the beginning of each round. It is
a [misplay](#misplays) to buy back for an incorrect number of cards.

Once a player has bought back into a trick, they may continue to play on their
subsequent turns within this trick without buying back until they pass again.

If the number of cards in a player's hand reaches or exceeds 20, they instantly
lose the round.

[fib]: https://en.wikipedia.org/wiki/Fibonacci_number

## Hand Rankings

Individual cards are ranked by their face value, with 3 being the lowest and 2
being the highest (i.e. 3 to 13, J, Q, K, A, 2), with all suits being equal.

A hand consisting of multiple cards of the same value (pairs, trips, quads) are
ranked by the value as above. Two hands with the same face value are ranked by
the "similarity" of cards within the hand, from low to high:

- Mixed (a hand consisting of both black and red cards)
- Coloured (a hand consisting of cards of the same colour, but different suits)
- Suited (a hand consisting of cards of the same suit)

Poker hands shall follow the usual poker ranking rules, except:

- Flushes are ranked higher than full houses.
- Poker hand values are modified to the extent that allows 2 to be the highest
  card. For example, J-Q-K-A-2 is a valid (and the highest) straight.

### Wildcards

Whilst 13 is ranked between 12 and J when played in a hand that consists solely
of 13s, they can also be used as wildcards when played in combination with other
cards. For example, any card X plus a 13 is considered a pair of Xs.

When 13s are used in a poker hand, it shall always form the lowest valid hand.
For example, a full house with 4-4-J-J-13 is always considered to be 4s full of
jacks; a straight with 8-9-10-11-13 is always considered to be 7-8-9-10-11.

A hand that includes one or more 13s is ranked lower than the "natural" version
of that hand (i.e. without 13s), and a hand with more 13s is ranked lower than
the same hand with fewer 13s.

## Game Direction

In addition to the ranking of hands, the game may be played either in the higher
or lower direction, which dictates whether each subsequent hand in a trick must
be higher or lower in ranking than the previous hand.

Each round starts in the higher direction. When a player plays a hand of natural
7s (e.g. a single 7, a pair of 7s, etc., without any 13s), the player may choose
to change the direction by verbally announcing "higher" or "lower". However:

- If a player does not announce a direction, the direction remains unchanged.
- If a player chooses to announce a direction, it _must_ be the opposite of the
  current direction. It is a [misplay](#misplays) to announce the same direction
  as what is currently in play.
- A player may play a 7 (or a hand of natural 7s with the same arity) on top of
  a 7 (or a hand of natural 7s), which will immediately reverse the direction,
  regardless of whether a direction change was made by the previous hand of 7s.
  It is a [misplay](#misplay) to make any announcement regarding direction in
  this case.

If a hand consisting solely of natural 3s is played while the game is going lower,
the direction "bounces" back to higher.

## Joker Hands

Joker hands can be played without following the arity of the trick when there
are no [consecutives](#consecutives) in force.

A natural joker is the lowest ranked joker hand. It can beat any non-joker hand
and other natural jokers.

Five or more natural cards of the same value are also joker hands, and are
ranked higher than natural jokers. These joker hands are ranked by hand size,
and then by numeric value within the same hand size.

If a joker hand is played during a trick (except when leading):

- When the [game direction](#game-direction) is higher, joker hands can beat any
  non-joker hands, and can only be beaten by higher joker hands.
- When the direction is lower, joker hands reset the ranking in play such that
  any valid hand that follows the trick's arity may be played on top of it.

If a joker hand is lead:

- When the direction is higher, joker hands are the highest ranked hands and
  can only be beaten by higher jokers.
- When the direction is lower, the arity of the trick is indeterminate. The
  next player may play any valid hand, and that hand shall determine the arity
  of the trick.

Joker hands are not allowed to be played as the last or second last play of a
player, to encourage their usage earlier in the round. If a player plays a joker
hand as their last or second last play, the play stands but they immediately
become the loser of the round.

### Fake Jokers

The extra cards with a different card-back design are "fake jokers". Players can
earn fake jokers by:

- Being the quickest to call another player's [misplay](#misplays) correctly.
  - If the player who misplayed had any fake joker(s) in their possession at
    the time of misplay, these fake joker(s) shall be transferred to the player
    who correctly called the misplay as a reward. If they did not possess any
    fake jokers, the caller shall receive 1 fake joker from the common pile as
    a reward.
  - If two or more players correctly call a misplay at the same time, a coin
    flip or other randomisation mechanism shall be used to determine who shall
    receive the reward.
  - However, fake jokers are not awarded if a misplay was only called _after_
    the table has reached a consensus about the validity of the play in question
    through discussion. In this case, any fake joker(s) possessed by the player
    who misplayed shall be returned to the common pile.
- Going out of a round by playing a hand consisting solely of natural cards with
  the same value as the [bounty card](#the-bounty-card).
  - It is a misplay to claim an incorrect number of fake joker(s) from the common
    pile. If this happens and is called out by another player, the mis-claimed
    fake joker(s) shall remain in (or be returned to) the common pile and do not
    form part of the reward that is transferred to the caller.

Fake jokers are not part of a player's regular hand. A player is considered to
have gone out of a round when their regular hand is exhausted, regardless of
whether they still hold any fake jokers. Fake jokers persist across rounds until
they are played or lost. Once a fake joker has been played, it shall be returned
to the fake joker pile and may be earned by other players.

Fake jokers can be played either face-up or face-down.

- When played face-up, they will take on their natural face value and can be
  used whenever that face value is valid.
- When played face-down during a trick, they reset the ranking in play such that
  any valid hand that follows the trick's arity may be played on top of it.
- When played face-up to lead a trick, the arity of the trick is indeterminate,
  regardless of current [game direction](#game-direction). The next player may
  play any valid hand, and that hand determines the arity of the trick.

Fake jokers are not allowed to be played face-down as the last or second last
play of a player. The same penalty as playing joker hands as the last or second
last play shall apply. However, fake jokers may be played face-up as the second
last play.

If the fake joker pile is exhausted, further actions that would have caused a
player to earn fake joker(s), including any deficit in the current claim, shall
cause that player to earn the next card(s) from the deck. Such cards are also
not part of the player's regular hand, but can only be played face-up, and are
not considered fake jokers for the purpose of card ranking.

### The Bounty Card

If a player finishes by playing a hand that consists solely of natural cards
with the same face value as the bounty card, that player "claims the bounty" and
gains a number of fake jokers equal to the number of bounty cards in their final
hand. The bounty card is immediately discarded and a new bounty card revealed,
so that other players may continue to claim the bounty within the same trick.

If a joker is revealed as the bounty card, it shall be shuffled back into the
deck and a new bounty card is revealed.

## Consecutives

During a trick, when the last 3 hands that were played form certain patterns,
a consecutive restriction (a.k.a. "consec") shall come into force. Consecs
only apply to hands that consist of cards of the same value (i.e. single cards,
pairs, trips, quads, etc., without any 13s) and not to poker hands.

13s and joker hands may not be played when any consec restriction is in force.

There are two orthogonal consec restrictions that may be applied. If, while one
consec restriction is in force, the pattern for the other consec restriction
emerges, then both restrictions shall be applied simultaneously from that point.

### Numerical Consec

Numerical consec occurs when three hands with an equal gap between their ranks
have been played, regardless of suit(s). The most basic case is three hands of
consecutive numeric value, e.g. if the last 3 hands played were 3♦, 4♣, 5♣ ,
the next valid hand is a 6 (of any suit).

13s are not part of the ranking when determining numerical consecutiveness, i.e.
the card ranked immediately after 12 is J.

When numerical consec is in force, the trick may "wrap around" to continue the
sequence. For example, if the last three hands played were 11, Q, 2, the next
valid hand is a 5, because the difference between each hand is 3 ranks.

If the [game direction](#game-direction) is lower:

- Numerical consecs may be formed via bouncing on 3. For example, if the last
  three hands played were 4, 3, 4, the next valid hand is a 5.
- If numerical consec is in force when the direction is lower, the direction
  shall only bounce if a 3 is played. Otherwise, the trick shall wrap around
  and continue from the top end. For example, if the last three hands played
  were 8, 6, 4, the next valid hand is a 2.

### Suited Consec

Suited consec occurs when three hands of the same suit(s) have been played.
From this point, only hands of the same suit(s) can be played.

If the trick's arity is greater than 1, then suited consec refers to hands with
the same combinations of suits. For example, if three pairs of X♦ X♣ have been
played, then all subsequent pairs must also consist of ♦ and ♣.

Because joker hands are not allowed during any consec, a 2 is the highest card
during a suited-but-not-numerical consec when the [direction](#game-direction)
is higher. When a player plays the 2 (or 2s), they must announce "unbeatable",
otherwise it is a [misplay](#misplays).

# Come At Me

During a trick, a player may announce "come at me" when they play a hand, to
indicate that they think they will win the trick. The trick shall then continue
as normal (typically at heightened spite levels). If the player who announced
"come at me" successfully wins the trick, they are rewarded by being allowed to
view the top several cards of the deck and optionally swap one of them with a
card in their hand. If they fail to win, they are given [misplay](#misplays)
penalties. Any number of players are allowed to come-at-me during a trick, but
only one player can be successful (obviously). A player can also come-at-me
multiple times within the same trick as more hands are played, and their reward
or penalty shall be increased for each additional come-at-me.

It is a misplay to come-at-me when the hand played can only be beaten by [joker
hands](#joker-hands) (e.g. a single 2 when not under numerical consec) or cannot
be beaten (e.g. a 2 when under suited consec), or if the player wins the trick
by playing a joker hand.

The base reward for a successful come-at-me is being allowed to view 3 cards.
The reward increases by 1 for each additional come-at-me by that player during
the same trick, and decreases by 1 for each successful previous come-at-me by
that player with no tricks being won by other players in between. For example,
if a player:

1. Wins a trick during which they come-at-me'ed twice;
2. Wins a trick without come-at-me;
3. Wins a trick during which they come-at-me'ed once;

Then their rewards shall be 4 (base reward + 1 for the additinal come-at-me)
and 2 (base reward - 1 for a subsequent come-at-me trick without a trick won
by other players in between), respectively. If the reward becomes negative,
that number of misplay penalties shall be applied.

A player is not required to actually view their reward cards (e.g. they think
their hand is already optimal), but they must declare what their reward count
is. An incorrect declaration is a misplay. It is also a misplay to swap more
than one card from their hand, or discard an incorrect number of cards after
viewing/swapping.

The base penalty for a failed come-at-me is a [misplay](#misplays) penalty, and
it increases by 1 for each additional come-at-me during the same trick.

# Winners and Losers

## Scoring

At the end of each round, winners and losers will gain and lose points in their
scores, respectively. The first player to finish their hand gets +2, the second
player to finish gets +1, the second last player to finish gets -1, and the last
player (the loser) gets -2. A player's score accumulates across rounds and is
calculated as follows:

1. Decay their current score by 1 towards 0. For example, if their current score
   is -3, they shall decay to -2; if their current score is 4, they shall decay
   to 3.
2. Reset their score to 0 if they did not finish in the same half as the last
   round. For example, if there are 6 players at the table and a player finished
   among the top 3 players last round, and was among the bottom 3 players this
   round, their score is reset to 0. If there are an odd number of players at
   the table, the middle player is always considered to be "in the other half".
3. Add the reward/penalty points from this round.

When a late joiner comes to the table, they become the loser and gets -2, and
the rankings of other players are shifted up by 1 place.

## Card Swapping

At the beginning of each round, cards are swapped based on the players' scores.
Players with positive scores shall put down their lowest ranked card(s) into a
pile, and those with negative scores shall put down their highest ranked card(s)
into another pile. The absolute value of a player's score indicates the number
of cards they shall put down.

Then, players with positive scores shall pick up cards from the high cards pile,
and players with negative scores shall pick up cards from the low cards pile,
equal to the number of cards they previously put down.

If there is an imbalance between the number of cards in the two piles, random
cards from the top of the deck shall be added to the short pile. If there are
excess cards remaining after card swapping has occurred, they shall be revealed
and discarded.

# Misplays

A key reason for Spite having such a complicated ruleset is to induce misplays.
A misplay occurs when:

- Playing an invalid/malformed hand;
- Playing a hand that does not beat the previous hand in the trick;
- Incorrectly calling "misplay" on another player;
- Dropping card(s) on any food, liquid, sticky, or greasy substance (also known
  as a "misplate" if they were dropped onto a plate containing such substances),
  or dropping card(s) on the floor (except when dealing);
- and any other misplay situations already mentioned elsewhere in these rules.

Any card(s) dropped face-up on the table (accidentally or otherwise) shall be
considered to have been "played" for the purpose of determining misplays. If the
dropped card(s) form a valid play then they shall stand and the player is not
allowed to rescind them.

If a player plays out of turn, all player(s) who could have played shall still
have the option to play. If, after those players have played or passed, the
out-of-turn play is still valid then it shall stand, otherwise it is a misplay.
The skipped players are strongly encouraged to play hands that would cuase the
out-of-turn play to become invalid.

If a player has misplayed:

- Any [fake jokers](#fake-jokers) held by that player are immediately forfeited
  and returned to the fake joker pile.
- They are not allowed to play in the current trick, without the possibility of
  buying back, if the misplay occurred during a trick.
- They must skip the number of turns in the next trick(s) equal to their misplay
  penalty count. They may then choose to buy back into the trick.

If a misplay occurs due to incorrect [buy back](#buy back), and the player has
already seen some or all of the buy-back cards, those cards shall be discarded.
