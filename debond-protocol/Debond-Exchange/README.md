## Debond Exchange: 

This package consist of contracts handling auctions  of bonds for the secondary market. Bond owners can onboard their bonds in batches  for auctioning them via FCFS.  


## Structures
1. Auction: This object  registers the parameters (bond address, auction price limit, time duration etc): 
    ```solidity
        //Auction  parameter for single bond. 
        struct AuctionParam {
        address owner; 
        uint256 startingTime; // timestamp when Auction is issued.
        uint256 endingTime;  // 
        uint256 duration; 
        address erc20Currency;
        uint256 maxCurrencyAmount;
        uint256 minCurrencyAmount;
        AuctionState auctionState;
        bool curvingPrice;
        address successfulBidder;
        uint256 finalPrice;
    }
    // batching the auctions by owner into single object.
    struct Auction {
        uint id;
        AuctionParam auctionParam;
        mapping(uint256 => ERC3475Product) products;
        uint256[] productIds;
    }
    ```

## Contracts: 


1. [Exchange](./contracts/Exchange.sol): This is the core contract that provides the wrapper  functions for checking the conditions  creation of auction (using `function createSecondaryMarketAuction()`) and bidding (from the side of users using `function bid()`) and then calling the functions from ExchangeStorage.
2. [Exchange storage](./contracts/ExchangeStorage.sol): This storage contract implements the core functions of exchange. this includes the creation , cancellation as well as transfer of the bonds / tokens after an successful auction.



## workflow steps: 

1. user selects on the frontend the different bonds with (classIds,NonceIds) to be auctioned , and then it calls :

    ```solidity
        function createSecondaryMarketAuction(
        address creator,
        address[] memory erc3475Addresses,
        uint256[] memory classIds,
        uint256[] memory nonceIds,
        uint256[] memory amounts, 
        address currencyAddress,
        uint256 maxCurrencyAmount,
        uint256 auctionDuration
    ) external;
    ```
the auction starts with price of whole batch decreasing  based on the linear formula. the price depends on the currentPrice of the bond (from debond-ERC3475 standard) as well as the initialPrice. also all the bonds of owner is transferred from the auction creator to exchange. 


2. frontend will present the price and status of all the auctions using the function 
    ```solidity
        
    function currentPrice(uint256 _auctionId) public view returns (uint256 auctionPrice);    


    // from ExchangeStorage
    function getAuction(uint auctionId) external view returns (AuctionParam memory auction);
    ```

3. Then there can be two conditions: Either the owner cancels the auction before anyone successfully bidding using  `function cancelAuction(uint256 _auctionId)` and the bonds will be returned to the owner. or there will be an successful bid by another user on the frontend using `function bid(uint256 _auctionId)` .



4. `ExchangeStorage.completeAuction`completes the auction by transferring the ERC20 tokens of the  successful bidder to the bond owner and at same time transferring the bonds from  Exchange to the successful bidder.   

## usage:

1. installing debond-exchange package. 
```bash
> npm install debond-exchange.
```

2. then inherit interface  in order to interact with exchange contract for creating your own custom secondary market contract / exchange.


## Diagrams: 

**1.[Exchange structure](docs/Exchange.png)**

**2.[Exchange Inheritance structure](docs/Exchange-storage-inheritance.png)**

