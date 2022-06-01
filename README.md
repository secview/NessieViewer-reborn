# Nessie Viewer - Reborn

# Why Nessie Viewer ? 

The tool is called NessieViewer as it will let you find the real issues hidden deep inside the lake of false positives.
https://en.wikipedia.org/wiki/Loch_Ness_Monster


# Usage ?

Nessus viewer was originally used to quickly find issues contained in a nessus or nmap report by sorting and filtering each entry. It is able to import entries from a nessus xmlV2 report and nmap xml report (-oA) and filter them by host IP, host name, plugin name, operating system, keywords ...
Try to double click on an IP to have a summary view of one host or generate clickable links to begin your tests.

Nessie Viewer Reborn is an update adding several improvements. It is a standalone tool for windows that allows you to quickly sort, group and find flaws based on the output of multiple  scanning tools (Nmap xml, Nessus xml, Zap xml, ...). 

# Interface 

The filter section allows you to filter specific values in the table. It is possible to filter the following elements:
- PluginID
- PluginName
- Host IP
- Host Name
- OS
- Port
- Service
- Risk
- Plugin Description
- Plugin Output

Multiple filters can be added, comma separated. Minus is used to remove entries. 

Right click on a line to quickly add a filter.

Double click on a cell (but not hostIP) to list all hosts with the same cell value.

Double click on one "Host Ip" cell to summarize all issues for this host.

Menu "Generate -> Generate links" and "Generate -> Parse plugin output" : Easy configurable way to parse all plugins output and create custom links for scripting.
Configuration can be done from "option" menu. 


# Parsers

- Nessus XML
- Nmap xml (-oX or -oA)


# Platform 

- Windows with C#
- Linux : 
-- Mono
-- Java implementation of NessieViewer (different project): https://github.com/vdbaan/IssueFinder
