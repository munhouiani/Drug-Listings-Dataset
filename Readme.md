Blog post: https://blog.munhou.com/2021/09/29/Drug-Listing-Dataset/

[Gwern published a collection of Darknet Market Archives in 2015](https://www.gwern.net/DNM-archives). While the dataset is comprehensive, a lot of works need to be done before we can start analyzing it. I put some effort to organize Gwern's archives, extract only drug-related content, and construct a drug listing dataset in csv format.

## Coverage
Drug listing data are parsed from the following marketplaces.

* 1776
* Abraxas
* Agora
* Evolution
* Nucleus
* Outlaw Market
* Silk Road 2
* The Marketplace

## Data Field
* `product_title`: The title of the item.
* `product_description`: The description of the item. This field could be null as some of the listing archives are damaged.
* `ship_from`: The place where the item is shipped from. This field could be null as shipping information isn't required for certain marketplaces.
* `ship_to`: The place where the item is shipped to. This field could be null as shipping information isn't required for certain marketplaces.
* `seller`: The seller of the item.
* `price`: The price of the item, the currency is not yet unified.
* `source`: The name of the marketplace where this item is posted.
