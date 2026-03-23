[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Service](README.md) > Food and Drink

# Food and Drink

<img src="../../assets/raptor_idle_south.png" width="96" align="right">

Station food service covers cooking, bartending, and vending operations. This article documents the hunger and fullness system, all cooking appliances and their recipes, drink production, condiment synthesis, and vending machine contents.

---

## Quick Reference

| Topic | Summary | Notable |
|---|---|---|
| [Hunger and Fullness](#hunger-and-fullness) | Nutrition bar drains over time | Starvation slows movement |
| [Microwave](#microwave) | Broadest recipe set; most dishes start here | Requires heat only |
| [Oven](#oven) | Breads, pies, pizzas, cakes | Requires oven appliance |
| [Grill](#grill) | Burgers, steaks, omelettes, toasts | Requires grill appliance |
| [Deep Fryer](#deep-fryer) | Fries, donuts, battered items | Requires fryer appliance |
| [Intermediate Ingredients](#intermediate-ingredients) | Dough, meatball, batter -- made by reagent reaction | Required for most recipes |
| [Condiments](#condiments) | Produced by grinding produce or mixing reagents | Applied to finished food |
| [Bar Spirits](#bar-spirits) | Pre-bottled spirits for the bartender | 100u per bottle |
| [Hot Drinks](#hot-drinks) | Coffee and tea; require heated water | Coffee machine or beaker with heat |
| [Mixed Drinks -- Alcoholic](#mixed-drinks----alcoholic) | Combined reagents produce cocktails | Shaker holds 60u |
| [Mixed Drinks -- Non-Alcoholic](#mixed-drinks----non-alcoholic) | Juice blends, sodas, milkshakes | No strength value |
| [Vending Machines](#vending-machines) | Getmore Chocolate Corp; no chef required | Credits required |

---

## Hunger and Fullness

Every crew member maintains a nutrition bar that depletes over time through activity. The bar has four visible states:

| State | Effect |
|---|---|
| Green (fed) | No penalties |
| Yellow (hungry) | Mild discomfort; no mechanical penalty |
| Dark red (starving) | Significant movement speed reduction; malnourished appearance |
| Black (overfed) | Movement penalty; description notes the crew member appears chubby |

Nutrition is released slowly after eating. A meal that does not immediately register fullness will continue providing nutrition over the following minutes.

The primary nutrition reagent is **nutriment**, present in most cooked food. Secondary contributors include animal protein, corn oil, ketchup, sugar, and some alcoholic drinks. Eating past the full threshold does not provide additional benefit and will push the meter toward overfed.

Starvation accelerates under several conditions: vomiting, exposure to cold environments, cryo recovery, blood loss recovery, and Lipozine intake. Some diseases also increase hunger drain rate.

---

## Intermediate Ingredients

Most recipes require pre-prepared ingredients that are not available off the shelf and must be synthesized from reagents. These reactions occur automatically when the required reagents are combined in a container or on a surface.

| Ingredient | Required Reagents | Catalysts | Notes |
|---|---|---|---|
| **Dough** | 10u flour + 3u egg | None | Inhibited by water, beer, or sugar in the mix |
| **Flat dough** | Dough + rolling pin | None | Produces 3 dough slices when cut |
| **Dough slice** | Flat dough cut with knife | None | Further sliceable into spaghetti |
| **Raw meatball** | Reagent reaction (see below) | None | Cooked in microwave to produce meatball |
| **Meatball** (from reagents) | 3u protein + 5u flour | 5u enzyme | Spawns 3 meatballs per reaction |
| **Raw cutlet** | Butchered meat | None | Cooked in microwave to produce cutlet |
| **Batter** | 10u flour + 3u egg + 5u water + 2u salt | None | Used in fryer recipes |
| **Beer batter** | 10u flour + 3u egg + 5u beer + 2u salt | None | Fryer coating variant |
| **Cake batter** | 15u flour + 10u milk + 15u sugar + 3u egg | None | 60u produced per reaction |
| **Brownie mix** | 5u flour + 5u cocoa powder + 5u sugar | None | 15u produced |
| **Cheesewheel** | 40u milk | 5u enzyme | Sliced into cheese wedges |
| **Tofu** | 10u soy milk | 5u enzyme | Used in many vegetarian dishes |
| **Chocolate bar** | 2u milk (or soy milk) + 2u cocoa + 2u sugar | 5u enzyme | Used in cakes and cookies |
| **Butter** | 20u cream + 1u salt | None | Used in pastries and cooking |
| **Soy sauce** | 4u soy milk + 1u sulphuric acid | None | |
| **Ketchup** | 2u tomato juice + 1u water + 1u sugar | None | 4u produced |
| **Mayo** | 9u egg + 5u cooking oil + 5u lemon juice + 1u salt | None | 15u produced |
| **Peanut butter** | 2u peanut oil + 1u sugar + 1u salt | 5u enzyme | 3u produced |
| **Bun** | Dough + microwave/oven with 1u salt | None | Produces 3 buns |
| **Sausage** | Meatball + raw cutlet + microwave | None | Produces 2 sausages |
| **Stuffing** | Bread + 5u water + 1u salt + 1u pepper | None | |

Egg as a reagent is obtained by breaking eggs into a beaker. Flour is obtained by grinding wheat. Sugar is obtained by grinding sugar cane or from the chemical dispenser. Milk and cream are available pre-bottled. Enzyme is obtained from a condiment bottle of enzyme, available in the kitchen.

---

## Cooking Appliances

The kitchen contains four main cooking appliances. Each accepts ingredients placed inside and produces a finished dish.

**Microwave** is the standard appliance and handles the broadest range of recipes. Most meals can be prepared in the microwave alone. Cooking time is short.

**Oven** is required for baked goods: breads, pies, pizzas, cakes, and croissants. The oven can also cook many microwave recipes as an alternative appliance.

**Grill** is required for burgers, steaks, and grilled items. Some dishes require the grill specifically and cannot be made in the microwave.

**Deep Fryer** is required for fries, donuts, battered meats, and similar fried foods. The fryer uses cooking oil and requires the oil to reach operating temperature.

A **grinder** (blender) in the kitchen processes produce and food items into liquid reagents. These reagents can be transferred to a **CondiMaster** unit to produce condiment bottles. The grinder also has a juicing setting for extracting juice from fruit.

---

## Microwave

<details>
<summary>Eggs and Breakfast</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Fried egg | 1 egg | | 1u salt, 1u pepper |
| Boiled egg | 1 egg | | 5u water |
| Devilled eggs | 2 eggs | 1 chili | 2u salt, 5u mayo |
| Poached egg | 1 egg | | 5u water, 1u space spice, 1u salt, 1u pepper |
| Bacon (from raw) | 1 raw bacon | | |
| Bacon and eggs | 1 bacon, 1 fried egg | | |
| Bacon stick | 1 bacon, 1 boiled egg | | |
| Egg pancake | 3 meatballs | | 6u egg |
| Hatchling surprise | 1 poached egg, 3 bacon | | |
| Father's breakfast | 1 sausage, 1 meatsteak | | 6u egg |
| Riztizkzi sea | 3 eggs | | 15u blood |
| NT muffin | 1 biscuit, 1 sausage, 1 fried egg, 1 cheese wedge | | |
| Red sun special | 1 sausage, 1 cheese wedge | | |
| Eggs benedict | 1 cutlet, 1 fried egg, 1 bread | | |
| Chawanmushi | | 1 mushroom | 5u water, 5u soy sauce, 6u egg |
| Egg bowl | | | 5u water, 10u rice, 3u egg |
| Gigapuddi | 2 eggs | | 15u milk |
| Happy pudding | 2 eggs | | 15u milk, 5u sugar |
| Muffin x2 | 1 dough | | 5u milk, 5u sugar |

</details>

<details>
<summary>Burgers, Sandwiches, and Wraps</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Sandwich | 1 meatsteak, 2 bread, 1 cheese wedge | | |
| Peanut butter and jelly | 2 bread | | 5u cherry jelly, 5u peanut butter |
| Club sandwich | 2 bread, 1 chicken, 1 bacon, 1 cheese wedge | 1 tomato, 1 lettuce | 5u mayo |
| BLT | 2 bread, 2 bacon | 1 tomato, 1 lettuce | |
| Doner kebab | 1 meatsteak, 1 flat dough | 1 tomato, 1 cabbage | 1u salt |
| Fish taco | 1 carp meat, 1 tortilla | 1 chili, 1 lemon | |
| Taco | 1 tortilla, 1 cutlet, 1 cheese wedge | | |
| Breakfast wrap | 1 bacon, 1 tortilla, 1 cheese wedge, 1 egg | | |
| Slime toast | 1 bread | | 5u slime jelly |
| Cherry toast | 1 bread | | 5u cherry jelly |
| Donk pocket | 1 dough, 1 meatball | | |

</details>

<details>
<summary>Soups and Stews</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Meatball soup | 1 meatball | 1 carrot, 1 potato | 10u water |
| Vegetable soup | | 1 carrot, 1 potato, 1 corn, 1 eggplant | 10u water |
| Nettle soup | | 1 nettle, 1 potato | 10u water, 3u egg |
| Tomato soup | | 2 tomatoes | 10u water |
| Wish soup | | | 20u water |
| Stew | 1 meat | 1 potato, 1 tomato, 1 carrot, 1 eggplant, 1 mushroom | 10u water |
| Bear stew | 1 bear meat | 1 potato, 1 tomato, 1 carrot, 1 eggplant, 1 mushroom | 10u water |
| Onion soup | | 1 onion | 10u water |
| Mushroom soup | | 1 mushroom | 5u water, 5u milk |
| Beet soup | | 1 white beet, 1 cabbage | 10u water |
| Miso soup | 2 soy dope, 2 tofu | | 10u water |
| Stewed soy meat | 2 soy dope | 1 carrot, 1 tomato | |
| Blood soup | | | 30u blood |
| Slime soup | | | 10u water, 5u slime jelly |
| Boiled slime core | 1 slime extract | | 5u water |
| Mystery soup | 1 bad recipe, 1 tofu, 1 cheese wedge | | 10u water, 3u egg |
| Hot and sour soup | 1 tofu | 1 cabbage, 1 mushroom | 2u salt, 2u pepper, 10u water |
| Chicken noodle soup | 1 spaghetti, 1 raw cutlet | 1 carrot | 10u water |

</details>

<details>
<summary>Rice, Pasta, and Grains</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Boiled spaghetti | 1 spaghetti | | 5u water |
| Boiled rice | | | 5u water, 10u rice |
| Rice pudding | | | 5u milk, 10u rice |
| Pasta tomato | 1 spaghetti | 2 tomatoes | 5u water |
| Meatball spaghetti | 1 spaghetti, 2 meatballs | | 5u water |
| Spesslaw | 1 spaghetti, 4 meatballs | | 5u water |
| Fried rice | | 1 carrot, 1 cabbage | 5u water, 10u rice, 5u soy sauce |
| Lo mein | 1 spaghetti | 1 carrot, 1 cabbage | 5u water, 5u soy sauce |
| Pork bowl | 1 cutlet | | 5u water, 10u rice |
| Egg bowl | | | 5u water, 10u rice, 3u egg |
| Omurice | | | 5u rice, 5u ketchup, 3u egg |
| Risotto | | 1 mushroom | 5u red wine, 10u rice, 1u space spice |
| Curry rice | | 1 chili | 10u rice |
| Red curry | 2 cutlets | | 5u cream, 2u space spice, 5u rice |
| Green curry | 2 tofu | 1 chili | 5u cream, 2u space spice, 5u rice |
| Yellow curry | | 2 peanut, 1 potato | 5u cream, 2u space spice, 5u rice |
| Bibimbap | 1 egg, 1 cutlet | 1 carrot, 1 cabbage, 1 mushroom | 5u rice, 2u space spice |
| Kudzu donburi | 1 carp meat | 1 kudzu | 10u rice |
| Sushi (from meat) | 3 meat | 1 cabbage | 20u rice |
| Sushi (from carp) | 3 carp meat | 1 cabbage | 20u rice |
| Kitsune udon | 1 spaghetti, 1 tofu | | 3u egg |
| Goulash | 1 cutlet, 1 spaghetti | 1 tomato | |
| Makaroni | 1 grub meat, 1 egg, 2 cheese wedge | | 15u flour, 5u milk |
| Boiled plump helmet biscuit x2 | | 1 plump helmet | 5u water, 5u flour |

</details>

<details>
<summary>Tortillas and Mexican Food</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Tortilla x3 | 1 flat dough | | 5u flour, 5u water |
| Chip plate | 1 tortilla | | 1u salt |
| Cuban nachos | 1 tortilla | 1 chili | 5u ketchup |
| Nachos | 1 chip plate, 1 cheese wedge | | |
| Burrito | 1 tortilla, 2 meatballs | | 1u space spice |
| Vegan burrito | 1 tortilla, 1 tofu | | |
| Cheese burrito | 1 tortilla, 2 meatballs, 1 cheese wedge | | |
| Meat burrito | 1 tortilla, 2 cutlets | 1 soybean | |
| Cheese and spicy burrito | 1 tortilla, 2 cheese wedge | 2 chili, 1 soybean | |
| Hell burrito | 1 tortilla, 2 meatballs | 1 soybean, 10 chili | 1u space spice |
| Fajita/fuego burrito | 1 tortilla | 1 soybean, 2 chili | |
| Breakfast wrap | 1 bacon, 1 tortilla, 1 cheese wedge, 1 egg | | |
| Salsa | | 1 chili, 1 tomato, 1 lime | 1u space spice, 1u pepper, 1u salt |
| Guacamole | 1 tofu | 1 chili, 1 lime | 1u space spice, 1u pepper, 1u salt |
| Cheese dip | 1 cheese wedge | 1 chili, 1 tomato | 1u space spice, 1u pepper, 1u salt |
| Pig in a blanket | 1 dough slice, 1 sausage | | |

</details>

<details>
<summary>Salads and Sides</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Tossed salad | | 2 lettuce, 1 tomato, 1 carrot, 1 apple | |
| Fruit salad | | 1 orange, 1 apple, 1 grapes, 1 watermelon | |
| Flower child salad | 1 roasted sunflower | 1 harebells, 1 poppies | |
| Rose salad | 1 roasted sunflower | 1 harebells, 1 rose | |
| Aesir salad | | 1 gold apple, 1 ambrosia deus | |
| Valid salad | 1 meatball | 1 potato, 3 ambrosia | |
| Tossedsalad | | 2 lettuce, 1 tomato, 1 carrot, 1 apple | |
| Mashed potato | 1 spreads | 1 potato | |
| Beans on toast | | 2 soybean | 5u ketchup |
| Stuffing x2 | 1 bread | | 5u water, 1u salt, 1u pepper |
| Roasted sunflower x2 | 1 raw sunflower | | 1u salt, 1u cooking oil |
| Roasted peanuts x2 | | 2 peanut | 2u salt, 1u cooking oil |
| Fries (microwave) | 1 raw sticks | | |
| Chili cheese fries | 1 fries, 1 cheese wedge, 1 hot chili | | |
| Fish and chips | 1 fries, 1 carp meat | | |
| Sashimi | 1 carp meat | | 5u soy sauce |
| Candied apple | | 1 apple | 5u water, 5u sugar |
| Caramel apple | | 1 apple | 5u milk, 5u sugar |
| Popcorn | | 1 corn | |
| Fortune cookie | 1 dough slice, 1 paper | | 5u sugar |
| Mint | | | 5u sugar, 5u frost oil |
| Sugar cookie x4 | 1 dough | | 5u sugar, 3u egg |

</details>

<details>
<summary>Meat Dishes</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Meatsteak (syntiflesh) | 1 syntiflesh | | 1u salt, 1u pepper |
| Hot chili | 1 meat | 1 chili, 1 tomato | |
| Cold chili | 1 meat | 1 ice chili, 1 tomato | |
| Bear chili | 1 bear meat | 1 chili, 1 tomato | |
| Roast beef | 1 meat | 2 carrot, 2 potato | |
| Rib plate | 1 meat | | 5u honey, 2u space spice, 1u pepper |
| Wing fang chu | 1 xeno meat | | 5u soy sauce |
| Eggroll | 1 fried egg | 1 cabbage | 10u soy sauce |
| Stuffed meatball x2 | 1 meatball, 1 cheese wedge | 1 cabbage | |
| Tamales | 3 dough slices, 1 meat | 1 corn | |
| Tocino | 1 raw cutlet | | 5u salt, 5u red wine |
| Bigos | 1 sauerkraut, 1 sausage | 1 onion | 5u flour, 5u water |

</details>

<details>
<summary>Sweets and Desserts</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Rofflewaffles x2 | 2 dough | | 5u psilocybin, 10u sugar |
| Spacylibertyduff | | | 5u water, 5u vodka, 5u psilocybin |
| Amanita jelly | | | 5u water, 5u vodka, 5u amatoxin |
| Chocolate egg | 1 egg, 1 chocolate bar | | |
| Ice cream sandwich | 1 ice cream | | 5u milk, 5u ice |
| Dank pocket | 1 meatball, 1 dough slice | 2 ambrosia | |
| Butterscotch x2 | 1 butter | | 10u sugar, 5u cream |
| Hot butter ice cream | 1 butter | | 5u ice, 5u cream |
| Reishi cup | 1 chocolate bar | | 3u psilocybin, 3u sugar |
| Berry clafoutis | 1 flat dough | 1 berries | |
| Honey candy | | | 5u sugar, 5u nutriment |

</details>

---

## Oven

<details>
<summary>Breads and Flatbreads</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Bread | 2 dough | | 1u salt, 5u yeast |
| Baguette | 2 dough | | 1u salt, 1u pepper, 5u yeast |
| Flatbread | 1 flat dough | | |
| Tortilla x3 | 1 flat dough | | 5u flour |
| Tofubread | 2 dough, 2 tofu, 2 cheese wedge | | |
| Cream cheese bread | 2 dough, 2 cheese wedge | | |
| Meatbread | 2 dough, 2 meat, 2 cheese wedge | | |
| Xeno meatbread | 2 dough, 2 xeno meat, 2 cheese wedge | | |
| Banana bread | 2 dough | 1 banana | 5u milk, 15u sugar |
| Bun x3 | 1 dough | | 1u salt |
| Cracker | 1 dough slice | | 1u salt |
| Poppy pretzel x2 | 1 dough | 1 poppies | |
| Croissant x2 | 1 dough | | 1u salt, 5u water, 5u milk, 5u yeast |
| Cinnamon roll | 1 dough, 1 butter | | 5u cinnamon, 10u sugar |
| Honey bun x4 | 1 dough | | 5u milk, 3u egg, 5u honey |
| Meatbun x2 | 1 meatball, 1 flat dough | 1 cabbage | 5u water |
| Spiced meatbun x2 | 1 dough slice, 1 raw cutlet | | 2u space spice, 5u water |
| Custard bun | 1 dough slice | | 1u space spice, 5u water, 3u egg |
| Chicken momo x2 | 3 dough slices, 1 chicken | | 2u space spice, 5u water |
| Veggie momo x2 | 3 dough slices | 1 carrot, 1 cabbage | 2u space spice, 5u water |

</details>

<details>
<summary>Pies and Tarts</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Meat pie | 1 flat dough, 1 meat | | |
| Tofu pie | 1 flat dough, 1 tofu | | |
| Apple pie | 1 flat dough | 1 apple | |
| Cherry pie | 1 flat dough | 1 cherry | 10u sugar |
| Banana pie | 1 flat dough | 1 banana | 5u sugar |
| Pumpkin pie | 1 flat dough | 1 pumpkin | 5u sugar |
| Plump helmet pie | 1 flat dough | 1 plump helmet | |
| Key lime pie | | 2 lime | 5u milk, 5u sugar, 3u egg, 10u flour |
| Amanita pie | 1 flat dough | | 5u amatoxin |
| Apple tart x2 | 1 flat dough | 1 gold apple | 10u sugar |
| Quiche | 1 cheese wedge | | 5u milk, 9u egg, 10u flour |
| Bacon flatbread | 1 flat dough, 1 cheese wedge, 4 bacon | 2 tomatoes | |
| Meat pocket x2 | 1 flat dough, 1 meatball, 1 cheese wedge | | |
| Buttspie | 1 butterscotch, 1 flat dough | | 10u cinnamon |
| Enchiladas | 1 cutlet, 1 tortilla | 2 chili | |

</details>

<details>
<summary>Pizzas</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Margherita | 1 flat dough, 4 cheese wedge | 1 tomato | |
| Meat pizza | 1 flat dough, 3 meat, 1 cheese wedge | 1 tomato | |
| Mushroom pizza | 1 flat dough, 1 cheese wedge | 5 mushroom, 1 tomato | |
| Vegetable pizza | 1 flat dough, 1 cheese wedge | 1 eggplant, 1 carrot, 1 corn, 1 tomato | |
| Pineapple pizza | 1 flat dough, 1 cheese wedge, 2 pineapple rings | 1 tomato | |
| Mac and cheese | 1 spaghetti, 1 cheese wedge | | 5u milk |
| Lasagna | 2 flat dough, 2 cutlets | 2 tomatoes, 1 eggplant | |
| Waffles x2 | 2 dough | | 10u sugar |
| Pancakes x2 | 2 flat dough | | 5u milk, 15u sugar |
| Berry pancakes x2 | 2 flat dough | 2 berries | 5u milk, 15u sugar |

</details>

<details>
<summary>Cakes and Pastries</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Plain cake | | | 30u cake batter, 2u vanilla |
| Carrot cake | | 3 carrot | 30u cake batter |
| Chocolate cake | | | 30u cake batter, 5u cocoa |
| Cheesecake | 2 cheese wedge | | 30u cake batter |
| Peanut cake | | 1 peanut | 30u cake batter, 5u peanut butter |
| Orange cake | | 2 orange | 30u cake batter |
| Lime cake | | 2 lime | 30u cake batter |
| Lemon cake | | 2 lemon | 30u cake batter |
| Apple cake | | 2 apple | 30u cake batter |
| Birthday cake | 1 cake hat | | 30u cake batter |
| Brain cake | 1 brain | | 30u cake batter |
| Brownies | | | 10u brownie mix, 3u egg |
| Cosmic brownies | | 1 ambrosia | 10u brownie mix, 3u egg |
| Yule log (Buche de Noel) | | 2 berries | 20u cake batter, 10u cream, 5u cocoa |
| Jaffa cake x6 | | 1 orange | 15u cake batter, 10u cocoa |
| Cinnamon bun x4 | 1 dough | | 15u sugar, 10u cream |
| Truffle x4 | 1 chocolate bar | | 5u sugar, 5u cream |
| Cookie x4 | 1 dough, 1 chocolate bar | | 10u milk, 10u sugar |
| Blondies | | | 10u blondie mix, 3u egg |
| Suppermatter | 1 cheesecake | | 5u radium, 5u milk |
| Exciting suppermatter | 1 cheesecake | | 5u radium, 5u space spice |

</details>

<details>
<summary>Other Oven Dishes</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Oven fries | 1 raw sticks | | |
| Loaded baked potato | 1 cheese wedge | 1 potato | |
| Turkey | 1 chicken (or raw turkey), 1 stuffing | 1 potato (raw turkey only) | 1u salt, 1u pepper |
| Tofurkey | 2 tofu, 1 stuffing | | 1u salt, 1u pepper |
| Zest fish | 1 carp meat | 1 lemon (or lime) | 3u salt |
| Rib plate | 1 meat | | 5u honey, 2u space spice, 1u pepper |
| Monkey's delight | 1 monkey cube | 1 banana | 1u salt, 1u pepper, 10u flour |
| Diona roast | 1 diona | 1 apple | 5u pacid |
| Bacon x6 | 6 raw bacon, 1 spreads | | |
| Spicy boys x6 | | | 5u cinnamon, 10u sugar, 10u corn oil |
| Scorpion (cooked) | 1 scorpion | | 1u salt |

</details>

---

## Grill

<details>
<summary>Burgers</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Monkey burger | 1 bun, 1 meat | | |
| Xeno burger | 1 bun, 1 xeno meat | | |
| Fish burger | 1 bun, 1 carp meat | | |
| Tofu burger | 1 bun, 1 tofu | | |
| Hotdog | 1 bun, 1 sausage | | |
| Bear burger | 1 bun, 1 bear meat | | |
| Bacon cheeseburger | 1 bun, 1 meat, 2 bacon | | |
| Slime burger | 1 bun | | 5u slime jelly |
| Cherry burger | 1 bun | | 5u cherry jelly |
| Big bite burger | 1 monkey burger, 3 meat | | 3u egg |
| Super bite burger | 1 big bite burger, 1 dough, 1 meat, 1 cheese wedge, 1 boiled egg | 1 tomato | 5u salt, 5u pepper |
| Chicken fillet | 1 chicken katsu, 1 bun | | |

</details>

<details>
<summary>Kabobs and Other Grill</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Monkey kabob | 2 metal rods, 2 meat | | |
| Tofu kabob | 2 metal rods, 2 tofu | | |
| Meatsteak | 1 meat | | 1u salt, 1u pepper |
| Omelette | 2 cheese wedge | | 6u egg |
| Omurice heart | | | 5u rice, 5u ketchup, 5u sugar, 3u egg |
| Honey toast | 1 bread | | 5u honey |
| Grilled cheese | 2 bread, 1 cheese wedge | | |
| Toasted sandwich | 1 sandwich | | |
| Cheese toast x4 | 1 butter, 1 bread, 1 cheese wedge | | 1u space spice |
| Grilled carp | 6 carp meat | 1 lettuce, 1 lime | 1u space spice |
| Bacon (from spreads) | 1 spreads, 1 raw bacon | | |

</details>

---

## Deep Fryer

<details>
<summary>Fryer Recipes</summary>

| Dish | Items | Fruits/Plants | Reagents |
|---|---|---|---|
| Fries | 1 raw sticks | | |
| Cheesy fries | 1 fries, 1 cheese wedge | | |
| Jalapeno poppers x2 | | 1 chili | |
| Onion rings x2 | | 1 onion | |
| Cuban carp | 1 dough, 1 carp meat | 1 chili | |
| Battered sausage | 1 sausage | | |
| Chicken katsu | 1 chicken | | |
| Fried pizza | 1 pizza | | |
| Fried mushroom | | 1 plump helmet | |
| Fish fingers | 1 carp meat | | |
| Corn dog | 1 sausage | 1 corn | |
| Sweet and sour | 1 bacon, 1 cutlet | | 5u soy sauce, 10u batter |
| Risotto balls x2 | 1 risotto | | 1u salt, 1u pepper |
| Frostbelle fritter x2 | 1 frostbelle | | 5u sugar |
| Jelly donut x2 | 1 dough slice | | 5u berry juice, 5u sugar |
| Churro | 1 dough slice | | |
| Plain donut x2 | 1 dough slice | | 5u sugar |
| Chaos donut x2 | 1 dough slice | | 10u frost oil, 10u capsaicin, 10u sugar |
| Funnel cake x2 | | | 5u sugar, 10u batter |
| Pisang goreng | | 2 banana | 2u capsaicin, 2u sugar, 10u batter |
| Wings | | | 5u capsaicin, 10u batter |
| General's chicken | 2 meat | | 2u capsaicin, 2u sugar, 10u batter |

</details>

---

## Condiments

Condiments are reagents applied directly to finished food. They can increase nutrition value, add flavor effects, or introduce additional chemical properties to food. A piece of food holds a maximum of 50 units of reagents total.

Condiments are produced in two ways. The **grinder** (blender) processes fresh produce into liquid form -- juicing tomatoes produces tomato juice, grinding plump helmets produces nutriment and protein. The resulting liquid is then transferred to the **CondiMaster** in the kitchen storage room, which bottles it into a condiment container. The blender also has a separate juicing mode for extracting juice from fruit.

The following condiments can be applied to food after cooking:

| Condiment | Source |
|---|---|
| Ketchup | 2u tomato juice + 1u water + 1u sugar |
| Soy sauce | 4u soy milk + 1u sulphuric acid |
| Mayonnaise | 9u egg + 5u cooking oil + 5u lemon juice + 1u salt |
| Peanut butter | 2u peanut oil + 1u sugar + 1u salt (enzyme catalyst) |
| Cherry jelly | Available pre-bottled; also from cherry juice |
| Slime jelly | From slime extracts |
| Hot sauce | Capsaicin extract; from chili grinding |
| Cold sauce | Frost oil; from ice chili |
| Barbecue sauce | 2u tomato juice + 1u apple juice + 1u sugar + 1u space spice |
| Butter | Applied from butter item |
| Honey | Applied from honey reagent |
| Salt and pepper | Available from dispensers in kitchen |

Some chefs mix Dylovene into food that contains mildly toxic ingredients to neutralize the poison before serving.

---

## Drinks

### Bar Spirits

The bar stockroom contains the following pre-bottled spirits. Each bottle holds 100 units.

| Bottle | Contents |
|---|---|
| Griffeater Gin | Gin |
| Uncle Git's Special Reserve | Whiskey |
| Special Blend | Special whiskey (lower toxicity variant) |
| Tunguska Triple Distilled | Vodka |
| Caccavo Tequilla | Tequila |
| Captain Pete's Cuban Spiced Rum | Rum |
| Goldeneye Vermouth | Vermouth |
| Robert Robust's Coffee Liqueur | Kahlua |
| College Girl Goldschlager | Goldschlager |
| Chateau De Baton Cognac | Cognac |
| Jailbreaker Verte | Absinthe |
| Emeraldine Melon Liqueur | Melon liqueur |
| Miss Blue Curacao | Blue curacao |
| Dr. Bone's Peppermint Schnapps | Peppermint schnapps |
| Dr. Bone's Peach Schnapps | Peach schnapps |
| Dr. Bone's Lemonade Schnapps | Lemonade schnapps |
| Schusskonig | Jager |
| Doublebeard Bearded Special Red | Red wine |
| Doublebeard Bearded Special White | White wine |
| NanoTrasen Carnoth Red | Carnoth red wine |
| Gilthari Luxury Champagne | Champagne |
| Mono-No-Aware Luxury Sake | Sake |
| Unathi Liquor | Unathi liquor |
| Flask of Holy Water | Holy water |
| Wrapp Artiste Patron | Patron (pre-mixed) |
| Briar Rose Grenadine Syrup | Grenadine |

Canned and bottled beers and sodas are also available behind the bar: Spacer Beer, Silver Dragon Pilsner, Meteor Beer, Lite-Speed Lite Beer, Crisp's Cider, Magm-Ale, Hushed Whisper IPA. Sodas: Space Cola, Space Cola Free, Space-Up, Space Mountain Wind, Dr. Gibb.

Some spirits can be synthesized from produce rather than ordered:

| Spirit | Recipe |
|---|---|
| Beer | 5u corn oil + 5u flour (inhibited by flour in grain mixes; use enzyme) |
| Vodka | 10u potato juice |
| Red wine | 10u grape juice |
| Cider | 10u apple juice |
| Sake | 10u rice |
| Moonshine | 10u nutriment |
| Mead | 1u sugar + 1u water |

---

### Hot Drinks

Hot drinks require water heated above 100°C combined with the appropriate reagent. A coffee machine or heated beaker produces the reaction.

| Drink | Recipe |
|---|---|
| Coffee | 5u hot water + 1u coffee powder |
| Black tea | 5u hot water + 1u tea powder |
| Decaf tea | 5u hot water + 1u decaf tea powder |
| Hot chocolate | 5u hot water + 1u cocoa powder |
| Drip coffee | Separate drip coffee machine |
| Iced coffee | 2u coffee + 1u ice |
| Iced tea | 2u tea + 1u ice |
| Mint tea | 5u tea + 1u mint |
| Lemon tea | 5u tea + 1u lemon juice |
| Lime tea | 5u tea + 1u lime juice |
| Orange tea | 5u tea + 1u orange juice |
| Berry tea | 5u tea + 1u berry juice |
| Green tea | 5u tea + 1u green tea reagent |
| Chai tea | 5u tea + 1u chai spice |
| Soy latte | 1u coffee + 1u soy milk |
| Cafe latte | 1u flat white + 1u milk |
| Long black | 1u water + 1u coffee |
| Americano | 1u water + 2u long black |
| Macchiato | 1u milk + 2u coffee |
| Cortado | 3u macchiato + 1u milk foam |
| Breve | 4u cortado + 1u cream |
| Cappuccino | 4u cortado + 1u milk + 1u milk foam |
| Flat white | 2u milk + 1u drip coffee |
| Mocha | 5u breve + 2u hot chocolate + 1u milk + 1u cream + 1u milk foam |
| Vienna | 1u coffee + 2u cream |

---

### Mixed Drinks -- Non-Alcoholic

<details>
<summary>Non-Alcoholic Cocktails and Sodas</summary>

| Drink | Recipe |
|---|---|
| Lemonade | 1u lemon juice + 1u sugar + 1u water |
| Melonade | 1u watermelon juice + 1u sugar + 1u soda water |
| Appleade | 1u apple juice + 1u sugar + 1u soda water |
| Pineappleade | 2u pineapple juice + 1u lime juice + 2u soda water + 1u honey |
| Kira Special | 1u orange juice + 1u lime juice + 1u soda water |
| Brown Star | 2u orange juice + 1u cola |
| Shirley Temple | 4u ginger ale + 1u grenadine |
| Roy Rogers | 5u Shirley Temple + 2u lemon-lime soda |
| Arnold Palmer | 1u iced tea + 1u lemonade |
| Collins Mix | 3u lemon-lime soda + 1u soda water |
| Driver's Punch | 2u appleade + 1u orange juice + 1u mint + 1u soda water |
| Mint Apple Sparkle | 2u appleade + 1u mint |
| Berry Cordial | 4u berry juice + 1u sugar + 1u lemon juice |
| Tropical Fizz | 6u soda water + 1u berry juice + 1u mint + 1u lime juice + 1u lemon juice + 1u pineapple juice |
| Melon Spritzer | 2u watermelon juice + 2u red wine + 1u apple juice + 1u lime juice |
| Faux Fizz | 2u soda water + 1u berry juice + 1u apple juice + 1u lime juice + 1u honey |
| Grape soda | 2u grape juice + 1u cola |
| Nuclear Cola | 1u uranium + 5u cola |
| Bilk | 1u milk + 1u beer |
| Milkshake | 1u cream + 2u ice + 2u milk |
| Chocolate milkshake | 1u milkshake + 1u cocoa |
| Berry milkshake | 1u milkshake + 1u berry juice |
| Coffee milkshake | 1u milkshake + 1u coffee |
| Peanut butter milkshake | 1u cream + 1u ice + 2u peanut butter + 1u milk |
| Eggnog | 5u milk + 5u cream + 5u sugar + 3u egg |
| Choc milk | 3u milk + 1u cocoa |
| Protein shake | 5u water + 1u protein powder |
| Virgin mojito | 3u soda water + 1u lime juice + 1u mint + 1u sugar |
| Virgin sex on the beach | 3u orange juice + 2u grenadine |
| Dream Cream | 2u milk + 1u cream + 1u honey |

</details>

---

### Mixed Drinks -- Alcoholic

Alcohol strength values determine intoxication rate. Lower numbers produce faster intoxication. Skrell are subject to a universal strength penalty and reach intoxication states faster than other species regardless of the listed value.

<details>
<summary>Light Drinks (Strength 5--12)</summary>

| Drink | Recipe | Strength |
|---|---|---|
| Special blend whiskey | (pre-bottled) | 7 |
| Bilk | 1u milk + 1u beer | ~8 |
| Mead | 1u sugar + 1u water | 12 |
| Irish cream | 2u whiskey + 1u cream | 12 |
| Long Island iced tea | 1u vodka + 1u gin + 1u tequila + 3u rum and cola | 12 |
| Sake bomb | 2u beer + 1u sake | 12 |
| Gin and tonic | 2u gin + 1u tonic | 15 |
| Rum and cola | 2u rum + 1u cola | 15 |
| Demons' Blood | 3u rum + 1u Space Mountain Wind + 1u blood + 1u Dr. Gibb | 15 |
| Devil's Kiss | 1u blood + 1u kahlua + 1u rum | 15 |
| Erika Surprise | 2u ale + 1u lime juice + 1u whiskey + 1u banana juice + 1u ice | 15 |
| Goldschlager | 10u vodka + 1u gold | 15 |
| Irish coffee | 1u Irish cream + 1u coffee | 15 |
| Manhattan | 2u whiskey + 1u vermouth | 15 |
| Patron | 10u tequila + 1u silver | 15 |
| Red mead | 1u blood + 1u mead | 15 |
| Sbiten | 10u vodka + 1u capsaicin | 15 |
| Screwdriver | 2u vodka + 1u orange juice | 12 |
| Whiskey soda | 2u whiskey + 1u soda water | 7 |
| Bilk | 1u milk + 1u beer | ~8 |

</details>

<details>
<summary>Medium Drinks (Strength 15--25)</summary>

| Drink | Recipe | Strength |
|---|---|---|
| Brave Bull | 2u tequila + 1u kahlua | 10 |
| Changeling Sting | 1u screwdriver + 1u lime juice + 1u lemon juice | 12 |
| Classic Martini | 2u gin + 1u vermouth | 25 |
| Cuba Libre | 3u rum and cola + 1u lime juice | 30 |
| Daiquiri | 3u rum + 2u lime juice + 1u sugar | 30 |
| Gargle Blaster | 2u vodka + 1u gin + 1u whiskey + 1u cognac + 1u lime juice | 50 |
| Gin Fizz | 1u gin + 1u soda water + 1u lime juice | 30 |
| Hippie's Delight | 1u psilocybin + 1u Gargle Blaster | 15 |
| Iced beer | 10u beer + 1u frost oil | 15 |
| Irish Car Bomb | 1u ale + 1u Irish cream | 15 |
| Irish cream | 2u whiskey + 1u cream | 12 |
| Long Island iced tea | 1u vodka + 1u gin + 1u tequila + 3u rum and cola | 12 |
| Margarita | 2u tequila + 1u lime juice | 15 |
| Mint Julep | 2u whiskey + 1u water + 1u mint | 25 |
| Mojito | 3u rum + 1u lime juice + 1u mint | 20 |
| Negroni | 1u gin + 1u bitters + 1u vermouth | 30 |
| Old Fashioned | 3u whiskey + 1u bitters + 1u sugar | 25 |
| Paloma | 1u soda water + 2u Tequila Sunrise | 20 |
| Pisco Sour | 1u wine brandy + 1u lemon juice + 1u sugar | 30 |
| Sake bomb | 2u beer + 1u sake | 12 |
| Sex on the Beach | 5u virgin sex on the beach + 1u vodka | 15 |
| Tequila Sunrise | 2u tequila + 1u orange juice | 10 |
| Vesper | 3u gin + 1u vodka + 1u red wine | 20 |
| Whiskey cola | 2u whiskey + 1u cola | 15 |
| Whiskey sour | 2u whiskey + 1u lemon juice + 1u sugar | 20 |
| White Russian | 2u Black Russian + 1u cream | 25 |
| Windgarita | 3u margarita + 2u Space Mountain Wind + 1u melon liqueur | 30 |

</details>

<details>
<summary>Strong Drinks (Strength 30+)</summary>

| Drink | Recipe | Strength |
|---|---|---|
| Clover Club | 1u berry juice + 1u lemon juice + 3u gin | 30 |
| Cold Front | 1u iced coffee + 1u whiskey + 1u mint | 25 |
| Grog | 1u rum + 1u water | 100 |
| Hooch | (synthesized) | 50 |
| Manhattan Project | 10u Manhattan + 1u uranium | 25 |
| Neurotoxin | (special synthesis) | 30 |
| Phoron Special | 2u rum + 2u vermouth + 2u phoron | 12 |
| Red Mead | 1u blood + 1u mead | 15 |
| Singulo | 5u vodka + 1u radium + 5u red wine | 30 |
| Snowwhite | 1u pineapple juice + 1u rum + 1u lemon-lime + 1u egg + 1u kahlua + 1u sugar | 100 |
| Syndicate Bomb | 1u beer + 1u whiskey cola | 25 |
| Three Mile Island | 10u Long Island iced tea + 1u uranium | 10 |
| Tokyo Rose | 1u sake + 1u berry juice | 35 |

</details>

<details>
<summary>Specialty and Station Drinks</summary>

| Drink | Recipe | Notes |
|---|---|---|
| Amasec | 1u iron + 5u red wine + 5u vodka | Station staple |
| Acid Spit | 1u sulphuric acid + 5u red wine | Toxic |
| Atomic Bomb | 10u B-52 + 1u uranium | Very strong |
| B-52 | 1u Irish cream + 1u kahlua + 1u cognac | |
| Beepsky Smash | 1u lime juice + 1u whiskey + 1u iron | |
| Doctor's Delight | 1u lime juice + 1u tomato juice + 1u orange juice + 2u cream + 1u tricordrazine | Healing drink |
| Goldschlager | 10u vodka + 1u gold | |
| God's Sake | 2u sake + 1u holy water | |
| Holy Mary | 2u vodka + 3u holy wine + 1u lime juice | |
| Ichor Mead | 1u holy wine + 1u mead | |
| Milk foam | (from steam wand with milk) | Used in coffee drinks |
| Morning After | 1u sbiten + 5u coffee | Very high caffeine |
| Nuclear Waste | 2u oil slick + 1u uranium | Radioactive |
| Rewriter | 1u Space Mountain Wind + 1u coffee | Caffeine + stimulant |
| Rotgut | 3u vodka + 1u rum + 1u whiskey + 3u cola | Very rough |
| Screaming Viking | 2u martini + 2u vodka tonic + 1u lime juice + 1u rum | |
| Tamagozake | 10u sake + 5u sugar + 3u egg | |
| Vox Delight | 3u phoron + 1u fuel + 1u water | Toxic to non-Vox |
| Wine Brandy | 10u red wine distilled to 5u | Requires distilling |

</details>

---

## Vending Machines

The **Getmore Chocolate Corp** machine is stocked in crew lounges and near the kitchen. It operates without a chef and dispenses pre-packaged snacks for credits. Standard stock includes:

| Item | Notes |
|---|---|
| Candy bar | |
| Gummy candy | |
| Dry ramen | Requires hot water to prepare; add hot water to produce hot ramen |
| Chips (plain, BBQ, Salt & Vinegar) | |
| Cheesie Honkers | |
| Pistachios | |
| Semki (sunflower seeds) | |
| Space jerky | |
| Packaged burger | Pre-cooked |
| Packaged hot dog | Pre-cooked |
| Packaged burrito | Pre-cooked |
| Raisin bread | |
| Space Twinkie | |
| Tasty bread | |
| Skrell snacks | |
| Cookie snack | |
| Tuna can | |
| Gum (box) | |
| Lollipop | |

Contraband items are not listed in standard stock but may be accessible through other means.

---

*See also: [Chemical Synthesizer Operations](../Medical/Chemistry.md), [Supply Manifest](../Cargo/SupplyManifest.md)*
