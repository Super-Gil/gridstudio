<img src='http://gridstudio.io/image/logo-grid.svg' width='200px' style='margin-bottom: 30px;'>

This is just a copy of ricklamer's grid studio.
I really love the project!

Grid studio is a web-based spreadsheet application with full integration of the Python programming language.

It intends to provide an integrated workflow for loading, cleaning, manipulating, and visualizing data. This is achieved through a spreadsheet backend written in Go with integration of the Python runtime to manipulate its contents.

### Architecture overview
The application is structured in two parts:

1. The (centralized) workspace manager
    1. CRUD interface for creating, copying, editing and deleting workspaces.
    1. Proxy to send traffic to the right workspace environment (part 2)
1. Workspace Go execution environment
    1. Go cell parsing and evaluating spreadsheet backend
    1. Node.js terminal session
    1. Python interpreter integration

For more details about each part check out the code in the repository. If anything is unclear (or unreadable - not all code is equally pretty!)
