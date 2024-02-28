## Candy Machine UI Setup Guide

**Introduction**

This guide outlines the steps to configure the user interface (UI) for your Candy Machine. This UI enables users to mint NFTs using your created SPL token via their Phantom wallets.

**Prerequisites**

* A configured Candy Machine with details in its `config.json` file, including:
    * Price
    * Quantity
    * Symbol
    * Seller fee basis points
    * SPL token account
    * SPL token
    * Go-live date
    * Creator details
* A designated Phantom wallet for minting
* A newly created SPL token

**Steps**

1. **SPL Token Setup**

   * If not already done, create an SPL token following Lesson Three guidelines. Note down its address.

2. **Update Candy Machine Config**

   * Edit your Candy Machine's `config.json` file and update these fields:
     * `splTokenAccount`: Replace with the created SPL token account address.
     * `splToken`: Replace with the SPL token address.

3. **UI Configuration**

   * Refer to the "Quick Node: Set Up a Minting Site" tutorial for instructions on building a UI for your Candy Machine. This UI allows users to connect their Phantom wallets and mint NFTs using the SPL token for payment.

4. **Adjust Minting Logic**

   * Modify your SPL project's minting logic (as per Lesson Three) to mint NFTs to the Phantom wallet address or adapt the transfer function to deliver minted NFTs to your Phantom wallet.

5. **Testing**

   * Thoroughly test the setup by transferring or minting your SPL token to a Phantom account.
   * Use the UI to mint NFTs, ensuring a smooth process for users paying with the designated SPL token.
