# AI-Law-Minicourse-HW
## Supreme Court Topic Modeling
### Step 1
> In this step, requests for data is being run using Beautiful Soup, specifically, Supreme Court rulings from 1760 thorugh 2018 is being pulled directly from the CaseLaw website. The results are returned ins a data table which includes as columns, case url and docket. The search results in 23,393 cases. 
### Step 2
> In this step, the 23,393 opinions gathered from Step 1 are broken down into three smaller frames to prevent CaseLaw from blocking the request. The first contains the first 5,000 opinions, the second the next 10,000, and the final the remaining 8,268. Within each group, the case name is scraped and "pickled" (or saved). Once all three are scraped for the case names, they're then recompiled and saved as a whole project. 
### Step 3
> In this third step, the opinions are processed to remove stopwords and to lemmatize. Packages of common English stop words are imported using the sklearn.feature_extraction module and then additional stopwords are created by assigning categories of words, including names (male and female), case names, and state names. To lemmatize words, we define separators ("\r", "\n", and more). This is also applied to the stopwords list created. The resulting case list/information is then "pickled", or saved, for later use. 
### Step 4
> In this next step, we go through different methods for topic modeling the Supreme Court cases extracted in the previous steps to find the best model to use: 
>> 1. Latent Dirchlet Allocation Model;
>> 2. Latent Semantic Analysis; and
>> 3. NMF Model. 
### Step 5
> In this final step, we apply the third model, NMF Model, to the data frame.
## Tensor Flow 
### Step 1. 
Found and verified text8.zip
Data size 17005207
### Step 2.
Most common words (+UNK) [['UNK', 418391], ('the', 1061396), ('of', 593677), ('and', 416629), ('one', 411764)]
Sample data [5234, 3081, 12, 6, 195, 2, 3134, 46, 59, 156] ['anarchism', 'originated', 'as', 'a', 'term', 'of', 'abuse', 'first', 'used', 'against']
### Step 3.
3081 originated -> 12 as
3081 originated -> 5234 anarchism
12 as -> 3081 originated
12 as -> 6 a
6 a -> 12 as
6 a -> 195 term
195 term -> 2 of
195 term -> 6 a
### Step 4. 
WARNING:tensorflow:From <ipython-input-14-2cd9be819b02>:57: calling reduce_sum (from tensorflow.python.ops.math_ops) with keep_dims is deprecated and will be removed in a future version.
Instructions for updating:
keep_dims is deprecated, use keepdims instead
### Step 5. 
Initialized
Average loss at step  0 :  285.828887939
Nearest to with: lifeforms, childress, catalog, garp, belgians, peat, attacks, brainiac,
Nearest to years: yah, breakbeat, wakko, offsets, phoebe, westerners, accordion, requested,
Nearest to first: olomouc, moon, infringement, percentile, readily, eris, drawbacks, sacrum,
Nearest to but: lapsed, replicate, wines, kodak, skill, pulley, insiders, screenshots,
Nearest to will: paige, ethica, organum, reductase, hohner, morse, latter, sheen,
Nearest to is: leah, asymptotes, carnivore, sledge, motif, alexandrian, neoconservatism, wolfram,
Nearest to also: viridis, wollaston, serene, gimlin, bodied, lightsaber, isidore, alcoholism,
Nearest to many: youngster, anglophone, scone, kapoor, kiln, colossus, fanfiction, winnipeg,
Nearest to after: unclassified, sooty, md, missed, avm, banshee, boethius, evaporates,
Nearest to war: notorious, alliances, voltage, moustache, pauses, mordecai, disgusted, saa,
Nearest to in: enosis, gq, uruk, micronations, allowing, attribution, cert, firsthand,
Nearest to see: argento, portrayed, futhark, bluegrass, ubiquitous, disintegrated, obstructed, bloodless,
Nearest to people: marches, fogo, bearable, misdemeanors, pfeiffer, uber, unchanging, rdoba,
Nearest to time: shingles, verity, ecuadorean, plate, junit, freak, corticosteroids, archived,
Nearest to b: synapse, detract, detailing, escoffier, asserts, walkway, benefits, herakles,
Nearest to be: poseidon, provost, indiscriminate, organized, sahib, latvia, bahasa, barton,
Average loss at step  2000 :  112.440091161
Average loss at step  4000 :  53.2432478173
Average loss at step  6000 :  33.4743904212
Average loss at step  8000 :  23.2457017548
Average loss at step  10000 :  17.9553051608
Nearest to with: and, as, of, by, deke, for, belgians, in,
Nearest to years: gland, aberdeen, requested, semitism, diacritic, UNK, museum, five,
Nearest to first: agave, definitions, impure, secure, aid, UNK, abba, invasive,
Nearest to but: honor, lapsed, chicken, quality, aberdeen, skill, input, touring,
Nearest to will: latter, scandal, precautions, fear, examination, tackle, employment, required,
Nearest to is: was, by, aberdeen, in, and, are, indicates, ignored,
Nearest to also: es, alcoholism, unwanted, where, is, pinto, alcohols, initiative,
Nearest to many: aires, lovell, fanfiction, vs, aberdeen, winnipeg, plays, agave,
Nearest to after: agave, assumed, and, off, md, spider, extent, axis,
Nearest to war: notorious, alliances, covered, vowels, sports, voltage, town, july,
Nearest to in: and, of, as, for, coke, on, mosque, by,
Nearest to see: speer, portrayed, leo, special, scoring, agave, schemata, ubiquitous,
Nearest to people: aberdeen, kw, koestler, bear, sites, hakama, bckgr, rdoba,
Nearest to time: plate, hakama, aberdeen, atemi, encouraged, allah, greeted, total,
Nearest to b: detailing, aalborg, required, rogue, audiobook, asserts, initiatives, reason,
Nearest to be: seems, objective, wolverine, chaos, rogue, latvia, barton, conceding,
Average loss at step  12000 :  14.2075844798
Average loss at step  14000 :  11.751193164
Average loss at step  16000 :  10.0245820698
Average loss at step  18000 :  8.62468684524
Average loss at step  20000 :  8.09010765362
Nearest to with: for, and, by, in, of, as, deke, rig,
Nearest to years: dasyprocta, accordion, five, amazonas, gland, requested, mango, six,
Nearest to first: agave, impure, invasive, operatorname, secure, milan, definitions, archimedean,
Nearest to but: and, is, dye, chicken, if, honor, touring, circ,
Nearest to will: scandal, examination, precautions, subkey, fear, dasyprocta, targeting, latter,
Nearest to is: was, are, were, by, has, for, agouti, in,
Nearest to also: not, isidore, it, cartographer, unwanted, approval, where, lit,
Nearest to many: aires, dasyprocta, the, fleece, fanfiction, aberdeen, some, ranges,
Nearest to after: heterogeneous, and, assumed, agave, sooty, off, by, from,
Nearest to war: alliances, notorious, agouti, perceptual, covered, sports, vowels, voltage,
Nearest to in: and, of, on, for, from, at, by, nine,
Nearest to see: speer, portrayed, leo, dye, circ, special, scoring, ubiquitous,
Nearest to people: circ, dasyprocta, guards, aberdeen, illustrator, rdoba, napoleonic, bear,
Nearest to time: plate, dasyprocta, amazonas, hakama, encouraged, wattle, atemi, agouti,
Nearest to b: d, and, circ, detailing, aalborg, operatorname, initiatives, sweeps,
Nearest to be: by, have, is, seems, chaos, as, were, rogue,
Average loss at step  22000 :  7.10370227587
Average loss at step  24000 :  6.80994153327
Average loss at step  26000 :  6.81830236101
Average loss at step  28000 :  6.38070867467
Average loss at step  30000 :  5.95833082259
Nearest to with: amalthea, for, by, in, and, from, as, into,
Nearest to years: dasyprocta, accordion, requested, five, mango, amazonas, six, gland,
Nearest to first: agave, operatorname, invasive, adjusting, impure, disadvantages, utopian, abet,
Nearest to but: and, playoffs, circ, birkenau, pediment, dye, amalthea, dasyprocta,
Nearest to will: can, scandal, targeting, subkey, examination, could, fear, would,
Nearest to is: was, are, were, has, abet, agouti, for, as,
Nearest to also: not, it, abet, which, isidore, often, lit, alcoholism,
Nearest to many: some, aires, ranges, the, birkenau, fanfiction, dasyprocta, fleece,
Nearest to after: heterogeneous, from, by, seven, aaliyah, off, and, sooty,
Nearest to war: alliances, notorious, agouti, perceptual, covered, csa, amaranthus, sports,
Nearest to in: on, at, and, from, for, by, nine, abet,
Nearest to see: portrayed, speer, cappella, dye, leo, special, circ, scoring,
Nearest to people: circ, rdoba, dasyprocta, trinomial, guards, illustrator, poles, napoleonic,
Nearest to time: plate, dasyprocta, amazonas, encouraged, aediles, wattle, hakama, acquaintance,
Nearest to b: d, detailing, aalborg, circ, sweeps, initiatives, intentionally, one,
Nearest to be: by, have, were, is, as, seems, was, chaos,
Average loss at step  32000 :  5.93702329206
Average loss at step  34000 :  5.68958295739
Average loss at step  36000 :  5.72655980468
Average loss at step  38000 :  5.56046866465
Average loss at step  40000 :  5.25601143146
Nearest to with: amalthea, zero, for, and, by, in, from, of,
Nearest to years: dasyprocta, accordion, six, requested, gland, five, amazonas, abet,
Nearest to first: agave, operatorname, invasive, adjusting, impure, vma, disadvantages, circ,
Nearest to but: and, that, playoffs, circ, flamingo, methodology, pediment, birkenau,
Nearest to will: can, could, would, should, targeting, scandal, to, subkey,
Nearest to is: was, are, has, were, abet, zero, agouti, by,
Nearest to also: not, which, often, abet, it, now, isidore, that,
Nearest to many: some, these, ranges, aires, birkenau, both, dasyprocta, fanfiction,
Nearest to after: heterogeneous, from, by, seven, off, on, stitch, five,
Nearest to war: alliances, notorious, perceptual, pauses, agouti, csa, covered, gemini,
Nearest to in: on, at, and, from, zero, abet, of, dasyprocta,
Nearest to see: portrayed, speer, cappella, dye, zero, scoring, circ, nominal,
Nearest to people: circ, rdoba, guards, dasyprocta, trinomial, pgs, aberdeen, intellectualism,
Nearest to time: dasyprocta, plate, amazonas, encouraged, wattle, aediles, hakama, acquaintance,
Nearest to b: d, circ, zero, spilled, shipbuilding, detailing, aalborg, operatorname,
Nearest to be: have, by, were, was, make, seems, chaos, is,
Average loss at step  42000 :  5.37119328272
Average loss at step  44000 :  5.2434101907
Average loss at step  46000 :  5.26232920611
### Step 6.
