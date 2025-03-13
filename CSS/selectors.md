# CSS Selectors

## Table of Contents
- [Introduction](#introduction)
- [Basic Selectors](#basic-selectors)
- [Combinator Selectors](#combinator-selectors)
- [Pseudo-class Selectors](#pseudo-class-selectors)
- [Pseudo-element Selectors](#pseudo-element-selectors)
- [Attribute Selectors](#attribute-selectors)
- [Conclusion](#conclusion)

## Introduction
CSS selectors are used to select the HTML elements you want to style.

## Basic Selectors
- **Universal Selector (`*`)**: Selects all elements.
- **Type Selector (`element`)**: Selects all elements of a given type.
- **Class Selector (`.class`)**: Selects all elements with a given class.
- **ID Selector (`#id`)**: Selects a single element with a given ID.
- **Attribute Selector (`[attribute]`)**: Selects elements with a specific attribute.

## Combinator Selectors
- **Descendant Selector (`ancestor descendant`)**: Selects all descendants of a given element.
- **Child Selector (`parent > child`)**: Selects all direct children of a given element.
- **Adjacent Sibling Selector (`element + adjacent`)**: Selects the adjacent sibling of a given element.
- **General Sibling Selector (`element ~ siblings`)**: Selects all siblings of a given element.

## Pseudo-class Selectors
- **`:hover`**: Selects elements when you mouse over them.
- **`:focus`**: Selects elements when they are focused.
- **`:nth-child(n)`**: Selects the nth child of a parent element.

## Pseudo-element Selectors
- **`::before`**: Inserts content before an element's content.
- **`::after`**: Inserts content after an element's content.
- **`::first-line`**: Selects the first line of a block-level element.

## Attribute Selectors
- **`[attribute]`**: Selects elements with a specific attribute.
- **`[attribute=value]`**: Selects elements with a specific attribute value.
- **`[attribute~=value]`**: Selects elements with an attribute value containing a specified word.

## Conclusion
CSS selectors are a powerful tool for applying styles to specific elements in your HTML documents. Understanding and using them effectively can greatly enhance the presentation and usability of your web pages.
