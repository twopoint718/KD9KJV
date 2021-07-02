---
layout: post
title:  "QSO Protocol"
date:   2021-07-01 21:21:00 -0500
---

I'm learning more about the standard QSO Protocol.
Okay, well there really isn't a _standard_ as such but the Long Island CW Club has something to that effect.
There's a general style about how the conversation should go.
It covers the info that you need to send as part of any [QSO](https://en.wikipedia.org/wiki/Contact_(amateur_radio)) but then also how the contact ought to flow.
There are lots of common abbreviations used to make the contact more brief.
Also there are [prosigns](https://en.wikipedia.org/wiki/Prosigns_for_Morse_code) thrown in as well.
As a slight aside, I have a strong suspicion that a connection can be drawn between morse code prosigns and computer [control characters](https://en.wikipedia.org/wiki/Control_character).

Anyhow, I've been learning about this but I wanted something that was a little bit more in our _modern visual vernacular_.
So, here it is a brief QSO as if it were a text message chat:

<style>
  .speech-bubble-right {
    font-family: "Courier";
    font-size: 1.2em;
    color: white;
    font-weight: bold;
    position: relative;
    background: #0099aa;
    border-radius: .4em;
    width: 15em;
    padding: 1em;
    margin-left: auto;
    margin-bottom: 1.8em;
  }
  
  .speech-bubble-right:after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    width: 0;
    height: 0;
    border: 30px solid transparent;
    border-top-color: #00aabb;
    border-bottom: 0;
    border-right: 0;
    margin-left: -15px;
	margin-bottom: -30px;
  }
  
  .speech-bubble-left {
	font-family: "Courier";
	font-size: 1.2em;
	font-weight: bold;
	position: relative;
	background: #c1c1c1;
	border-radius: .4em;
	width: 15em;
	padding: 1em;
	margin-bottom: 1.8em;
  }
  
  .speech-bubble-left:after {
	content: '';
	position: absolute;
	bottom: 0;
	left: 50%;
	width: 0;
	height: 0;
	border: 30px solid transparent;
	border-top-color: #c1c1c1;
	border-bottom: 0;
	border-left: 0;
	margin-left: -15px;
	margin-bottom: -30px;
  }
  
  .container {
	margin: auto;
  }
  
  .prosign {
	text-decoration: overline;
	font-style: italic;
  }
</style>

<div class="container">
  <div class="speech-bubble-right">
    <abbr title="[is this frequency] busy">QRL</abbr>?
  </div>
  
  <div class="speech-bubble-right">
    <abbr title="[is this frequency] busy">QRL</abbr>?
  </div>
  
  <div class="speech-bubble-right">
    <abbr title="calling all stations">CQ</abbr>
    <abbr title="calling all stations">CQ</abbr>
    <abbr title="this is/from">DE</abbr>
    <abbr title="(calling station's callsign)">KD9KJV</abbr>
    <abbr title="(calling station's callsign)">KD9KJV</abbr>
    <abbr title="over [to you]">K</abbr>
  </div>
  
  <div class="speech-bubble-left">
    <abbr title="(calling station's callsign)">KD9KJV</abbr>
    <abbr title="this is/from">DE</abbr>
    <abbr title="(answering station's callsign)">K1PDQ</abbr>
    <abbr title="(answering station's callsign)">K1PDQ</abbr>
    <abbr title="over [to you]">K</abbr>
  </div>
  
  <div class="speech-bubble-right">
    <abbr title="(answering station's callsign)">K1PDQ</abbr>
    <abbr title="from">DE</abbr>
    <abbr title="(calling station's callsign)">KD9KJV</abbr>
    <abbr title="good morning">GM</abbr>
    <abbr title="thanks">TNX</abbr>
    <abbr title="your signal is">UR</abbr>
    <abbr title="readability, strength, tone">599</abbr>
    <abbr title="near">NR</abbr>
    <abbr title="(city)">MADISON</abbr>,
    <abbr title="(state)">WI</abbr>
    <abbr title="pause/break (prosign)"><span class="prosign">BT</span></abbr>
    NAME
    <abbr title="(calling station's name)">KIT</abbr>
    <abbr title="how copy?">HW?</abbr>
    <abbr title="(answering station's callsign)">K1PDQ</abbr>
    <abbr title="this is/from">DE</abbr>
    <abbr title="(calling station's callsign)">KD9KJV</abbr>
    <abbr title="over to you">K</abbr>
  </div>
  
  <div class="speech-bubble-left">
    <abbr title="received as transmitted/roger">R</abbr>
    <abbr title="your signal is">UR</abbr>
    <abbr title="Readability, strength, tone">RST</abbr>
    IS
    <abbr title="readability, strength, tone">599</abbr>
    <abbr title="pause/break (prosign)"><span class="prosign">BT</span></abbr>
    <abbr title="operator">OP</abbr>
    <abbr title="here">HR</abbr>
    JIM
    <abbr title="pause/break (prosign)"><span class="prosign">BT</span></abbr>
    <abbr title="location">QTH</abbr>
    DALLAS, TX
    <abbr title="end of message"><span class="prosign">AR</span></abbr>
    <abbr title="(calling station's callsign)">KD9KJV</abbr>
    <abbr title="this is/from">DE</abbr>
    <abbr title="(answering station's callsign)">K1PDQ</abbr>
    <abbr title="over [to you]">K</abbr>
  </div>
  
  <div class="speech-bubble-right">
    <abbr title="thanks">TNX</abbr>
    <abbr title="for">FER</abbr>
    <abbr title="communication/contact">QSO</abbr>
    <abbr title="best regards">73</abbr>
    <abbr title="end of contact"><span class="prosign">SK</span></abbr>
    <abbr title="(answering station's callsign)">K1PDQ</abbr>
    <abbr title="this is/from">DE</abbr>
    <abbr title="(calling station's callsign)">KD9KJV</abbr>
    <abbr title="over [to you]">K</abbr>
  </div>
</div>

Things to note about the above exchange:

First are [Q Codes](https://en.wikipedia.org/wiki/Q_code#Amateur_radio).
Their meaning is modified by whether or not they're followed by a question mark, changing the sense to be a question.
_QRL?_ means "are you busy?" (or is the frequency busy/in-use), but _QRL_ would mean "I'm busy."

The items marked typographically with overbars are _prosigns_.
These are created by running the characters of the prosign together.
In CW there's a standard amount of space between the letters of a word, but in a prosign that spacing is reduced.

SK - this prosign has a dual meaning. Here it means that you're done with the contact.
But it is also used in a metaphorical way to denote the fact that the radio operator has died.
In the latter sense, "SK" is listed after the person's callsign.

It may seem odd that some CW abbreviations are the same length.
Why would we use "FER" instead of "FOR"?
The answer is that dashes take longer to send than dots, 3 times as long, usually.
Speed-wise you're trading ..-. --- .-. (FOR) for the quicker ..-. . .-. (FER). 
Similarly, the numbers are longer than the letters, and so you'll often see letters used in place of numbers.
"5NN" is used in signal reports instead of "599".
Again, a place where typographically it seems like a wash, the same three characters either way, but in morse it's _much_ faster.

_Seriously_ though, prosigns are just so obviously control characters.
Look how they're used!
