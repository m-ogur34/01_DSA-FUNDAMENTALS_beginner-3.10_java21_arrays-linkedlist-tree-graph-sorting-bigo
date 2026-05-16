# 01 — DSA Fundamentals
**Zorluk:** Beginner (3/10) | **Java 21** | **Mülakat Hazırlığı**

Java ile temel veri yapıları ve algoritmaların sıfırdan implementasyonu. Her yapı için mülakatta çıkan klasik problemler ve Big O analizleri.

---

## İçerik

| Konu | Dosya | Kapsanan Problemler |
|------|-------|---------------------|
| **Arrays** | `arrays/ArrayProblems.java` | Two Sum, Max Subarray (Kadane), Sliding Window, Two Pointer, Prefix Sum, Merge Intervals, Trapping Rain Water |
| **Linked List** | `linkedlist/LinkedListImpl.java` | Reverse, Cycle Detection (Floyd), Middle Node, Kth From End, Merge Sorted Lists, Palindrome, Intersection |
| **Stack** | `stack/StackImpl.java` | Valid Parentheses, Min Stack, Infix→Postfix, Eval RPN, Daily Temperatures, Largest Rectangle |
| **Queue** | `queue/QueueImpl.java` | Circular Queue, Queue w/ Stacks, Level Order BFS, Sliding Window Max, Top K Frequent, Rotten Oranges |
| **Tree** | `tree/TreeImpl.java` | BST CRUD, Traversals, Max Depth, Balanced Check, LCA, Path Sum, Serialize/Deserialize, Kth Smallest |
| **Graph** | `graph/GraphImpl.java` | BFS, DFS, Cycle Detection, Topological Sort, Dijkstra, Number of Islands, Union-Find |
| **Sorting** | `sorting/SortingAlgorithms.java` | Bubble, Selection, Insertion, Merge, Quick, Heap, Counting, Binary Search, Rotated Array Search |
| **Dynamic Programming** | `dp/DynamicProgramming.java` | Fibonacci, Climbing Stairs, Coin Change, LCS, LIS, Knapsack, Edit Distance, House Robber |
| **Hashing** | `hashing/HashingProblems.java` | HashMap impl, Group Anagrams, Longest Consecutive, Subarray Sum K, LRU Cache |

---

## Big O Özeti

```
Veri Yapısı     | Erişim | Arama | Ekleme | Silme
----------------+--------+-------+--------+------
Array           | O(1)   | O(n)  | O(n)   | O(n)
Linked List     | O(n)   | O(n)  | O(1)*  | O(1)*
Stack/Queue     | O(n)   | O(n)  | O(1)   | O(1)
HashMap         | O(1)   | O(1)  | O(1)   | O(1)
BST (balanced)  | O(logn)| O(logn)| O(logn)| O(logn)
Heap            | O(1)** | O(n)  | O(logn)| O(logn)

* baş/son için
** min veya max için
```

```
Algoritma    | Best      | Average   | Worst     | Space
-------------+-----------+-----------+-----------+------
Bubble Sort  | O(n)      | O(n²)     | O(n²)     | O(1)
Merge Sort   | O(n logn) | O(n logn) | O(n logn) | O(n)
Quick Sort   | O(n logn) | O(n logn) | O(n²)     | O(logn)
Heap Sort    | O(n logn) | O(n logn) | O(n logn) | O(1)
Binary Search| O(1)      | O(logn)   | O(logn)   | O(1)
BFS/DFS      | O(V+E)    | O(V+E)    | O(V+E)    | O(V)
Dijkstra     | -         | O((V+E)logV)| -       | O(V)
```

---

## Mülakatta Sık Sorulan Sorular

### Arrays & Strings
- Two Sum neden HashMap ile O(n)'de çözülür?
- Sliding Window ne zaman kullanılır?
- Kadane algoritması ne yapar?

### Linked List
- Floyd's Cycle Detection nasıl çalışır?
- Linked List'i O(1) space ile nasıl ters çevirirsin?

### Stack & Queue
- Stack kullanarak Queue nasıl implemente edilir?
- Monotonic Stack nedir, hangi problemlerde kullanılır?

### Tree
- BFS vs DFS ne zaman hangisi tercih edilir?
- LCA (Lowest Common Ancestor) algoritması?
- BST inorder traversal neden sıralı dizi verir?

### Graph
- Topological Sort ne zaman kullanılır?
- Dijkstra negatif ağırlıklı edge'lerde çalışır mı?
- Union-Find'ın path compression'ı neden önemli?

### Dynamic Programming
- Memoization vs Tabulation farkı nedir?
- Bir problemi DP ile çözüp çözemeyeceğini nasıl anlarsın?
- 0/1 Knapsack ile Unbounded Knapsack farkı?

---

## Çalıştırma

```bash
mvn compile
mvn exec:java -Dexec.mainClass="com.dsa.arrays.ArrayProblems"
mvn exec:java -Dexec.mainClass="com.dsa.sorting.SortingAlgorithms"
mvn exec:java -Dexec.mainClass="com.dsa.dp.DynamicProgramming"
```

---

## Öğrenme Sırası

```
1. Arrays       → temel veri yapısı, tüm diğerlerinin temeli
2. Hashing      → O(1) arama, Two Sum ve benzeri problemler
3. Linked List  → pointer mantığı, recursive düşünme
4. Stack/Queue  → LIFO/FIFO, BFS/DFS hazırlığı
5. Tree         → recursive yapı, BST
6. Graph        → BFS, DFS, Dijkstra
7. Sorting      → algoritma karmaşıklığı
8. DP           → en zor kategori, en çok pratik gerektiren
```

---

**Sonraki Repo →** [02 - Bank Account Manager](../02_BANK-ACCOUNT-MANAGER) (Java OOP, Collections, Streams)
