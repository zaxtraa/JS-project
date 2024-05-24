# JS-project
NFT Minting Script
This repository contains a simple JavaScript script for minting and listing NFTs (Non-Fungible Tokens). It allows users to mint unique NFTs with customizable attributes and list all minted NFTs along with their details.

Features
Mint NFTs: Users can mint NFTs by providing details such as name, eye color, shirt type, and bling.
List NFTs: The script enables users to list all minted NFTs along with their attributes.
Get Total Supply: Users can retrieve the total number of minted NFTs.
Usage
To use the script, simply run it in a JavaScript environment that supports ES6 syntax. You can customize the attributes of the NFTs by calling the mintNFT function with desired parameters. After minting NFTs, you can list them using the listNFTs function and retrieve the total supply with the getTotalSupply function.

Example
javascript
Copy code
const NFTs = []

function mintNFT (_name, _eyeColor, _shirtType, _bling) {
    // Function to mint a new NFT with provided attributes
    const NFT = {
        "name" : _name,
        "eyeColor" : _eyeColor,
        "shirtType" : _shirtType,
        "bling" : _bling
    }
    NFTs.push(NFT);
    console.log("Minted: " + _name)
}

// Example usage
mintNFT("James", "Green", "Black Suit", "Diamond Chain");
mintNFT("Kent", "Brown", "Black Suit", "Gold Chain");

listNFTs(); // List all minted NFTs
getTotalSupply(); // Get total supply of minted NFTs
License
This project is licensed under the MIT License.

