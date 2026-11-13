# Binary Search Tree (C#)

A generic BST (`BinarySearchTree<T> where T : IComparable<T>`) — left subtree < node < right subtree. Average O(log n) insert/search/delete (O(n) worst case if unbalanced).

## Usage

```csharp
var tree = new BinarySearchTree<int>();
tree.Insert(50);
tree.Insert(30);
tree.Insert(70);

bool found = tree.Contains(30); // true
tree.Delete(30);

foreach (var v in tree.InOrder()) // sorted output
    Console.Write($"{v} ");
```

## API

`Insert`, `Contains`, `Delete`, `Min`, `Max`, `InOrder`/`PreOrder`/`PostOrder`, `Count`, `Height`

## Build & Test

```bash
dotnet build
dotnet test
```
