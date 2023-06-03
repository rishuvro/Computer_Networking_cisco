# Computer_Networking_cisco
INDEX

1…VLAN

2…INTERVLAN

3…RIP

4…STATIC ROUTING

5…NAT  
6…SERVER

VLAN

**VLAN** is a custom network which is created from one or more local
area networks. It enables a group of devices available in multiple
networks to be combined into one logical network. The result becomes a
virtual LAN that is administered like a physical LAN. The full form of
VLAN is defined as Virtual Local Area Network.

<img src="./media/image1.png" style="width:6.5in;height:2.50833in" />The
below topology depicts a network having all hosts inside the same
virtual LAN:

Now, we will configure and make it works in cisco packet tracer.

-\> let, laptop0 and laptop 2 is in vlan10, and laptop1 and laptop3 is
in vlan20.

For configure vlan let,

Vlan10 ip=192.168.1.0/24

Vlan20 ip=192.168.2.0/24

<img src="./media/image2.png" style="width:7.57292in;height:5.04167in"
alt="Text Description automatically generated" />Command use in switch0
for configuring vlan….

Now we need to do the same thing in switch1 for configuring vlan.

<img src="./media/image3.png" style="width:6.95833in;height:2.87361in"
alt="Diagram Description automatically generated" />After configuring
both of the switch now I will give the ip of every laptops for vlan 10
and vlan 20.

Lets check the vlan is works or not….

<img src="./media/image4.png"
style="width:8.28255in;height:0.95833in" />Message:

<img src="./media/image5.png" style="width:4.43403in;height:1.87708in"
alt="Text Description automatically generated" />Pinging:

The vlan is works successfully.

<img src="./media/image6.png" style="width:6.5in;height:2.16389in"
alt="Table Description automatically generated with medium confidence" />Swtich0:

Switch1:

<img src="./media/image7.png" style="width:6.5in;height:2.325in" />

INTER VLAN ROUTING

Inter vlan routing is need for connecting one vlan to another.

Because of the inter vlan routing the router0 is connected to switch1 so
we need to trunk in fa3/1 , lets go do it….

Now we need to go in the router CLI to configure intervlan router

<img src="./media/image8.png" style="width:6.5in;height:1.44583in" />

<img src="./media/image9.png"
style="width:6.77083in;height:4.52083in" />now we need to configure in
Router0 for intervlan,

Now we fixed the default gateway of vlan10-192.168.1.1

And vlan20-192.168.2.1

Now the intervlan routing is done

Now we can access any pc of the vlan , lets

Pinging-

<img src="./media/image10.png"
style="width:5.11458in;height:2.3808in" />

The intervlan is done.

<img src="./media/image11.png" style="width:6.5in;height:3.45069in" />The
final form is

RIP

<img src="./media/image12.png"
style="width:7.3125in;height:4.91667in" />*Routing Information
Protocol* (RIP) is a distance-vector routing protocol. Routers running
the distance-vector protocol send all or a portion of their routing
tables in routing-update messages to their neighbors.

We are performing rip in these 4 router ,

First Router0:

<img src="./media/image13.png" style="width:6.5in;height:3.65208in" /><img src="./media/image14.png" style="width:6.5in;height:4.01042in" />Router1:

<img src="./media/image15.png"
style="width:6.32292in;height:3.77153in" /><img src="./media/image16.png" style="width:6.5in;height:3.97569in" />Router3:

Router2:

Now all done, lets ping any of the four interface from the laptop….

<img src="./media/image17.png" style="width:6.5in;height:2.90139in" />

<img src="./media/image18.png"
style="width:5.8125in;height:3.90139in" />We get reply from router
interface, that’s we can say the rip is successfully done.

NAT

NAT, in which the Private IP address or local address are translated
into the public IP address. NAT is used to slow down the rate of
depletion of available IP address by translates the local IP or Private
IP address into global or public ip address. NAT can be a one-to-one
relation or many-to-one relation.

For this well will take a router as isp , the we will perform NAT int
our topology…it will be looks like this

<img src="./media/image19.png" style="width:6.5in;height:5.31042in" />

No we need to perform static routing in router 3 and 4,,

For router 3..

<img src="./media/image20.png" style="width:6.5in;height:1.93125in" />

For router4…

<img src="./media/image21.png" style="width:6.5in;height:2.41181in"
alt="Graphical user interface, text, application Description automatically generated" />

<img src="./media/image22.png" style="width:6.5in;height:5.11944in" />Now
perform Nat

now configure the server…

<img src="./media/image23.png"
style="width:5.94792in;height:2.55208in" />

<img src="./media/image24.png" style="width:6.5in;height:4.59236in" />

Lets do search

<img src="./media/image25.png" style="width:6.5in;height:6.07917in" />
