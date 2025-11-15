def build_graph(edges, directed=False):
    graph = {}

    for u, v in edges:
        if u not in graph:
            graph[u] = []
        graph[u].append(v)

        if directed:
            if v not in graph:
                graph[v] = []
        else:
            if v not in graph:
                graph[v] = []
            graph[v].append(u)

    return graph


def degree_dict(graph):
    deg = {}
    for node in graph:
        deg[node] = len(graph[node])
    return deg


if __name__ == "__main__":
    sample = [('PC1','SW1'), ('SW1','PR1'), ('PR1','PC2')]
    g = build_graph(sample, directed=False)
    print("Graph:", g)
    print("Degrees:", degree_dict(g))
