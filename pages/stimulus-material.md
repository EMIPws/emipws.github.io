---
layout: single
permalink: /stimulus-material/
header:
title: "Distributed Collection of Eye Movement Data in Programming - Stimulus Material"
sidebar:
  nav: "main"
---

The EMIP Distributed Data Collection includes the two programs “Rectangle” and “Vehicle”, which are available in Java, Python, and Scala. In order to avoid effects from the order in which the programs are presented, it alternates between participants:

- participant1 sees Rectangle first, Vehicle second
- participant2 sees Vehicle first, Rectangle second
- participant3 sees Rectangle first, Vehicle second
- …

## Downloads
- [Stimulus material](/assets/EMIP_DataCollection_Material.zip) consisting of:
  - “Rectangle” and “Vehicle” in Java, Python, and Scala
  - Comprehension questions
  - Participant questionnaire
  - Instructions
- [Files for SMI Experiment Center](/assets/EMIP_DataCollection_SMI.zip)

## Java Version

**Rectangle**

```java
public class Rectangle {
   private int x1 , y1 , x2 , y2 ;
   
   public Rectangle ( int x1 , int y1 , int x2 , int y2 ) {
      this.x1 = x1 ; 
      this.y1 = y1 ; 
      this.x2 = x2 ; 
      this.y2 = y2 ;
   }

   public int width ( ) { return this.x2 - this.x1 ; }

   public int height ( ) { return this.y2 - this.y1 ; }

   public double area ( ) { return this.width ( ) * this.height ( ) ; } 

   public static void main ( String [ ] args ) {
      Rectangle rect1 = new Rectangle ( 0 , 0 , 10 , 10 ) ; 
      System.out.println ( rect1.area ( ) ) ;
      Rectangle rect2 = new Rectangle ( 5 , 5 , 10 , 10 ) ; 
      System.out.println ( rect2.area ( ) ) ;
   } 
}
```
The program

- … computes the area of rectangles by multiplying their width (x1-x2) and height (y1-y2).
- … computes the area of rectangles by multiplying their width (x2-x1) and height (y2-y1).
- … computes the area of rectangles by multiplying their width (x1-y1) and height (x2-y2).
- I’m not sure.
 

**Vehicle**

```java
public class Vehicle {
   String producer , type ;
   int topSpeed , currentSpeed ;

   public Vehicle ( String p , String t , int tp ) {
      this.producer = p ; 
      this.type = t ; 
      this.topSpeed = tp ; 
      this.currentSpeed = 0 ;
   } 

   public int accelerate ( int kmh ) {
      if ( ( this.currentSpeed + kmh ) > this.topSpeed ) { 
         this.currentSpeed = this.topSpeed ;
      } else {
         this.currentSpeed = this.currentSpeed + kmh ;
      }
      return this.currentSpeed ; 
   }

   public static void main ( String args [ ] ) {
      Vehicle v = new Vehicle ( "Audi" , "A6" , 200 ) ; 
      v.accelerate ( 10 ) ;
   } 
}
```
The program

- … defines a vehicle by a producer, that has a type and can reduce its speed.
- … defines a vehicle by a producer, that has a type and can accelerate its speed.
- … defines a vehicle by a producer, that has a type and can accelerate and reduce the speed.
- I’m not sure.