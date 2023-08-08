# Automation++
a mod for [Cosmoteer](https://cosmoteer.net/)

### Version 2.0.0 for Cosmoteer 0.23.1
This is a modern version of the mod
[Classic versions are available on the Cosmoteer forum](https://forum.cosmoteer.net/d/12348-automation-1-3-1-power-reloaded)

Distributed under the MIT License. See [LICENSE](LICENSE) for more information.

## Roadmap

- ### I) updating
    - #### A) update code to not crash the game
        - ##### buffs : check if good
        - ##### gui : find mod adding gui elements as examples
        - ##### ai : find file for ai logic (triggers and toggles)
        - ##### decals : check if good
        - ##### strings : check if good
        - ##### parts
            - ###### uniformize parts type category
            - ###### check usefulness of GeneratorRequiresDoor = false & NoAutoDoors = true
            - ###### check replacement of AreaAmmoDrain for WifiProvider
            - ##### ai mainframe
                - graphics code
            - ##### ammo belt
            - ##### auto gun
            - ##### auto laser
            - ##### auto rifle
            - ##### auto loaders
            - ##### auto reactors
                - update graphics code after doing sprites
            - ##### capacitor
                - find a new name : automated capacitor ?
            - ##### circuit breaker
            - ##### console
            - ##### coupling wires
            - ##### drone controller
            - ##### drone cores
            - ##### drone ftl
                - update vanilla ftl as needed to give them the same features
            - ##### ftl resonator
            - ##### internal structure : check if good
            - ##### nodes
            - ##### scout shield
                - SelectionTypeID = "shield" > "shield_gen"
            - ##### semiconducting wires
            - ##### small sensor
                - graphics code
            - ##### transformer
                - graphics code
            - ##### weapon controller : check if good
                - update graphics code after finishing sprites

    - #### B) remake sprites in modern style
        - ##### buffs : wrong shade of green, add shadow
            - redo range buff and accuracy buff
        - ##### gui : redo all + check code for merging sprites
        - ##### decals : check if good
        - ##### parts 
            - ##### ai mainframe
            - ##### ammo belt
            - ##### auto gun : mix point defense and small laser
            - ##### auto laser : mix point defense and disruptor
            - ##### auto rifle : mix classic sprites and point defense
            - ##### auto loaders : don't spend too much time on ammo and missile auto loader as size might change when grinders get added
            - ##### auto reactors : regular reactors with extra stuff
                - check schematic in secret folder
                - bonus : differents lights for each modes
            - ##### capacitor
            - ##### circuit breaker
                - blueprint : green
                - roof sprites
                - normal map
                - doodads for lights
                - damage levels
            - ##### console : 2x2 control room with extra stuff
            - ##### coupling wires
            - ##### drone controller : 3x3 control room with extra stuff
            - ##### drone cores
            - ##### drone ftl : regular ftl but smaller
            - ##### ftl resonator
            - ##### internal structure : done
            - ##### nodes
            - ##### scout shield : large shield but very small
            - ##### semiconducting wires
            - ##### small sensor : mix big sensor sprites with radar from control rooms
            - ##### transformer
                - blueprint : green
                - roof sprites
                - normal map
                - doodads for lights
                - damage levels
            - ##### weapon controller
                - blueprints : red
                - roof sprites
                - normal map if different than roof light 
                - merge floor, optimize doodads
                - damage levels

- ### II) porting and balancing
    - #### A) rewrite parts to make them useful and not op
        - ##### auto loaders : take ressources from grinders to produce ammo

    - #### B) add new parts as needed
        - ##### grinders : one for each natural resources, store large amount of resources for auto loader only
        - ##### ammo belt for other ammo
        - ##### auto storage : like an ammo belt, but with more storage
        - ##### small automated resource collector : 1x1, smaller range
        - ##### large automated resource collector : 3x3, longer range
        - ##### drone mining drill : 2x2 side mount, short range
        - ##### extra cpu : more command points for drone core
        - ##### automated hyperdrive beacon

    - #### C) add feature and qol
        - ##### fire resistance buff or automated fire extinguisher (might need c# to not look janky)
        - ##### make transformer and circuit breaker detect autoreactor adjacency for turning on
        - ##### weapon controller code glue reset crew priorities 
            - solution : leaving partcrew as is, add crewtoggle and replace partcrew references by crewtoggle reference (pro: bug removed, cons: more code, more works to make other mods compatible with auto++)

- ### III) c# or waiting for feature
    - ##### removing crew from drone : prevent ship from turning into junk when no crew on board if they have a node
    - ##### build/repair ships without crew


- ### ?) faction ships and career content
