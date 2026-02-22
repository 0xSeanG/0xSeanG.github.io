---
layout: page
title: All Recipes
permalink: /recipes/
---

<ul class="recipe-list">
  {% assign all_recipes = site.recipes | sort: "title" %}
  {% for recipe in all_recipes %}
    <li>
      <a href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.title }}</a>
      <span class="recipe-category-inline">{{ recipe.category_label }}</span>
    </li>
  {% endfor %}
</ul>
