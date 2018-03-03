## Basic info

Supported `ping` methods:
* `active` - ask server every N time, recalculating current ping based on response
* `passive`- calculate ping after skill cast

By default: `active`

## Information

### Passive method

Author: Undefined

Pros: 
* Not detectable
* Actual ping value in battle without delays 

Cons:
* 1-3 first skills can be a bit delayed in battle
* Effect can be different for users
* Your skills will be broken with bad settings

### Active method

Author: PinkiePie (edited by SaltyMonkey)

Pros: 
* Simple
* Stable

Cons:
* Detectable (in theory)
* For players with unstable connection can't get real values

## Configuration

### Mode

1) Open config.json (path `./config/config.json`)

2) Find "pingMethod" field and change it to `"passive"` or `"active"`

3) Edit "pingHistoryMax" field (`35+` for `"passive"`, `15-20` for `"active"` ping method)

### For users with unstable connection

4) Find "pingSpikesLimit" and set it to "true"

5) Find "pingSpikesMin": field and set it to:  `your average minimal ping - 10`

6) Find "pingSpikesMax" field and set it to: `your average ping + 30`

### WARNING №1! Wrong settings for spikes can ruin your gameplay.

### WARNING №2! Ping spikes control CAN'T work with constant spikes.
