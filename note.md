# Intro to High-Quality VFX with Houdini

## 13

```text
lerp(Position A, Position B, bias);
getbbox(0,min,max);
v@rel = relbbox(0,v@P);
```

## 14

```text
centroid(surface_node, type)
```

## 15

Point Cloud

```text
// pcopen(geometry B input(reference geometry), "B Position", Position attribute, reference range(radius), number of Point to be referenced)
// pcfilter(handle,"Attribute to be imported")

int handle = pcopen(1,"P",v@P,1.0,1)
v@Cd = pcfilter(handle,"Cd")
```

xyzdist

```text
// float xyzdist(geometry, origin, &prim, &uv)
```

## 17

Alt + E : Edit Expression (Write H Script in)
