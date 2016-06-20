All you have to do is to plug in your RTL2832u compatible USB receiver and run the container :)

<code>
docker run --privileged -v /dev/bus/usb:/dev/bus/usb mradochonski/dump1090-docker
</code>

It exposes the following ports:
 - 8080 -> data feeds and basic website for data visualisation
 - 30001 -> raw input port
 - 30002 -> raw output
 - 30003 -> SBS1 (BaseStation) format output
 - 30004 -> Beast input port
 - 30005 -> Beast output port

