---
layout: post
title: "Pure intonation vs. 12 equal temperament musical intervals"
date: 2025-03-26
---

Given a musical sound <span markdown="0">\(X\)</span>, we can
characterize its pitch by its fundamental frequency
<span markdown="0">\(f(X)\)</span>. A note at twice that frequency
is an octave above <span markdown="0">\(X\)</span>. Two notes an
octave apart have a particularly close musical relationship, and
their frequencies stand in the ratio
<span markdown="0">\(2:1\)</span>.

One way to divide the octave into twelve equal intervals is to put
the frequencies in a geometric progression. Starting from a note
<span markdown="0">\(X\)</span>, the note
<span markdown="0">\(k\)</span> semitones above it has frequency

$$
f(X)\,2^{k/12}.
$$

The ratio between any two consecutive notes is therefore always
<span markdown="0">\(2^{1/12}\)</span>. This tuning is called
*12-tone equal temperament*, or **12-ET**. Modern pianos and many
other instruments are normally tuned around this system.

You may also have heard that the perfect fifth—the interval from
<span markdown="0">\(C\)</span> to the
<span markdown="0">\(G\)</span> above it—has the simple frequency
ratio <span markdown="0">\(3:2\)</span>. But in 12-ET, a fifth spans
seven semitones, so

$$
f(G)=f(C)\,2^{7/12}\approx f(C)\times 1.4983.
$$

That ratio is close to, but not exactly,
<span markdown="0">\(1.5\)</span>. What's happening here?

<!--more-->

The two ratios are very close: the equal-tempered fifth is about two
cents narrower than the pure <span markdown="0">\(3:2\)</span> fifth.
Depending on the sounds, the listener, and the context, that
difference may be subtle; sustained notes can also make it audible
through beats. To understand why the simple ratio matters, we can look
at the harmonic series.

A pitched sound from an instrument such as a piano contains a
fundamental frequency and higher partials. In an ideal harmonic
series, these have frequencies

$$
f(C),\quad 2f(C),\quad 3f(C),\quad 4f(C),\quad \dots
$$

Their relative strengths contribute to the
[timbre of the instrument](https://en.wikipedia.org/wiki/Timbre).
Real instruments can depart somewhat from the ideal series—for
example, piano strings have some inharmonicity.

Notice that the frequencies <span markdown="0">\(2f(C)\)</span> and
<span markdown="0">\(3f(C)\)</span> stand in the ratio
<span markdown="0">\(3:2\)</span>: they form a pure fifth. Similarly,
the third and fourth harmonics stand in the ratio
<span markdown="0">\(4:3\)</span>, and the third and fifth in the ratio
<span markdown="0">\(5:3\)</span>.

These relationships give us a reason to pay attention to simple
ratios: ratios whose numerator and denominator appear early in the
sequence <span markdown="0">\(1,2,3,4,\dots\)</span>. *Just
intonation* (JI), also called pure intonation, uses ratios of whole
numbers to tune intervals. Here is one possible justly tuned
<span markdown="0">\(C\)</span> major scale:

| Note | C | D | E | F | G | A | B | C |
|---|---|---|---|---|---|---|---|---|
| Ratio from C | 1/1 | 9/8 | 5/4 | 4/3 | 3/2 | 5/3 | 15/8 | 2/1 |
| Cents | 0 | 204 | 386 | 498 | 702 | 884 | 1088 | 1200 |

A **cent** expresses an interval on a logarithmic scale. If
<span markdown="0">\(X\)</span> is above
<span markdown="0">\(C\)</span>, we can write

$$
f(X)=f(C)\,2^{\mathrm{cents}(X)/1200}.
$$

An octave is 1200 cents, and each semitone in 12-ET is exactly 100
cents. The corresponding 12-ET
<span markdown="0">\(C\)</span> major scale therefore has cent values
0, 200, 400, 500, 700, 900, 1100, and 1200.

Here is *Clair de Lune* played in just intonation:

[Listen on YouTube](https://www.youtube.com/watch?v=ub9LhEmmVKY)

Harmonic-series-based approaches are among the early ways of thinking
about tuning. For example,
[Pythagorean tuning](https://en.wikipedia.org/wiki/Pythagorean_tuning)
builds intervals from pure fifths. The marked positions on the
soundboard of the Chinese *guqin* also help players find harmonics.
Many tuning systems have been used across musical traditions and
periods.

## A difficulty with a fixed just tuning

Suppose we tune notes according to the
<span markdown="0">\(C\)</span> major table above, then want to play
in <span markdown="0">\(D\)</span> major. An important interval is
now the fifth from <span markdown="0">\(D\)</span> to
<span markdown="0">\(A\)</span>. Using their ratios to
<span markdown="0">\(C\)</span>, we get

$$
\frac{f(A)}{f(D)}
=
\frac{5/3}{9/8}
=
\frac{40}{27}
\approx 1.4815.
$$

The fifth from <span markdown="0">\(C\)</span> to
<span markdown="0">\(G\)</span> has the pure ratio
<span markdown="0">\(3/2\)</span> by construction, while this
<span markdown="0">\(D\)</span>–<span markdown="0">\(A\)</span>
fifth is narrower. In cents, the two intervals are approximately

$$
1200\log_2(3/2)\approx 701.955
$$

and

$$
1200\log_2(40/27)\approx 680.449.
$$

The difference is about 21.5 cents. How noticeable a difference is
depends on the listener, timbre, duration, and musical context, but
this is a substantial change in the size of the interval.

This illustrates a difficulty with a **fixed** set of justly tuned
notes: intervals that play the same role in different keys need not
have the same ratios. Musicians can adjust pitches or use additional
notes to accommodate this, but a fixed-pitch instrument has to make
choices.

Equal temperament takes another approach. Because every semitone has
the same ratio, an interval spanning a given number of semitones has
the same size in every key. Twelve divisions also provide useful
approximations to several simple ratios: the perfect fifth and
perfect fourth, for example, are each about two cents away from their
pure counterparts.

## Listening and familiarity

Twelve-tone equal temperament became widespread over a long period;
other temperaments and tuning practices have also been important in
Western music. Bach explored music in many keys, though his exact
preferred temperament remains a subject of debate.

When I listen to a major third in just intonation, it can sound
strange or unfamiliar to me. Perhaps you felt something similar
listening to the *Clair de Lune* recording. Experiences like this
make me wonder how much our sense of sonic beauty is shaped by
culture and listening habits.

If you're interested in other tuning systems and the ideas behind
them, explore the [Xenharmonic Wiki](https://en.xen.wiki/w/Main_Page).
