# JavaScript Groceries Solution

In this lab, you're going to write an interactive program that simulates you on the phone with your roommate. You forgot to bring your grocery list for the recipe you are cooking for dinner, so you've called your roommate to make sure you pick up the correct items.

The starter files already include an HTML file named groceries.html and in includes an external JavaScript file, scripts.js. You will write your script in the scripts.js file.

### Prompt for amounts
You are making a fruit salad, so you know you need different types of fruit, but you can't remember how many of each, so you're going to ask your roommate.

* how many pounds of apples?
* how many pounds pears?

### Calculate sub-total
Once you've collected these values through the prompt function, you need to calculate how much the fruit will cost altogether based on their cost per pound.  

* apples are $2.29/lb.
* pears are 2.99/lb.

### Add sales tax
Once you have the sub-total, you need to add the sales tax, which is 10%. This calculation will give you the total cost.(I know we don't charge sales tax on food in stores, but this is just an exercise).

### Confirm should purchase
Next, you need to use the confirm function to check with your roommate that it's ok to spend the total amount that you calculated. If he says ok, then use the alert function to say you bought everything and coming home. If he cancels, then user the alert function to say you put everything back and are coming home.

Here's a few requirements:

* use **const** variables whenever possible.
* write a function calculateTotalWithTax, that has two parameters, the total before taxes, and the tax rate, that returns the total, including with taxes included.
* the confirm message should contain the total cost.
  * the cost should be the nearest dollar amount, not including cents.
    * use the Math.floor function to round down.
  * use back-ticks, \`\`,  with the ${} syntax to build the string to pass to the confirm function that includes the total spent.

You can assume the user clicks the Ok button rather than Cancel when entering the number of pounds.

#### Pseudocode

```javascript 
lbsApples = Prompt for the number of lbs of apples
lbsPears = Prompt for the number of lbs of pears
subTotal = Calculate the cost of the fruit 
  (lbs of apples * cost/lb) +
  (lbs of pears * cost/lb)

total = subTotal + sales tax (10%)
confirm with roommate you should proceed with purchase
If (Ok) Then
  alert "I bought the fruit"
Else
  alert "I put the fruit back"
```

Here are the steps the user should see:

![](https://raw.githubusercontent.com/hoc-labs/images/main/conditionals-prompt1.png)

![](https://raw.githubusercontent.com/hoc-labs/images/main/conditionals-prompt2.png)

![](https://raw.githubusercontent.com/hoc-labs/images/main/conditionals-confirm1.png)

If the user clicks Ok

![](https://raw.githubusercontent.com/hoc-labs/images/main/conditionals-alert1.png)


If the user clicks Cancel

![](https://raw.githubusercontent.com/hoc-labs/images/main/conditionals-alert2.png)


