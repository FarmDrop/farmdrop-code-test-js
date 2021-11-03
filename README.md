# Farmdrop Code Test (JavaScript)

This test must be written using React.

You can use any React boilerplate to help you get started (e.g. Create React App or Next.js)

It has been split into two parts:

## Product cards

Using the [supporting data file](data/products.json) or the graphql [endpoint](https://staging-graphql-gateway.farmdrop.com/graphql), display a grid of product cards matching the [design](mockups/products.png) as close as possible. Please ignore the "Family Roasts" overlay green tag. 
We have provided [fonts](fonts) for you which are similar to the fonts we use at Farmdrop and a set of svg [icons](icons).

We have attached the query which you can use for the graphql endpoint [here](graphql-query/query.txt)

- Each product has one or more variants. The information in the root of each node is the default variant. If the product has any additional `variants` (contained within the variants nested property) display them in a drop-down;
- Clicking on a variant in the drop-down will update the price on the product card `e.g. £12.10` and the price per unit `e.g. £25.20/kg`;
- If the product has no variants show the display name;
- If there is a sale price show the old price with a strikethrough and show the sale price in red as per the design;
- If there is sale text show in red beneath the dropdown;
- The width of each card in the grid should be dynamic never smaller than 200px and never larger than 360px.

## Testing

Please write some tests. It doesn't have to be a fully working test suite.

## Bonus functionality

If you do have the time you can complete the part two of this assignment which is to simulate adding the product to the basket using whichever state logic you prefer.

- When clicking the Add button the product card should show the quantity in the basket as per the design.
- We have attached a [header bar mockup](mockups/header.png) which we would also like you to build
- The basket should update with the quantity of products in the basket.

## Submission

Please clone this repository, write some code and update this README with a
guide of how to run it.

Either send us a link to the repository on somewhere like github or bitbucket
(bitbucket has free private repositories) or send us a git bundle.

    git bundle create yournamehere-farmdrop-code-test-js.bundle master

And send us the resulting `yournamehere-farmdrop-code-test-js.bundle` file.

This `.bundle` file can be cloned using:

    git bundle clone bundle-filename.bundle -b master directory-name


## Score Considerations

- To use typescript or not is your choice and it won't have any bearing on final score;
- To have SSR/SSG is your choice and it won't have any bearing on final score;
- To use the local data file or not is your choice. Using the graphql endpoint will give you bonus points and not using won't incur in any penalties.