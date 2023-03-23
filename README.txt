This contract implements a simple supply chain where products can be added and their ownership can be transferred. The contract keeps track of the current owner, previous owners, and history of each product.

The Product struct contains the current owner of the product, an array of previous owners, and an array of strings representing the history of the product.

The addProduct function adds a new product to the supply chain. It sets the initial product info with the caller as the current owner and an empty array of previous owners and history. It also adds the initial history item provided as an argument.

The transferProduct function transfers ownership of a product to a new owner. It first checks that the caller is the current owner of the product. If the caller is the current owner, it updates the product info by setting the new owner as the current owner, pushing the previous owner to the array of previous owners, and adding the history item provided as an argument to the array of history.

The getCurrentOwner function returns the current owner of a product.

The getPreviousOwners function returns an array of previous owners of a product.

The getHistory function returns an array of strings representing the history of a product.
