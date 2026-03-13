# Breadth-first-search
Practice program 
graph = {
    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': [],
    'F': []
}
visited = []
queue = []
def bfs(node):
    visited.append(node)
    queue.append(node)
    while queue:
        s = queue.pop(0)
        print s,
        for i in graph[s]:
            if i not in visited:
               visited.append(i)             queue.append(i)
bfs('A')
OUTPUT:

A B C D E F
