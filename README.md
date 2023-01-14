# USB Descriptor Generator

Generate USB descriptors from parameters.

## Background

This code comes from CircuitPython, but was [removed unceremoniously](https://github.com/adafruit/circuitpython/commit/f0564b49862eaef0b9752b62d80ef00e3e12a3ee) in 2021. It is still very useful, and so has been brought out to this project.

## Usage

Clone this repository recursively:

```
git clone https://github.com/xobs/usb-descriptor-generator.git
cd usb-descriptor-generator
git submodule update --init --recursive
```

Then, run the command:

```
python mkdescriptor.py --manufacturer "Kosagi" --product "Precursor" --vid 0x1209 --pid 0x1234 --output_c_file temp.c --output_h_file temp.h --max_ep 16
```

This will generate output files with your descriptors in them.
