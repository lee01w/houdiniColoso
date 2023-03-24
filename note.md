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

## 20

```text

dot(A,B) = length(A) * length(B) * cos(θ)
θ = acos(dot(A,B) / length(A)*length(B))

A : normalized vector
B : normalized vector
θ = acos(dot(A,B))
```

cross(a,b) : solver를 활용하여 회전 시킬 수 있다
dot(a,b) : 각 point의 normal과 특정 vector의 normal의 각도을 계산하고, 일정 각도의 포인트를 제거하면 눈이 쌓인 효과를 연출할 수 있다.

## 22

@nage : @age / @life
