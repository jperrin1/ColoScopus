# ColoScopus 1.3.1

ColoScopus is a free graphical bibliography tool. Literature review is done in the form of 2D graphs, in a similar fashion to research rabbit (https://www.researchrabbit.ai/) or connected papers (https://www.connectedpapers.com/). ColoScopus is desktop based, and searches can be saved locally. Data is retrieved from Scopus, without any filtering, offering you a complete overview over your field of interest.

## Getting started

### Access to Scopus API
ColoScopus relies on data provided by the Scopus API. **An access to Scopus and an API key are therefore necessary**.
To create a Scopus API key, head to https://dev.elsevier.com/, click on "My API Key" and log in. 

![alt text](<markdown images/Scopus dev portal.PNG>)

Create an API key and copy it. You will need it to start ColoScopus.

![alt text](<markdown images/Scopus dev portal api key created.PNG>)


### Launching ColoScopus

To download ColoScopus, click on the latest release on the Github page. Extract the folder to a location of your choice, and run ColoScopus.exe.

![alt text](<markdown images/release_download.png>)

When running the software for the first time on your computer, you will need to install .Net 6.0. Upon starting, you will be prompted for the Scopus API key you created earlier.

![alt text](<markdown images/Enter API key.PNG>)

## How to use



### Interface

The interface is split in two parts: the right part is a web browser to explore Scopus, the left part is where graphs are displayed and can be manipulated.

![alt text](<markdown images/interface.PNG>)

#### Node interface

Buttons related to nodes representing papers are listed below.

|Button|Action|
| :-----------: | :-----------: |
| ![alt text](<markdown images/add.png>) | Add or select a paper from the Scopus window |
| ![alt text](<markdown images/del.png>) | Removes a node from the graph |
| ![alt text](<markdown images/cite.png>) | Add papers citing the selected paper |
| ![alt text](<markdown images/link.png>) | Add citation links between the selected node and the other displayed nodes|
| ![alt text](<markdown images/interesting.png>) | Mark paper as interesting |
| ![alt text](<markdown images/important.png>) | Mark paper as important |
| ![alt text](<markdown images/revisit.png>) | Mark paper as to revisit later |

#### Graph interface

Buttons related to graph management and bibliography search are listed below.

|Button|Action|
| :-----------: | :-----------: |
| ![alt text](<markdown images/new_graph.png>) | Create a new graph |
| ![alt text](<markdown images/load.png>) | Open a graph |
| ![alt text](<markdown images/save.png>) | Save the current graph |
| ![alt text](<markdown images/export_csv.png>) | Export data to CSV |
| ![alt text](<markdown images/new_from_node.png>) | Create a new graph from a node |


### Adding the first paper

To create a new graph, log in Scopus in the right part of the window, then search for an article.

![alt text](<markdown images/paper_example.PNG>)

Click on the result you are interested in, then click on the "add" button to add the paper to the graph interface on the left.

![alt text](<markdown images/paper_example_added.PNG>)

### Forward searching

Forward reference searching corresponds to examining references citing a given article (https://libguides.fau.edu/c.php?g=966176&p=7013756). Forward searching in ColoScopus can be done by recursively selecting a paper, and adding all the papers citing it with the "cite" button.

### Backward searching

Backward reference searching in ColoSopus can only be done by selecting articles from the reference section of the Scopus interface. References of interest can be added to the graph by displaying their corresponding page in the Scopus interface and then clicking on the "add" button.

![alt text](<markdown images/backward_searching.png>)

### Exporting data to CSV files

Detailed information on the papers you marked as important or interesting can be exported. After clicking on the "Export to CSV" button, a pop-up window will appear displaying the number of papers exported.

![alt text](<markdown images/export_csv_dial.PNG>)

When you close this window, the folder where ColoScopus is running will open. The CSV files are saved in this folder, and you'll just have to copy them to a location of your choice. I recommend copying them in the same place you saved the corresponding graph.

![alt text](<markdown images/export_csv_folder.png>)

### Exploring graphs and keeping your bibliography up to date

Graphs created with this tool provide you with an overview of some research field. They are also convenient for keeping track of the papers you already screened.

![alt text](<markdown images/paper_example_graph.PNG>)

Saved graphs can be later opened to check for new citations of papers of interest.

Original graph | Graph with latest citation added for the selected node
:---: | :---:
![alt text](<markdown images/paper_example_end.PNG>) | ![alt text](<markdown images/paper_example_end_new.PNG>)

## Acknowledgements

All calls to Scopus's API are handled with Scopus.Dotnet.Client by arslanaybars (https://github.com/arslanaybars/Scopus.Dotnet.Client)
