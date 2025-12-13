# openHAB3_ui_widgets

## sources

### github repos

1. [openHAB3Widgets](https://github.com/BangerTech/openHAB3Widgets)
1. [OpenhabWidget](https://github.com/massimilianocasini/OpenhabWidget)
1. [HeatingWidget](https://github.com/NRquadrat/oh3-widgetHeating)
1. [oh3-widgets](git@github.com:Rosi2143/oh3-widgets.git)
1. [ScrewPlate](git@github.com:Rosi2143/ScrewPlate.git)
1. [robowidget](git@github.com:Hypfer/Valetudo-Openhab.git)

### [openhab community](https://community.openhab.org/)
- see the readme file in the directory
- branch conventions
   - main branches are the "originals"
   - master branches are "my" versions

# tips and tricks
## Display State vs. State
* https://www.openhab.org/docs/ui/building-pages.html#dynamically-configuring-components-with-expressions

The @ symbol can be used in front of an item name string as a shortcut to the displayState from the items dictionary with a fallback to the raw state:

    footer: =@'Switch1'

is the same as

    footer: =items['Switch1'].displayState || items['Switch1'].state

Similarly, @@ can be used as a shortcut for just the item state.
