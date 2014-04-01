# hbf_phylesystem_test

This is a temporary repo of NexSON 1.2.1 to be used for testing the 
api.opentreeoflife.org. It will be removed when those tests complete
and the new curation application "goes live."

This is a full translation into "HoneyBadgerFish 1.2.1" of the phylesystem
repository use in the estimation of the full Tree of Life by the 
[Open Tree of Life](http://opentreeoflife.org) project.

Assuming that you have the directory structure:

    somepath/phylesystem
    somepath/peyotl

then you can create the content of this directory by:

    cd somepath/phylesystem
    python bin/refresh_nexsons_from_phylografter.py -v
    cd ../peyotl
    mkdir -p ../phylesystem-par/phylesystem-0/study
    mkdir ../scratch
    python dev/migrate_testing_phylesystem.py ../phylesystem ../sharded-phylesystem-par/phylesystem-0 ../scratch

# More details

See [phylesystem](https://github.com/OpenTreeOfLife/phylesystem) for more details.

## License

The *data* in this repository is released under the [Create Commons Zero 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) license.

