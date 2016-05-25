Financial Optimization Platform
-------------------------------------------

##Problem Statement##
Using vis.js to visualize the financial data



##General Approach##
• Use data in data.js and transfer all information into two main objects
  • graphNodes, graphEdges
• Compute total values in each node and


##Why Vis.js but not D3.js?##
D3.js is....
1. Complicated scripts
2. Force driven transitions need to be built
3. Heavyweight code

Vis.js is...
1. Simple scripts, same functionality
2. Force driven transitions pre-built
3. Lightweight code that takes up less lines

##data.js##
• data_nodes: 	contains nodeId, name of node and position of node
• data_edges: contains edgeId and connected nodes
• data_instruments: contains each instrument and their prices
• data_edge_positions: contains instruments transferred on edge
  • edgeId, instrumentId and quantity
• data_node_positions: contains instruments contained in each node
  • nodeId, instrumentId and quantity
• data_edge_cost: cost of transferring instruments across an edge


##Converting data nodes to network##
• Graph contains nodes that have weighted values on them
• One of the primitive characteristics of a neural network
• Has capability of estimating non-linear outputs
• Could possibly treat the internal structures as the hidden layers of the ANN
• Therefore, use inputs as amount of investable assets that one can use
• Output as the maximum, optimal path of investment
