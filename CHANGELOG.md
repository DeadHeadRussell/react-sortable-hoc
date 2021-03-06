Changelog
------------
### 0.4.9
Fix: This release fixes a bug introduced in `0.4.8` caused by calling the `forEach` method directly on a NodeList, which is undefined in a number of browsers [#125](https://github.com/clauderic/react-sortable-hoc/issues/125)

### 0.4.8
Fix: Added logic to ensure that `select`, `input` and `textarea` fields in `SortableElement` always retain their `value` when the element is cloned (this happens when sorting begins) [#122](https://github.com/clauderic/react-sortable-hoc/issues/122) [#123](https://github.com/clauderic/react-sortable-hoc/pull/123). Thanks [@tomasztomys](https://github.com/tomasztomys)!

### 0.4.7
Fix: This release fixes a bug in Firefox caused by active anchor tags preventing mousemove events from being fired [#118](https://github.com/clauderic/react-sortable-hoc/issues/118)

### 0.4.5
Fix: getHelperDimensions height was not being used (Thanks [@SMenigat](https://github.com/SMenigat)!)

### 0.4.4
Tweak: cherry-picking lodash methods instead of importing the entire bundle (slipped by in a PR, thanks for pointing this out [@arackaf](https://github.com/arackaf)!)

### 0.4.3
Fixes an edge-case bug in Firefox where window.getComputedStyle() returns null inside an iframe with `display: none` [#106](https://github.com/clauderic/react-sortable-hoc/pull/106). Thanks [@funnel-mark](https://github.com/funnel-mark)!

### 0.4.2
Fixes an issue when attempting to sort items while rapidly moving the mouse. By setting an immediate timer, we move the cancel event to the tail of the timer queue, and ensure that it is fired after the pressTimer [#80](https://github.com/clauderic/react-sortable-hoc/pull/80). Thanks [@v0lkan](https://github.com/v0lkan)!

### 0.4.0
– Fix a timing issue in Chrome caused by setTimeout [#71](https://github.com/clauderic/react-sortable-hoc/pull/71)
– Private props are no longer passed down to the wrapped component [#98](https://github.com/clauderic/react-sortable-hoc/pull/98)

### 0.3.0
Added grid support for elements of equal widths / heights [#4](https://github.com/clauderic/react-sortable-hoc/issues/4) [#86](https://github.com/clauderic/react-sortable-hoc/pull/86). Huge shout-out to [@richmeij](https://github.com/richmeij) for making this happen!

### 0.2.0
Add a `getHelperDimensions` prop to control SortableHelper size [#83](https://github.com/clauderic/react-sortable-hoc/issues/83). Thanks [@nervetattoo](https://github.com/nervetattoo)!

### 0.1.1
Added `touchCancel` listener to properly handle canceled touches [#73](https://github.com/clauderic/react-sortable-hoc/pull/73)

### 0.1.0
- Force `box-sizing: border-box` on sortable helper [#67](https://github.com/clauderic/react-sortable-hoc/issues/67)
- Support changing an item's collection prop on the fly [#66](https://github.com/clauderic/react-sortable-hoc/pull/66)

### 0.0.11
Utilize babel-plugin-transform-runtime to utilize `babelHelpers` without them being required in application code [#45](https://github.com/clauderic/react-sortable-hoc/issues/45)

### 0.0.10
The `arrayMove` helper no longer mutates the array, it now returns a new array [#61](https://github.com/clauderic/react-sortable-hoc/issues/61)

### 0.0.9
Server-side rendering bugfix: safeguard against `document` being undefined [#59](https://github.com/clauderic/react-sortable-hoc/pull/59)

### 0.0.8
- Added `distance` prop ([#35](https://github.com/clauderic/react-sortable-hoc/issues/35))
- Added a `shouldCancelStart` ([#47](https://github.com/clauderic/react-sortable-hoc/issues/47), [#36](https://github.com/clauderic/react-sortable-hoc/issues/36), [#41](https://github.com/clauderic/react-sortable-hoc/issues/41)) prop to programatically cancel sorting before it begins.
- Prevent right click from causing sort start ([#46](https://github.com/clauderic/react-sortable-hoc/issues/46))

### 0.0.7
Fixes server-side rendering (window undefined) ([#39](https://github.com/clauderic/react-sortable-hoc/issues/39))

### 0.0.6
- Added support for a custom container ([#37](https://github.com/clauderic/react-sortable-hoc/issues/37))
- Fix changing disable property while receiving props ([#34](https://github.com/clauderic/react-sortable-hoc/issues/34))
