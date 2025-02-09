# Tailwind CSS @apply Directive Issue with Pseudo-Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to correctly apply styles when used with classes containing pseudo-selectors (e.g., `hover`, `focus`, `active`).

## Bug Description
The `@apply` directive doesn't seem to properly handle pseudo-selectors in the target classes. Styles defined within the class for these pseudo-selectors are not applied correctly when the associated state is activated.

## Reproduction Steps
1. Clone this repository.
2. Compile the CSS (if necessary).
3. Observe the affected element's behavior in a browser. The expected styles won't be applied on hover, focus or other interactions.

## Solution
The recommended solution is to apply the pseudo-selector styles directly in the main stylesheet or use JavaScript to handle interactions and apply the necessary classes dynamically.