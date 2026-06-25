# UICollectionView Compositional Layout Demo

UIKit sample app demonstrating compositional collection-view layouts with reusable layout builders, section configuration, and a simple supplementary header view.

## What This Project Shows

- `UICollectionViewCompositionalLayout` setup.
- Reusable layout creation helpers in `Layout+Extension.swift`.
- Section/header composition with `SimpleHeaderView`.
- UIKit collection-view registration helpers.
- Storyboard-based application shell with programmatic collection-view behavior.

## Main Modules

| Path | Responsibility |
| --- | --- |
| `CompositeLayout/CompositeLayout/Components/ViewController.swift` | Main collection-view screen |
| `CompositeLayout/CompositeLayout/Components/Layout+Extension.swift` | Compositional layout helpers |
| `CompositeLayout/CompositeLayout/Components/SimpleHeaderView.swift` | Supplementary header |
| `CompositeLayout/CompositeLayout/Components/ViewController+Extension.swift` | Controller helpers |
| `CompositeLayout/CompositeLayout/Util.swift` | Demo data/constants |

## Running

```sh
open CompositeLayout/CompositeLayout.xcodeproj
```

Select the `CompositeLayout` scheme and run on an iOS simulator.

## Technical Notes

- The repo is intentionally small: it isolates collection-view layout composition without introducing networking or persistence.
- The useful extension point is adding multiple section builders and data-driven layout selection.
- For production code, keep layout factories pure and test them through deterministic section configuration.
