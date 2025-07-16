# ColoScopus 1.3.1

ColoScopus is a graphical bibliography software. Literature review is carried out in the form of graphs, similar to research rabbit (https://www.researchrabbit.ai/) or connected papers (https://www.connectedpapers.com/). ColoScopus does not resort to IA, and searches local.

## Getting started

### Access to Scopus API
ColoScopus relies on data provided by the Scopus API. An access to Scopus and an API key are therefore required.
Head to https://dev.elsevier.com/, click on "My API Key" and log in. 

![alt text](<markdown images/Scopus dev portal.PNG>)

Create an API key and copy it.
![alt text](<markdown images/Scopus dev portal api key created.PNG>)


### Launching ColoScopus
When running the ColoScopus.exe for the first time on your computer, you should install .Net 6.0. Uppon starting, you will be prompted for your Scopus API key.

![alt text](<markdown images/Enter API key.PNG>)

## How to use



### Interface

The interface is split in two parts: the right part is a web browser to explore Scopus, the left part is where graphs are displayed. 

#### Node interface

Buttons related to nodes representing papers are listed below.

|Button|Action|
| :-----------: | :-----------: |
| ![alt text](<markdown images/add.png>) | Add or select a paper from the Scopus window |
| ![alt text](<markdown images/del.png>) | Removes a node from the graph |
| ![alt text](<markdown images/cite.png>) | Add papers citing the selected paper |
| ![alt text](<markdown images/link.png>) | Add citation links between the selected node and the other displayed nodes|
| ![alt text](<markdown images/interesting.png>) | Mark paper as interesting |
| ![alt text](<markdown images/important.png>) | Mark the paper as important |
| ![alt text](<markdown images/revisit.png>) | Mark the paper as to revisit later |

#### Graph interface

Buttons related to graph management and bibliography search are listed below.

|Button|Action|
| :-----------: | :-----------: |
| ![alt text](<markdown images/new_graph.png>) | Create a new graph |
| ![alt text](<markdown images/load.png>) | Open a graph |
| ![alt text](<markdown images/save.png>) | Save the current graph |
| ![alt text](<markdown images/export_csv.png>) | Export data to CSV |
| ![alt text](<markdown images/new_from_node.png>) | Create a new graph from a node |


## Important information

ColoScopus is a hobby project, although developped with the best intent, use at your own risk. The author is not related to 
ColoScopus is only expected to run on Windows 7 or higher. 
Calls to Scopus's API are handled with Scopus.Dotnet.Client by arslanaybars (https://github.com/arslanaybars/Scopus.Dotnet.Client)
