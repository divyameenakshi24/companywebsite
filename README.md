# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Hexabyte Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'css/img/hb.jpg' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
       HEXABYTE PRIVATE LIMITED
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a href="/people">People</a></div>
        <div class="menuitem"><a href="/contact">Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2021 Hexabyte Private Limited, Developed by Divya Meenakshi
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
        <h1><u>ABOUT US</u></h1>
        <img src="/static/img/office.jpg" alt="office">
    
        <div class="contenttext">
            Hexabyte Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
            <ul>
                <li>Memory Chips</li>
                <li>SATA HDD</li>
                <li>SATA SSD </li>
                <li>Broadband Modems</li>
                <li>Wifi Devices</li>
                <li>Switching Devices</li>
                <li>Optical Sensors</li>
            </ul> 
        </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1><u>Our Premium Products</u></h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/optical.jpg" alt="product image">
            </div>
            <div class="itemname">WTB12-3P2431 SICK - Optic sensor 1041411</div>
            <div class="itemprice">Price: Rs.20569.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/router.png"  alt="product image">
            </div>
            <div class="itemname">XIAOMI MI 4C WIRELESS ROUTER (DVB4211IN, WHITE)</div>
            <div class="itemprice">Price: Rs.1099.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/samsung.jpg"  alt="product image">
            </div>
            <div class="itemname">Samsung 860 EVO 500GB SATA 2.5" Internal Solid State Drive (SSD) (MZ-76E500)</div>
            <div class="itemprice">Price: Rs.6299.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/zeb.jpg"  alt="product image">
            </div>
            <div class="itemname">Zebronics Motherboard ZEB-G41 Socket 775.</div>
            <div class="itemprice">Price: Rs.2590.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/sound.jpg"  alt="product image">
            </div>
            <div class="itemname">Focusrite Scarlett Solo (3rd Gen) USB Audio Interface with Pro Tools, First</div>
            <div class="itemprice">Price: Rs.9995.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/gpu.jpg"  alt="product image">
            </div>
            <div class="itemname">ASUS GeForce GT710 2GB GDDR5 64-Bit Graphics Card with 0db Low Profile</div>
            <div class="itemprice">Price: Rs.2999.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/mic.jpg"  alt="product image">
            </div>
            <div class="itemname">Audio-Technica AT2020TYO Cardioid Condenser Studio Microphone (NA, Blue)</div>
            <div class="itemprice">Price: Rs.11000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/cams.png"  alt="product image">
            </div>
            <div class="itemname">HP W100 WEBCAM FOR DESKTOP (480P RESOLUTION, 1W4W4AA, BLACK)</div>
            <div class="itemprice">Price: Rs.1699.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/gaming.jpg"  alt="product image">
            </div>
            <div class="itemname">ASUS ROG Strix Z490-F Gaming</div>
            <div class="itemprice">Price: Rs.25600.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/floppy1.jpg"  alt="product image">
            </div>
            <div class="itemname">USB Floppy Drive Emulator for Electronic Organ</div>
            <div class="itemprice">Price: Rs.1800.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/beats.jpg"  alt="product image">
            </div>
            <div class="itemname">Beats by Dr. Dre Studio3 Wireless Bluetooth Headphones (Blue)</div>
            <div class="itemprice">Price: Rs.40300.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/point.jpg"  alt="product image">
            </div>
            <div class="itemname">Logitech Wireless Presenter R400 (Black)</div>
            <div class="itemprice">Price: Rs.2299.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
### people.html
```

{% extends "website/base.html" %}

{% block content %}
    <div class="peoplecontent">
    <h1><u>Our Crew</u></h1>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/css/img/rm.png" alt="member image" style="width:200px;height:250px;">
            </div>
            <div class="membername">KIM NAMJOON</div>
            <div class="designation">C.E.O AK CORP</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/css/img/jin.jpg" alt="member image" style="width:200px;height:250px;">
            </div>
            <div class="membername">KIM SEOKJIN</div>
            <div class="designation">FRONTEND DEV</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/css/img/suga.jpg" alt="member image" style="width:200px;height:250px;">
            </div>
            <div class="membername">MIN YOONGI</div>
            <div class="designation">TECHNICAL TEAM</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/css/img/hobi.jpg" alt="member image" style="width:200px;height:250px;">
            </div>
            <div class="membername">JUNG HOSEOK</div>
            <div class="designation"> R & D HEAD </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/css/img/mochi.jpg" alt="member image" style="width:200px;height:250px;">
            </div>
            <div class="membername">PARK JIMIN</div>
            <div class="designation"> DESIGN TEAM </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/css/img/v.jpg" alt="member image" style="width:200px;height:250px;">
            </div>
            <div class="membername">KIM TAEHYUNG</div>
            <div class="designation"> MARKETING HEAD </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/css/img/jk.jpg" alt="member image" style="width:200px;height:250px;">
            </div>
            <div class="membername">JEON JUNGKOOK</div>
            <div class="designation"> PROJECT MANAGER </div>
        </div>
    </div>    
 {% endblock  %}
```
### contact.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="content">

        <p class="free">

        </p>
        <div class="contain">
            <div class="image">
                <img src="/static/css/img/contactus.jpg" alt="contact" width="1050" height="300">
            </div>
            <div class="text">
            <h2><u>CONTACT NO:</u><br>
                +822 34440105</h2>
            </div>
        </div>
        <div class="contain">
            <div class="image">
            </div>
            <div class="text">
                <h2><u>EMAIL:</u><br>
                hexabytepvt.ltd@gmail.com</h2>
            </div>
            <div class="text">
                <h2><u>ADDRESS:</u><br>
                42 Teheran-ro 108-gil, Daechi-dong,<br>
                Gangnam-gu, Seoul, South Korea
                </h2>
            </div>
        </div>
    </div>

{% endblock  %}
```



## OUTPUT:
![output](./static/img/o1.png)

![output](./static/img/o2.png)

![output](./static/img/o3.png)

![output](./static/img/o4.png)

![output](./static/img/o5.png)

![output](./static/img/o6.png)

## CODE VALIDATION REPORT:
![output](./static/img/home.png)

![output](./static/img/products.png)

![output](./static/img/people.png)

![output](./static/img/contact.png)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://divya.student.saveetha.in:8000/. HTML code is validated.