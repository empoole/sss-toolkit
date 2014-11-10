sss-toolkit is intended to help you get a new sass project off the ground quickly.

The toolkit contains an assortment of helper mixins and functions as well as a built-in fluid grid system that you can use with any project.

sss-toolkit is built according to BEM and SMACSS principles to make it easy to maintain.

CONTENTS and USAGE:
The main.scss file in the sss-toolkit directory is used to collect all of the partial files from each of the different SMACSS directories located in the SMACSS folder.  This file should not need to be changed.  Simply run the following command to create your main css file:

sass --watch main.scss

Inside the SMACSS directory there are several additional directories, each of which contains it's own _main.scss partial.  These files must be updated with any new partials you create for your project.


CONFIGURATION
To configure your new sass project use the included _config.scss partial located in the SMACSS/Base directory.  There is a sample config file included to help get you started.

Here you can define color schemes, color palletes, fonts and grid properties in one location so that you can make quick changes to the overall look of your project easily.


USING THE GRID
sss-toolkit includes a built-in grid system similar to that found in Bootstrap.  You can edit the number of grid columns and their various properties in the _config.scss file located in the SMACSS/Base directory.

Once your grid is set up include the class "grid" to an element you would like to use as your grid container and classes grid__col--x to each column element within the container where x is the number of grid columns you would like that element to span.