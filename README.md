# Alfresco CLI - Command line interface for Alfresco

> Interact with the Alfresco repository with an interactive command line.

## Target Audience

-   Alfresco Developers and Architects

## Installation

### From NPM

-   Run `npm install -g alfresco-cli`

### From GitHub

-   Clone the repository

-   Install using `npm install -g && npm link`

## Usage

-   Call `alfresco-cli` from your terminal.

### Logging in

Type `login --help` to read the help on logging in to the system and fetch an authentication token for the CLI.

### Changing into a node

Use `cd <nodeId>`, where nodeId is the node ID of the nodeRef you want to change to.

### Listing contents (chldren) within a node

Use `ls` or `ls <nodeId>` to list contents within a node.

### Uploading files

Use `upload <filePath> [destinationNodeId]` to upload new files to Alfresco.

### Search for contents

Use `search <query> [language]` to search for contents.

### Commands and Operations

-   Login

-   Logout

-   List files

-   List sites

-   Upload files

-   Download files \[TBD\]

-   View Metadata

### Aliases Reference

You can use the following aliases within commands.

-   `.` - current folder/content

-   `..` - parent folder/content

## License

MIT License

## Author

-   Bhagya Nirmaan Silva (about.me/bhagyas)

## Development Sponsors

-   [Loftux AB](http://loftux.com)

## Privacy Policy

There are no analytics gathered upon the use of the tool. However, the author reserves the right to add analytics on a later release to improve features provided by the tool.

## Contributors

None

## Version History

-   1.2 - 20181025

    -   \[MAJOR\] Adding folder name auto completion

    -   Added `delete` command with support for deleting child nodes.

-   1.1 - 20181024

    -   Converted the code to Typescript

    -   Added support for node name as an alias for nodeId when referred from a valid context.

    -   Added `create user`, `create site`, `cd-site` commands.

    -   Added support for `.` and `..` aliases.

-   1.0 - 20181023

    -   Initial release
