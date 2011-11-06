# Get Stuff Done Host Filter
`gsd` is a small utility that allows you to quickly filter out
distracting websites and get stuff done.

It works by repalcing your systems /etc/hosts file with a custom
version of the file that is maintined in ~/.gsd/myhosts.

# Installation

1. Clone gsd repository
2. `sudo make install`

# Usage

## Enable Filter
To enable the filter, simply run

    sudo gsd enable

## Disbale Filter
To disable the filter, run

    sudo gsd disable

## Check the Filter's status
To check whether the filter is active and to see the which sites are
currently being filtered, run

    gsd status

## Add site to filter
To add sites to your gsd filter, run

    gsd add SITE_NAME

If SITE_NAME does not start with 'www', an entry including 'www' will
also be added automatically.

## Remove site from filter
To remove a site from your gsd filter, run

    gsd del ENTRY_NUM

where ENTRY_NUM is the number of the entry displayed in `gsd status`.

## Reload the filter
To reload the filter after modifying the list of filtered sites, run

    sudo gsd relaod

