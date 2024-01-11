---
layout: doc
title: Tag
category: Selection and input
examples:
  - fileName: Default.vue
    title: Default
    description: Use to signify the attributes of an object.
  - fileName: Removable.vue
    title: Removable
    description: Use to allow merchants to remove attributes from an object.
  - fileName: Clickable.vue
    title: Clickable
    description: Use to allow merchants to add attributes to an object.
  - fileName: Link.vue
    title: With link
    description: Use to allow merchants to navigate to a resource. For example a customer segment or a smart collection
  - fileName: CustomContent.vue
    title: With custom content
    description: Use when a tag needs to be visually distinguished from others, like when it's added automatically.
  - fileName: RemovableWithLink.vue
    title: Removable with link
    description: A removable attribute to an object that allows merchants to navigate to a resource.
---

# {{ $frontmatter.title }}

<Lede>

{{ $frontmatter.description }}

</Lede>

<Examples>

<<< ./[examples]

</Examples>

## Props

<div style="font-size: 0.8125rem">

Some types of props are following the [Polaris Design Tokens](https://polaris.shopify.com/tokens).

</div>

<PropsTable />

## Slots

<SlotsTable />

<div style="font-size: 0.8125rem">

## Best practices

Tags should:

- Be presented close to or within the input control that allows merchants to add and remove tags

---

## Related components

- To show the status of an object, [use the badge component](https://polaris.shopify.com/components/feedback-indicators/badge)
- To add and remove tags, [use the text field component](https://polaris.shopify.com/components/selection-and-input/text-field)

---

## Accessibility

### Labeling

The button to remove a tag is automatically given a label using `aria-label` so that screen reader users can distinguish which tag will be removed.

### Keyboard support

The control to remove a tag is implemented as a button with standard keyboard support.

- Give buttons keyboard focus with the <kbd>tab</kbd> key (or <kbd>shift</kbd> + <kbd>tab</kbd> when tabbing backwards)
- To activate a button, press the <kbd>enter</kbd>/<kbd>return</kbd> or <kbd>space</kbd> key

When a merchant uses the button to remove a tag, it is important to make sure that keyboard focus is managed. Moving focus to the next element in the page is recommended.

</div>