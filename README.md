# Trade Life Cycle Management Part 2

A trade, also called a deal, is an exchange of financial products from one entity to another. The life cycle of a trade is the fundamental activity of exchanges, investment banks, hedge funds, pension funds and many other financial companies.

 All the steps involved in a trade, from the point of order placed and trade execution through to settlement of the trade, are commonly referred to as the trade life cycle. Trade life cycle consists of a series of logical stages and steps.



1.	Pre-sale stage: Marketing persons from investment banks, brokers and dealers introduce various financial products and vehicles to clients. Investors or institutional fund managers survey the market and find the most suitable and competitive products.
2.	Trade execution: After trading negotiations between seller and buyer, an order is placed and the trade is executed. The completion of a buy or a sell order of a financial product is known as Trade Execution.
3.	Trade Capture: After trade execution, the trade is booked in the Front Office system, Middle Office Risk Management system and Back Office system.
4.	Trade Validation and Confirmation: Back office validates trade attributes and confirms trade settlement. Risk Management checks the valuation, risks and limits.
5.	Trade Settlement: Any fee or premium needs to be settled. For a periodic cash settlement trade, such as interest rate swaps or bonds, there is a process of simultaneous exchange of cash between parties at each payment date.
6.	Trade Termination: A trade may be expired at maturity or terminated early. The early termination  could be caused by a position sell or triggered by an early termination provision, such as auto call/cancel, knock-out, etc.

1.	Trade Validation
Users can define their own end-of-day (EOD) details. At each EOD, FinPricing will conduct EOD process automatically based on user definition - value and settle all trades and generate reports. Also FinPricing provides a manual interface for what-if analysis on valuation and validation.

After creating a new trade or loading an existing trade (see details in "How to book a single trade?" above), click the Market Data tab that is beside the Trade Detail tab. Then the user can either click the New button to input new market data or the Load button to extract the existing market data.

If the user chooses to input new market data by specifying the Valuation Date and then clicking the New button, the system knows what kind of market data needed for this trade and thus generates market data templates displayed in the main window.

After filling the market data and then clicking the Save button, an OK windows pops up if all data are in correct formats and value types. That means the new market data are saved into the system and ready to use.

Please note that FinPricing provides some market data to users. However, a user feels free to modify or provide their own market data. Those new or modified market data will be private to the user.

If user chooses to load existing market data by inputting a Valuation Date (say, 2/8/2018) and then clicking the Load button, a selection form appears in the main window. The user can select a date from pull-down menus. If all available dates are not what he wants, just select NA (not available). Then click the Extract button at the right of the row.

Note: the valuation date and the market data date are allowed to be different as sometimes a user conducts what-if analysis at a start-of-day (SOD), when the new market data are still not available. In that case, the user can use yesterday's data.

The market data on 2/8/2018 are loaded in the main window. Again the user can modify and save the market data.

After either new market data saved or existing market data loaded, the user can click the Pricing button. The calculation results will be presented in the Results tab.

Some notes on results 
– Sometimes, bond prices are available (quoted) in the market. If the bond price is provided, FinPricing will match the model price to the market price by calibrating a credit spread that reflects credit risk and liquidity risk. 

– If the market bond price is not given, FinPricing will compute the model price only based on the discount and/or forecast curves provided.

– FinPricing calculates sensitivities or Greeks based on market observable and liquid instruments, such as LIBOR rates, Eurodollar futures, and swap rates. This is the best market practice and convention as hedge and risk analysis are based on market observables. Most trading systems in the market compute Greeks relying on zero-rates, which is an easy way for convenience.

– To compute Greeks on market instruments, system/model needs to shock each instrument and then reconstruct curve one by one. The calculation is much more complex and time-consuming. But trickery cannot be used to gain advantage.

You can find more details at
https://finpricing.com/lib/IrCurveIntroduction.html
