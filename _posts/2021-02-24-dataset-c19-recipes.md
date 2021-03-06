---
layout: post
title: "A Dataset of Nineteenth-Century American Recipes"
author: akblankenship
permalink: /2021/02/24/c19-recipes/
---

<https://github.com/ViralTexts/nineteenth-century-recipes/>

Previous experiments through the _Viral Texts_ project have focused on specific genres of nineteenth-century newspaper reprinting, such as fiction, vignettes, news, etc. Thus far, the project has yet to focus on one of the most prolific genres of text in the nineteenth century: the recipe. For many people operating out of and within the domestic sphere in the nineteenth century, recipe writing and cookbooks more broadly were some of the only ways in which they could access print media and disseminate their ideas and authority to a broader audience. The newspaper was one way in which recipes circulated in the nineteenth century, though even within a seemingly clear-cut genre and form such as the recipe, there were still many writers using the recipe form in order to expand the genre to include humor writing, medicine, and even cosmetic products. 

In order to apply the _Viral Texts_ methodology of reprint detection to recipes and recipe-like texts, we are using machine learning methods of classification to locate recipes in our newspaper data. First, however, I had to develop a training set of texts that I already identify as recipes, so that the classifier could then use this data to locate similar recipes, or recipe-like texts, in unknown textual data like the millions of newspaper reprints in our database. 

This dataset is currently a work in progress, though in its current version it includes 1,000+ recipes. As I obtain more recipes in plain text format, I plan to continue adding to this dataset—hopefully to also include the recipes I locate in the newspaper once we train the machine learning model. I also welcome any submissions of interesting recipes to this dataset. 

My next steps for this project are to develop a classifier using this training dataset. My starting point has been nineteenth-century American recipes in printed recipe books, though I hope to also expand this set to include community cookbooks developed by church groups or for charities, as well as recipe-like texts, such as joke recipes. If anyone uses this data for their own work, I would love to hear more about the work that you are doing and ways I can focus my own efforts. 

## Why recipes?

My own research focuses on recipes and recipe circulation and customization in nineteenth-century America. Recipes could take on many different purposes, and even social issues, in the nineteenth century. From medicine to discussing domestic discord, recipes would be taken up and disseminated for a multitude of reasons, though in many ways they represent a world of print culture within themselves. By attending to the texts of the domestic sphere, not only can conversations surrounding the proliferation of print in the nineteenth century be expanded to include the millions of recipes that were produced in this period, but by taking food seriously, we can also track changes in resource availability, the availability of technology, as well as systems of domestic labor. 

While many recipe books have been digitized and are available through websites such as HathiTrust or Project Gutenberg, I found it difficult to locate a dataset were recipes are treated as singular objects, detangled from the broader books which could include recipes for all types of things—including cleaning products rather than food. In order to address the need to study recipes as objects circulating within a broader network of print media, I decided to take the printed books and separate the recipes into their own plain text files so that they could more easily be traced through out periodicals as well as to use these individual recipes to find others of a similar type. 

As I’ve been developing this dataset, I has occurred to me that others might be interested in similar lines of inquiry or in other research related to recipes and consumption in nineteenth-century America, so in the spirit of open access, I am sharing this dataset, though it continues to be built upon and modified. In doing so, my hope is that the kinds of incredible analysis Digital Humanists are already doing can expand to include recipe writing. 

## How are the files organized?

To begin assembling training data, I pulled all of the nineteenth-century American recipe books available in plain-text format from Project Gutenberg. Since defining what makes a recipe book “American,” exactly, can be tricky, I decided to use books published in America in the nineteenth century, though some of these books may be centered around a particular kind of cuisine, like French cuisine. Then, going through each book by hand, I separated each recipe into its own text file. Each text file was named with the ID in Gutenberg followed by the title (or in some cases the shortened title) of each recipe. This way, if I were, say, only interested in recipes about cakes or recipes with pork the central ingredient, this would be possible by only searching through the titles as opposed to reading the entire text of the recipe. 

Additionally, since many recipe books in the nineteenth century also feature recipes specifically aimed towards people with illnesses,or for medicinal uses, I indicated when this was the case by adding “illness” to the end of the filename for recipes aimed at feeding people with illness and “medicine” to the end of any filename where the recipe is providing some sort of cure for an ailment. By marking these recipes as distinct from the rest of the set, those interested in only looking at medicinal recipes or recipes for feeding people with illnesses could filter for those recipes specifically, or remove them if only typical, food-related recipes were of interest. 

## Suggested dataset citation:

Blankenship, Avery. “A Dataset of Nineteenth-Century American Recipes,” _Viral Texts: Mapping Networks of Reprinting in 19th-Century Newspapers and Magazines_. 2021. <https://github.com/ViralTexts/nineteenth-century-recipes/>
