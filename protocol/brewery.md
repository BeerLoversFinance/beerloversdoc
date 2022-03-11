# Brewery

## The Brewery User Interface

![The Brewery user interface](<../.gitbook/assets/img1.png>)

Please take a look at each element of the Brewery user interface and what it means.

1. **NEXT EPOCH**\
   The amount of time remaining until the next epoch.
2. **CURRENT EPOCH**\
   The number of the current epoch.
3. **BEER Price(TWAP)**\
   The TWAP (time-weighted average price) of the BEER peg. The Brewery only mints new BEER as rewards for BARREL stakers when this value **is above 10.1** **at the end of the current epoch**.
4. **APR**\
   The yield for BARREL stakers in the Brewery **if the Brewery was printing every epoch**. This calculation is based on **the last recorded print in the Brewery**.
5. **BARRELS STAKED**\
   ****The total amount of BARREL currently staked in the Brewery.
6. **BEER Earned**\
   ****The amount of BEER you've earned as rewards for staking BARREL in the Brewery.
7. **BARREL Staked**\
   The amount of BARREL you currently have staked in the Brewery.

### Brewery Specifications

* Epoch duration: 6 hours
* Any interaction with the Brewery (staking/unstaking BARREL or withdrawing BEER rewards) will **lock your staked BARREL for 6 epochs and BEER rewards for 3 epochs.**&#x20;
*   Distribution of BEER during expansion (Boardoom printing):

    **60%** goes to Brewery BARREL stakers as rewards\
    **20%** goes to BEER stakers (xBEER)

    **10%** goes to DAO fund

    **10%** goes to dev fund
* Epoch Expansion: The current expansion cap is based on the currently circulating BEER supply (see [BEER Distribution](beer-distribution.md) for details). If there are bonds to be redeemed, 65% of minted BEER goes to the treasury until its sufficiently stocked to satisfy future bond redemption.

{% hint style="info" %}
Note that the Brewery **does not** print any rewards for BARREL stakers when the Brewery TWAP < 1.01.
{% endhint %}

## Brewery FAQ

### **1. Once BOTTLEs are issued, does the Brewery stop printing BEER until we are above peg again?**

Staking BARREL will only give you BEER rewards when the price of BEER is above the peg (1 BEER to 10 FTM), but not when it is under the peg.

### **2. What happens if I interact with the Brewery in any way? Are there any lockup periods?**

Yes, there are two lockup timers. One for BEER rewards and one for staked BARREL. **Any interaction with the Brewery will reset both timers.** The lockup period for withdrawing BEER rewards is **3 epochs (18 hours)**, or **6 epochs (36 hours)** to unstake your BARREL.

### **3. Are the Brewery rewards pro-rated by time? For example, if I stake three hours before the end of an epoch versus five hours before the end of an epoch, would I get different rewards?**

No, Brewery rewards are determined by how much you have staked at the time of printing (i.e., at the end of one epoch and the start of the other). It doesn't matter if you stake three hours before or thirty seconds before the emissions occur.

### 4. If I remove my BARREL from the Brewery without first collecting my BEER, will they be lost forever?

No, they will still be there to collect whenever you need.

### 5. The Brewery APR dropped because we're in a "debt phase." What does that mean?

A debt phase takes place during expansion epochs that start after a contraction period where there are still BOTTLE to be redeemed.

65% of expansion during a debt phase is allocated to the treasury fund to prepare for subsequent BOTTLE redemption down the road. This amount is always reserved, regardless of whether BOTTLE holders are redeeming bonds or not.

Once enough BEER is sufficiently stocked in the treasury to satisfy the redemption of all circulating BOTTLE, expansion rates will resume to normal.

### 6. If we're in a debt phase, how long will it last until the Brewery continues printing as normal?

The debt phase will last as long as is necessary to adequately pay back outstanding BOTTLE debt. Please keep in mind that the DAO will also need to collect a little extra, as there needs to be a cushion to cover the bonus premiums when people redeem BOTTLE over peg.\
\
There's no exact way of calculating how many epochs it will take, since the protocol doesn't know exactly when people will redeem their BOTTLE. The debt phase cannot end until the treasury has enough BEER to cover the redemption of all outstanding BOTTLEs plus a premium.

### 7. At the end of the epoch, the Brewery did not print BEER, but then no BOTTLE(s) were issued either. Why?

There is a balanced state "at peg" when BEER's TWAP is between 1.00 and 1.01, which results in no contraction or expansion of the circulating supply of BEER. This is referred to as a **zen epoch**.

### 8. If BEER continues to climb above the price of the peg, will that influence how long the debt phase lasts?

Depending on the price of BEER, the Brewery print will have to adjust to provide a buffer for any unclaimed BOTTLE. As the price of BEER climbs above the peg, more BEER needs to be distributed to the treasury to account for BOTTLE redemption plus premiums.

### 9. How can I figure out what my future BEER rewards will be from the Brewery?

Let's take a look at a simplified example for a _non-debt phase_: say you have 1 BARREL staked out of 10 total BARRELss staked in the Brewery. In this case, you will receive 10% of the total BEER printed in the Brewery.&#x20;

For this example we are assuming that there is a total circulating supply of 10,000 BEER and the current expansion rate is at 4%, so a total of 400 BEER will be printed in the Brewery. Under the protocol's current rules, 60% of those newly printed BEER will be distributed to BARREL stakers in the Brewery. (See the [BEER Distribution](beer-distribution.md) page for more details on how BEER is distributed within the protocol.)\
\
Therefore, you would get: ((0.04 _\*_ 10000) _\*_ 0.6) \* (1/10) = **24 BEER**.\
\
Thus, the formula to calculate your rewards is as follows:\
((_ExpansionRate_ \* _CirculatingBEERSupply)_ \* 0.6) \* (_YourBarrelStake_ / _TotalBarrelStaked_)

### 10. How long will it take for BARREL to pay itself off from BEER rewards based on current prices?

This will vary constantly as the APR in the Brewery fluctuates, along with other variables such as the price of BEER.

&#x20;For a quick estimation, however, you can do the following:

1. Take the total APR shown in the Brewery and divide that by 365 to get the daily APR. (For this example we will say the daily APR is 5%.)
2. Multiply that daily APR by the current market price of the total BARREL you have staked to see what your daily rewards are. (In this example, we have 5 BARREL, each worth $500, for a total amount staked of $2500. Your daily return in this case would be $2500 \* 0.05, which comes out to $125 per day.)
3. Take your initial buy-in price for BARREL and divide it by your daily rewards. If you bought these 5 BARREL at a higher price, say $700 for example, in the current market conditions you would recover your initial investment of $3500 in 3500/125 or 28 days.
