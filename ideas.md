# Ideas

## Pushing a page

```dart
// TODO: kinda ugly ngl
yeet.addAndCommit(page);
```

## Pushing multiple pages

```dart
yeet.add(page1);
yeet.add(page2);
yeet.commit();
```

## Going to a URL

```dart
yeet.checkout('/the/URL');
```

## Creating a new URL

```dart
yeet.branch('/the/URL');
```

## Going back to the last checked out URL

```dart
yeet.checkout('-');
```

## Pushing a specific page from another position

```dart
yeet.cherryPick('/popup');
```

## Pushing several specific pages from another position

```dart
yeet.cherryPick('/path1', noCommit: true);
yeet.cherryPick('/path2', noCommit: true);
yeet.commit();
```

## Changing the location of a URL / Popping the page

```dart
// TODO
yeet.reset(...);
```

## Pushing the previous page on top again

```dart
// TODO
yeet.revert(...);
```

## Pushing all of the pages for a URL

```dart
yeet.checkout('/path/to/new')
yeet.rebase('/path/to/old');
```

## Initial structure

```dart
// TBD
// Similar to the current version of yeet
Yeet(
  path: '/...',
  children: [
    //...
  ]
)
```

## Not mentioned

```dart
yeet.back(); // going back in history
yeet.forward(); // going forward in history
yeet.pop(); // another way of saying the same thing
// more shortcuts and easier to understand verbs
// so non git enthusiasts can also use/enjoy it.

```