# Tokens

### BEER - beerlovers.finance Token

![beerlovers.finance (BEER)](<../.gitbook/assets/BEER.png>)

Contract: [0xf9525ee760D1859D77177D9A09B52cd81Ba005d3](https://ftmscan.com/address/0xf9525ee760D1859D77177D9A09B52cd81Ba005d3)

The BEER token is designed to be used as a medium of exchange. The built-in stability mechanisms within the protocol aim to maintain BEER's peg of 1 BEER = 10 FTM in the long run.&#x20;

{% hint style="warning" %}
Note that BEER **actively pegs via an algorithm**, but that **does not mean** it will be valued at 10 BEER to 1 FTM at all times as **it is not collateralized**. **BEER is not to be confused for a crypto or fiat-backed stablecoin.**
{% endhint %}

### BARRELS - BEER Shares

![SHARE](<../.gitbook/assets/BARREL.png>)

Contract: [0xCA565e364ac8C48CBB3B2C95DD82d5AcA16F991c](https://ftmscan.com/address/0xCA565e364ac8C48CBB3B2C95DD82d5AcA16F991c)

BEER Shares (BARREL) are one of the ways to measure the value of the Beer Money Protocol and shareholder trust in its ability to consistently maintain BEER close to peg. During epoch expansions the protocol mints BEER and distributes it proportionally to all BARREL holders who have staked their tokens in the [**Brewery**](brewery.md).

BARREL has a **maximum total supply of 65,001** tokens distributed

{% hint style="success" %}
The BeerLovers team will use the treasury funds in any way that they feel is best for the long-term success of the protocol.&#x20;
{% endhint %}

### [BOTTLE - BEER Bonds](bonds-mechanism.md)

![BOTTLE](<../.gitbook/assets/BOTTLE.png>)

Contract: [0x2624b2EE08128ABd9a55aA84013A37a20Edc9d9d](https://ftmscan.com/address/0x2624b2EE08128ABd9a55aA84013A37a20Edc9d9d)

The main purpose of BEER Bonds (BOTTLE) is to help incentivize fluctuations in the BEER supply during epoch contraction periods. When the TWAP (time-weighted average price) of BEER falls below 1 to 10 FTM, BOTTLEs are issued and can be bought with BEER at the current price. Exchanging BEER for BOTTLE burns BEER tokens, taking them out of circulation (deflation) and helps to get the price back up to peg. These BOTTLE can be redeemed for BEER when the price is above peg in the future, plus a premium based on how high above peg we currently are. This conversely creates inflation and subsequent sell pressure for BEER when it is above peg, helping to push it back toward 1 BEER to 10 FTM ratio.

{% hint style="info" %}
Unlike early algorithmic protocols, BOTTLEs do not have expiration dates.
{% endhint %}

All BOTTLE holders will be able to redeem their BOTTLE for BEER tokens as long as the treasury has a positive BEER balance, which typically happens when the protocol is in epoch expansion periods.
