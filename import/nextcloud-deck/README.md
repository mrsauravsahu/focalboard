# Nextcloud Deck importer

This node app converts data from a Nextcloud Server with the [app Deck](https://apps.nextcloud.com/apps/deck) installed into a Focalboard archive. To use:

1. Run `npm install` from within `focalboard/webapp`
2. Run `npm install` from within `focalboard/import/nextcloud-deck`
3. Run `npx ts-node importDeck.ts -o archive.focalboard` (also from within `focalboard/import/nextcloud-deck`)
   1. Enter URL and credentials (can also be provided via cli arguments)
   2. Enter ID of the board to convert
4. In Focalboard, click `Settings`, then `Import archive` and select `archive.focalboard`

## Import scope

Currently, the script imports all cards from a single board, including their stacks (column) membership, labels, names, descriptions, duedate and comments. [Contribute code](https://www.focalboard.com/contribute/getting-started/) to expand this.


