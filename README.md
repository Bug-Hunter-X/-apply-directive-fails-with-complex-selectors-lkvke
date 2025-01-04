# Tailwind CSS @apply Directive Bug with Complex Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to apply styles correctly when used with complex selectors, such as pseudo-classes or sibling selectors. The issue can lead to unexpected visual inconsistencies in your application.

## Bug Description

The `@apply` directive, when applied to classes with complex selectors (e.g., `hover:bg-gray-200`), does not always apply the styles as expected, especially when those classes are nested or combined with other selectors.

## Reproduction

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe the behavior: The hover effect might not be applied correctly.

## Solution

The solution is to avoid using `@apply` directly with complex selectors. Instead, use a more straightforward approach by applying the classes without the `@apply` directive. Refer to `bugSolution.html` for a working solution.  The solution shows how to directly include the desired class names or to use a different approach to achieve the same visual effect.