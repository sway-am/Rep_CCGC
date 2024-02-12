# -Re-CCGC
# How to run the experiments
### For experiment 1:
1.Set runtime to T4 GPU.<br>
2.Clone this repo in your google collab notebook.<br>
3.Install the required libraries(munkres and torch_geometric).<br>
4.Navigate into the CCGC_MLRC directory.<br>
5.run the train.py file with the necessary arguments as per each dataset (refer to GRID_SEARCH_NORMAL.ipynb). <br>
(NOTE) : Please make  necessary changes of path in utils.py load_graph_data() function. used for loading the dataset.
### For experiment 2:
#### SCGC Loss + RNS
1.Set runtime to T4 GPU.<br>
2.Clone this repo in your google collab notebook.<br>
3.Install the required libraries(munkres and torch_geometric).<br>
4.Navigate into the CCGC_MLRC directory.<br>
5.Run the train_SCGC_with_RNS_train.py file with necessary arguments for each dataset(refer to train_SCGC_with_RNS.py).<br>
#### RNS only
1.Set runtime to T4 GPU.<br>
2.Clone this repo in your google collab notebook.<br>
3.Install the required libraries(munkres and torch_geometric).<br>
4.Navigate into the CCGC_MLRC directory.<br>
5.Run the train_only_rns.py file with necessary arguments for each dataset(refer to CCGC_ONLY_RNS.py).
#### Add  edges
1.Set runtime to T4 GPU.<br>
2.Clone this repo in your google collab notebook.<br>
3.Install the required libraries(munkres and torch_geometric).<br>
4.Navigate into the CCGC_MLRC directory.<br>
5.Uncomment the add_edges section in utils.py load_graph_data() function.
6.Run the train.py with necessary arguments for each dataset.(refer to AddandDropedges.ipynb)<br> 
#### Drop edges
1.Set runtime to T4 GPU.<br>
2.Clone this repo in your google collab notebook.<br>
3.Install the required libraries(munkres and torch_geometric).<br>
4.Navigate into the CCGC_MLRC directory.<br>
5.Uncomment the drop_edges section in utils.py load_graph_data() function.<br>
6.Run the train.py with necessary arguments for each dataset.(refer to Drop_edges.ipynb)<br> 
#### Diffusion
1.Set runtime to T4 GPU.<br>
2.Clone this repo in your google collab notebook.<br>
3.Install the required libraries(munkres and torch_geometric).<br>
4.Navigate into the CCGC_MLRC directory.<br>
5.Uncomment the diffusion section in utils.py load_graph_data() function.<br>
6.Run the train.py with necessary arguments for each dataset.(refer to Diffusion(1).ipynb)<br>
#### Mask features
1.Set runtime to T4 GPU.<br>
2.Clone this repo in your google collab notebook.<br>
3.Install the required libraries(munkres and torch_geometric).<br>
4.Navigate into the CCGC_MLRC directory.<br>
5.Uncomment the feat_mask section (last 2 lines) in utils.py load_graph_data() function.<br>
6.Run the train.py with necessary arguments for each dataset.(refer to Drop_edges.ipynb(as it contains mask features run as well)<br>
### For extension
#### Extension on Graph Datasets
1.Set runtime to T4 GPU.<br>
2.Clone this repo in your google collab notebook.<br>
3.Install the required libraries(munkres and torch_geometric).<br>
4.Navigate into the CCGC_MLRC directory.<br>
5.Run the train.py with necessary arguments for each dataset(refer Graph_Extension(1).ipynb).
#### Extension on Non Graph 
1.Set runtime to T4 GPU.<br>
2.Clone this repo in your google collab notebook.<br>
3.Install the required libraries(munkres and torch_geometric).<br>
4.Navigate into the CCGC_MLRC directory.<br>
5.Remove feature smoothening in train.py.<br>
6.Introduce PCA commented in load_graph_data() function utils.py.<br>
7.Run the train.py with necessary args (refer REUT.ipynb and usps_grid.ipynb).<br>





