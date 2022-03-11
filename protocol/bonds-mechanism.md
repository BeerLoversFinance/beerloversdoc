# Bonds (BOTTLE)

![The "Pit", where you can interact with the protocol's bonding mechanism](<../.gitbook/assets/img2.png>)

### What are BOTTLE (Bonds)?

Bonds are unique tokens that can be utilized to help stabilize BEER price around peg (1 BEER = 1 FTM) by reducing the circulating supply of BEER if the TWAP (time-weighted average price) goes below peg.

### When can I buy BOTTLE (Bonds)?

BOTTLE can be purchased only during periods of supply contraction and when the TWAP of BEER is below 1.

At the beginning of every new epoch during contraction periods, BOTTLEs are issued in the amount of 3% of BEER's circulating supply, with a max debt amount of 35%. This means that if bonds reach 35% of the circulating supply of BEER, no more bonds will be issued.

{% hint style="info" %}
Note that during a zen epoch (when an epoch ends with a TWAP between 1.0 - 1.01), **no BOTTLE will be issued, even though the Boardroom does not print.**
{% endhint %}

{% hint style="danger" %}
BOTTLE TWAP (time-weighted average price) is based on the BEER TWAP from the previous epoch as it ends. In other words, the BEER TWAP is real-time but the BOTTLE TWAP is not.
{% endhint %}

### Where can I buy BOTTLE (Bonds)?

You can buy BOTTLEs if any are available through [beerlovers.finance](https://beerlovers.finance/bonds) in the [bond](https://beerlovers.finance/#/bond). Anyone can buy as many BOTTLEs as they want as long as they have enough BEER to pay for them.

There is a limit of available BOTTLEs per epoch during contraction periods (3% of BEER's current  circulating supply), and are sold first-come-first-serve.

### Why should I buy BOTTLE (Bonds)?

The first and most important reason to buy BOTTLE is that they help to maintain the peg, but they are not the only measure in place to keep the protocol on track.&#x20;

BOTTLEs don't have an expiration date, so you can view them as an investment in the long-term health of the protocol to be redeemed for a premium at a later date.

#### Incentives for Holding BOTTLE

The idea is to reward BOTTLE buyers for helping the protocol, while also protecting the protocol from being manipulated by big players.

So after you buy BOTTLE using BEER, you have two possible ways to get your BEER back:

1. Sell back your BOTTLE for BEER **while the peg is between 1 - 1.1** (1 BEER = 10 FTM) with no redemption bonus. This is in place to prevent an instant dump as soon as peg is recovered.
2. Sell back your BOTTLE for BEER **while the peg is above 1.1** (1 BEER = 10 FTM) with a bonus redemption rate.

The longer you hold, the more both the protocol and you benefit from BOTTLE.

{% hint style="success" %}
Example:

1. When BEER = 8, burn 1 BEER to get 1 BOTTLE (BOTTLE price = 0.8)
2. When BEER = 11.5, redeem 1 BOTTLE to get 1.105 BEER (BOTTLE price = 12.7)&#x20;
{% endhint %}

So, which one is better?

If I buy BEER at 8, and hold it until 11.5 and then sell, I'm getting +$3.5 per BEER.

But, if I buy BEER at 8, burn it for BOTTLE, and redeem it at 11.5, I'm getting 11.05 BEER \* 11.5 (BEER current price) = 1,271 (+$4.7) per BOTTLE redeemed.

But, what if getting back to peg is taking too long?

We will adjust our use cases to have different behaviors on contraction and expansion periods to benefit both BEER and BOTTLE holders when needed.

### What is the formula to calculate the redemption bonus for BOTTLE?

To encourage the redemption of BOTTLE for BEER when BEER's TWAP > 10.1 and in order to incentivize users to redeem bonds at a higher price, BOTTLE redemption is designed to be more profitable with a higher BEER TWAP value. The BOTTLE to BEER ratio is 1:R, where R can be calculated using the formula as shown below:

$$
R=10+[(BEERtwapprice)-1)*coeff)]
$$

$$
coeff = 7
$$

### When can I swap BOTTLE for a premium?

You can only redeem BOTTLEs for a premium when the previous epoch's TWAP is greater than 10.1.
