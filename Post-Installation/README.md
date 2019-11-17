### VerbStub
Fixes the audio issues (noise when plugging in headphones, audio not working after sleep, etc.). 
* Make sure your `layout-id` is set to `72` in Clover settings (Devices > Properties > PciRoot(0)/Pci(0x1f,3) > layout-id)
* Open the Terminal, `cd` to the VerbStub folder and type in `./install.sh`. Follow the instructions on the screen

### VoltageShift
* Undervolting can help reduce heat and improve battery life while not losing any performance. It works by lowering the voltages of CPU, GPU and CPU cache.
* Read the instructions here: https://github.com/sicreative/VoltageShift#voltageshift
* i7-8750H allows to about -150mV undervolting so I would suggest you take this as a starting point. 
* You can also apply a more conservatinve undervolt on the GPU (about 75mV).
* Try it with `./voltageshift offset -150 -75` first, tune it accordingly. 
* Once you've found the configuration that works for you, you can apply the undervolt on every boot: `sudo ./voltageshift buildlaunchd  -150 -75 0 0 0 0 60`
