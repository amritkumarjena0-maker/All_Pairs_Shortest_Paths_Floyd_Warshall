<<<<<<< HEAD
# All-Pairs Shortest Paths Using Floyd–Warshall

## Aim

To implement the Floyd–Warshall algorithm in C to find the shortest paths between all pairs of vertices in a weighted graph.

## Folder Name

`All_Pairs_Shortest_Paths_Floyd_Warshall`

## File Name

`floyd_warshall.c`

## Description

The Floyd–Warshall algorithm is a dynamic programming algorithm used to find the shortest distances between every pair of vertices in a graph.

It works with positive and negative edge weights but does not support negative-weight cycles.

## Algorithm

1. Start.
2. Read the number of vertices `n`.
3. Read the adjacency matrix of the graph.
4. Select each vertex `k` as an intermediate vertex.
5. Check every pair of vertices `i` and `j`.
6. If the path through vertex `k` is shorter, update the distance using the formula.
7. Repeat the process for all intermediate vertices.
8. Display the final shortest-path matrix.
9. Stop.

## Flowchart

```text
          +-----------+
          |   START   |
          +-----------+
                |
                v
    +-----------------------+
    | Input number of       |
    | vertices and matrix   |
    +-----------------------+
                |
                v
    +-----------------------+
    | Select intermediate k |
    +-----------------------+
                |
                v
    +-----------------------+
    | Check each pair i, j  |
    +-----------------------+
                |
                v
    +-----------------------+
    | Is path through k     |
    | shorter?              |
    +-----------------------+
          /          \
        Yes           No
         |             |
         v             |
    +----------------+ |
    | Update dist[i] | |
    | [j]            | |
    +----------------+ |
         |             |
         +------+------+
                |
                v
    +-----------------------+
    | Repeat for all k, i, j|
    +-----------------------+
                |
                v
    +-----------------------+
    | Display shortest-path |
    | matrix                |
    +-----------------------+
                |
                v
          +-----------+
          |   STOP    |
          +-----------+
```

## Formula

`dist[i][j] = min(dist[i][j], dist[i][k] + dist[k][j])`

Here:
- `dist[i][j]` is the current distance from vertex `i` to vertex `j`.
- `dist[i][k]` is the distance from vertex `i` to vertex `k`.
- `dist[k][j]` is the distance from vertex `k` to vertex `j`.

## Sample Input

```text
4
0 5 99999 10
99999 0 3 99999
99999 99999 0 1
99999 99999 99999 0
```

Here, `99999` represents the absence of a direct edge.

## Sample Output

```text
0       5       8       9
INF     0       3       4
INF     INF     0       1
INF     INF     INF     0
```

## Complexity Analysis

- **Time Complexity:** O(V³)
- **Space Complexity:** O(V²)

Here, `V` represents the number of vertices.

## Technologies Used

- Programming Language: C
- Algorithm: Floyd–Warshall
- Subject: Design and Analysis of Algorithms (DAA)

## Result

The Floyd–Warshall algorithm successfully calculates the shortest distances between all pairs of vertices in a weighted graph.

## Author

BCA Student
=======
# All_Pairs_Shortest_Paths_Floyd_Warshall
>>>>>>> 3e9a0c243d0f1341dd1df5df0e2bb68e40fbc3ef
