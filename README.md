# SPEROEXCHANGE-JS
A libary for SPERO EXCHANGE API written in JS
# SPEROEXCHANGE-JS

A libary for SPERO EXCHANGE API written in JS

Here is a full implimentation of the SPERO EXCHANGE API in a nodejs NPM package.


> accessKey secretKey listMarkets allMarketsTicker ticker account
> allDeposits deposits deposit depositAddress orders ordersAll
> createOrder order cancelOrder clearAllOrdersSide clearAllOrders
> orderBook depth trades myTrades kLine timestamp

    //listMarkets
    //Get all available markets
    /*
    listMarkets(function(res){
        if(!res.error){
                //console.log(res);
                for (var key in res) {
                        if (res.hasOwnProperty(key)) {
                                console.log(res[key]);
                        }
                        }
        }else{
                console.log(res)
        }
    });
    */

    //createOrder
    //Create a Sell/Buy order
    /*
    createOrder("sperodoge", "buy", "5.0", "0.000000200", function(res){
        if(!res.error){
            console.log(res);
        }else{
           console.log("ERROR: " + res)
        }
    });

    */

# Example
Install:

    npm install spero

Example:

        //Import module
        var  spero  =  require("./spero.js");
            //Settings / Config
        spero.accessKey  =  "";
        spero.secretKey  =  ""

        spero.allMarketsTicker(function(res){
                if(!res.error){
                    console.log(res)
                }else{
                    console.log(res)
                }
        });

For a more detailed example, please see "mm.js" in the git directory.
