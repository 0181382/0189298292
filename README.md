Cloning with 5 retries
Initialized empty Git repository in /drone/src/.git/
+ git fetch origin +refs/heads/develop:
From https://github.com/boostorg/graph
 * branch              develop    -> FETCH_HEAD
 * [new branch]        develop    -> origin/develop
+ git checkout develop
Branch 'develop' set up to track remote branch 'develop' from 'origin'.
Switched to a new branch 'develop'
+ git fetch origin refs/pull/411/head:
From https://github.com/boostorg/graph
 * branch              refs/pull/411/head -> FETCH_HEAD
+ git merge 9ed5d902f2b793a449199a8fabd79353081c4064
Updating ce1daebc..9ed5d902
Fast-forward
 example/accum-compile-times.cpp                    |  8 ++-----
 example/actor_clustering.cpp                       | 20 +++++++----------
 example/adjacency_list.cpp                         |  6 ++---
 example/astar-cities.cpp                           | 16 ++++++-------
 example/astar_maze.cpp                             | 16 ++++++-------
 example/bellman-example.cpp                        | 11 ++++-----
 example/bfs-example2.cpp                           |  2 +-
 example/bfs-name-printer.cpp                       | 17 +++++++-------
 example/bfs.cpp                                    |  2 +-
 example/bfs_neighbor.cpp                           |  2 +-
 example/biconnected_components.cpp                 |  5 ++---
 example/boost_web_graph.cpp                        | 14 ++++++------
 example/boykov_kolmogorov-eg.cpp                   | 10 ++++-----
 example/bron_kerbosch_clique_number.cpp            |  2 +-
 example/bucket_sorter.cpp                          |  8 +++----
 example/canonical_ordering.cpp                     |  7 +++---
 example/cc-internet.cpp                            |  3 +--
 example/city_visitor.cpp                           |  2 +-
 example/clustering_coefficient.cpp                 |  2 +-
 example/connected-components.cpp                   |  2 +-
 example/connected_components.cpp                   |  2 +-
 example/copy-example.cpp                           |  2 +-
 example/cuthill_mckee_ordering.cpp                 | 18 ++++++---------
 example/cycle_canceling_example.cpp                |  2 +-
 example/cycle_ratio_example.cpp                    | 19 +++++++---------
 example/dag_shortest_paths.cpp                     |  5 ++---
 example/dave.cpp                                   |  3 +--
 example/dijkstra-example-listS.cpp                 | 21 +++++++----------
 example/dijkstra-example.cpp                       | 10 ++++-----
 example/dijkstra-no-color-map-example.cpp          |  8 +++----
 example/directed_graph.cpp                         |  4 ++--
 example/edge-connectivity.cpp                      | 26 ++++++++--------------
 example/edge-function.cpp                          |  4 ++--
 example/edge_basics.cpp                            | 12 +++++-----
 example/edge_connectivity.cpp                      |  3 +--
 example/edge_iterator_constructor.cpp              |  2 +-
 example/edge_property.cpp                          |  6 ++---
 example/edmonds-karp-eg.cpp                        |  8 +++----
 example/family_tree.cpp                            |  3 +--
 example/filtered-copy-example.cpp                  |  2 +-
 example/filtered_graph_edge_range.cpp              |  6 ++---
 example/gerdemann.cpp                              |  8 +++----
 example/girth.cpp                                  |  4 ++--
 example/graph-thingie.cpp                          | 10 ++++-----
 example/graph_as_tree.cpp                          |  5 ++---
 example/grid_graph_properties.cpp                  |  2 +-
 example/hawick_circuits.cpp                        |  5 +----
 example/implicit_graph.cpp                         |  2 +-
 example/influence_prestige.cpp                     |  2 +-
 example/interior_property_map.cpp                  |  2 +-
 example/iteration_macros.cpp                       |  3 +--
 example/johnson-eg.cpp                             |  2 +-
 example/kevin-bacon.cpp                            |  6 ++---
 example/kevin-bacon2.cpp                           |  2 +-
 example/king_ordering.cpp                          | 16 +++++--------
 example/kruskal-example.cpp                        |  8 +++----
 example/kruskal-telephone.cpp                      | 11 ++++-----
 example/kuratowski_subgraph.cpp                    |  2 +-
 example/last-mod-time.cpp                          |  5 ++---
 example/leda-graph-eg.cpp                          |  2 +-
 example/loops_dfs.cpp                              | 22 +++++++-----------
 example/make_biconnected_planar.cpp                |  2 +-
 example/make_maximal_planar.cpp                    |  2 +-
 example/matching_example.cpp                       |  6 ++---
 example/max_flow.cpp                               |  8 +++----
 example/mcgregor_subgraphs_example.cpp             |  6 ++---
 example/mean_geodesic.cpp                          |  2 +-
 example/miles_span.cpp                             |  6 ++---
 example/min_max_paths.cpp                          |  4 ++--
 example/minimum_degree_ordering.cpp                |  3 +--
 example/modify_graph.cpp                           |  3 +--
 example/neighbor_bfs.cpp                           |  6 ++---
 example/ordered_out_edges.cpp                      |  4 ++--
 example/ospf-example.cpp                           |  6 ++---
 example/planar_face_traversal.cpp                  |  2 +-
 example/prim-example.cpp                           |  7 +++---
 example/prim-telephone.cpp                         |  9 ++++----
 example/property-map-traits-eg.cpp                 |  2 +-
 example/property_iterator.cpp                      |  6 ++---
 example/push-relabel-eg.cpp                        | 13 +++++------
 example/quick-tour.cpp                             |  8 +++----
 example/quick_tour.cpp                             |  7 +++---
 example/reachable-loop-head.cpp                    | 11 +++------
 example/reachable-loop-tail.cpp                    |  3 +--
 example/read_graphviz.cpp                          |  8 +++----
 example/read_write_dimacs-eg.cpp                   | 12 +++++-----
 example/remove_edge_if_bidir.cpp                   |  4 ++--
 example/remove_edge_if_undir.cpp                   |  2 +-
 example/roget_components.cpp                       | 10 ++++-----
 example/scc.cpp                                    |  3 +--
 example/sloan_ordering.cpp                         | 11 ++++-----
 example/strong-components.cpp                      |  3 +--
 example/subgraph_properties.cpp                    |  6 ++---
 ...e_shortest_path_nonnegative_weights_example.cpp |  2 +-
 example/tiernan_print_cycles.cpp                   |  4 +---
 example/topo-sort-with-leda.cpp                    |  3 +--
 example/topo-sort-with-sgb.cpp                     |  3 +--
 example/topo-sort1.cpp                             |  3 +--
 example/topo-sort2.cpp                             |  3 +--
 example/topo_sort.cpp                              |  5 ++---
 example/transpose-example.cpp                      |  2 +-
 example/two_graphs_common_spanning_trees.cpp       |  3 +--
 example/undirected_adjacency_list.cpp              | 23 ++++++++-----------
 example/undirected_graph.cpp                       |  6 ++---
 example/vertex-name-property.cpp                   |  3 +--
 example/vertex_basics.cpp                          |  7 +++---
 example/vf2_sub_graph_iso_multi_example.cpp        | 11 ++-------
 107 files changed, 284 insertions(+), 419 deletions(-)
