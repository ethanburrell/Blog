---
layout: post
title: Moving Averages
---

Over the course of this post I will be explaining moving averages and how I think they can be used to predict the future movement
of the market. Please note, I am not endorsing that you should go out and trade with this type of algorithm, I am showing that
Technical/Quantitative Analysis for financial markets can be very powerful. The data in this is a "toy example" and should not be used to base real trading off of. Thank you for reading.

# Moving Averages
Welcome to my first post on indicators for the stock market, this is going to focus on Moving averages, a widely used indicator for all traded quantities.

I'm sure that you are all familiar with the 5 most common statistical measures: mean, median, mode, range, and standard deviation. These metrics are great at describing a large dataset, however they can also be used on a small amount of data to "smooth out" the values and create a simple representation of what has recently happened. You'll see what I mean by smoothing out in a second.

![alt text](/blog/public/images/Moving-Averages-1/Price vs Global Average.jpg "Global Average")


This is a graph of the price vs. the *global average*. The global average is the average of the price over a time period, the sum of all of the points on the "Price" line divided by the number of days. This is a great way to compare stocks over a specific
period of time, but not necessarily usefule to visualize the activity of a stock over the short term. That's where a moving
average comes in.

![alt text](public/images/Moving-Averages-1/Price vs. Moving Average.jpg "Moving Average")


Pictured above is a *moving average*. This looks like a smoothed out and delayed copy of the price graph. To calculate this, choose a certain number of days and find the average value of the price over this time period, repeat this for each day, and this
produces the moving average.

### Why are moving averages used?

The general rule with moving averages is that the average will eventually return and intersect with the actual price, this makes
it an excellent indicator of the "true" underlying value of the commodity. When the moving average is far above the actual price,
the commodity is commonly undervalued and it is seen as a good time to buy. On the other had, when the moving average is far below
the price then the stock is commonly overvalued and it could be very profitable to sell and buy in later on.

Is this the real "true" value of the stock? No. However, people treat it like it is. This is just a tool to get more insight on
the trend of the stock, and in many cases perform informed buying and selling. Significant deviations between the two lines
generally return to the actual price, this insight and general rule of thumb is why traders use this indicator.

Notice how I am using the word *far* or *significant* to describe the distance between the moving average and the price, and
actually knowing when to buy and sell is the secret to making money while trading.

### When to know to buy and sell? When is there a significant enough difference?

Figuring out questions like these will make you the big bucks in economics. Finding whether or not to buy or sell is very
difficult, here are some theories that many people use.

We need a way to measure the difference between the moving average and the actual price...

##### Use Thresholds

One way to do this is to use a threshold. For example, if the price is 110% of the moving average the trader could sell. If the price is 90% of the moving average the commodity could be bought.

![alt text](/public/images/Moving-Averages-1/Price vs. MA Thresh.jpg "Moving Average with Thresholds")


It's even possible to check if the price is 10 cents over the moving average, or 10 cents under, and then make your decision off of this. Trading commodities with low fees (such as cryptos) commonly use this second practice.

##### Use Standard Deviations

This method uses standard deviations to determine how volatile a commodity is and then base trading off of that. Remember the
Normal Distribution from Statistics (or a Bell Curve)? This rule says that 97.7% of all values are inside of 2 standard
deviations from the mean(average) value. Even though stock/commodity prices are not normally distributed this rule can be
generally applied. See where this is heading?

![alt text](/public/images/Moving-Averages-1/Standard_deviation_diagram.png "Normal Distribution")

If the variance/behavior of the actual price is within 2 standard deviations of the mean, then the movement of the stock is not
noteworthy. As soon as the price gets outside of 2 standard deviations then a buy or sell should happen. This allows the trader
to make trading decisions that are different from the just noise. Say a certain stock is very vulnerable constantly making 5%
dips up and down, the standard deviation would be able to point out when the price is "out of the norm" and distinguish this from
it's general action. This helps us distinguish when to buy and sell and ensure that the algorithm is not trading based off of
noise (just general activity) of the stock.

![alt text](/public/images/Moving-Averages-1/Price vs MA Bollinger.jpg "Moving Average with Bollinger")


On wall street this is referred as a Bollinger Band®.
