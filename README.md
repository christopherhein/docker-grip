# Grip Server

Allows Github Style README previewing.

## Usage

If you use Docker Compose you and add this to your file:

    grip:
      image: christopherhein/grip
      volumes:
        - ./README.md:/work/README.md
      ports:
        - "6419:6419"

If you'd just like to run a one preview the command would look like:

    $ docker run -p 6419:6419 -v README.md:/work/README.md christopherhein/grip


