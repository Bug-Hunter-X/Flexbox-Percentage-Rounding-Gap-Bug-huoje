# Flexbox Percentage Rounding Gap Bug

This repository demonstrates an uncommon CSS bug involving rounding issues with percentages within a flexbox layout.  The bug manifests as a small gap between nested elements, even when percentages are seemingly set to fill the parent container.

## Bug Description

The core issue stems from the way browsers handle percentage-based widths and heights.  Due to floating-point calculations, the sum of percentage values might not exactly equal 100%, resulting in slight rounding discrepancies. When combined with flexbox, these discrepancies can cause gaps between elements, particularly when `align-items` and `justify-content` are used to center content.

## Solution

The provided solution offers a simple fix that ensures proper element alignment and avoids gaps.