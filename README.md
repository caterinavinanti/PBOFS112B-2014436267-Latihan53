# PBOFS112B-2014436267-Latihan53

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author ASUS
 * Nama     : Caterina Vinanti
 * Kelas    : PBO FS112B
 * NIM      : 201443267
 * Deskripsi program : Program ini berisi pemrograman Rabbit
 */

class Animal {
    boolean vegetarian;
    String eats;
    int noOfLegs;
    Rabbit rabbit;
    
    Animal(boolean vegetarian, String food, int legs) {
        this.vegetarian = vegetarian;
        this.eats = food;
        this.noOfLegs = legs;
    }
    
    boolean isVegetarian() {
        return this.vegetarian;
    }
    
    String getEats() {
        return this.eats;
    }
    
    int getNoOfLegs() {
        return this.noOfLegs;
    }
}

class Rabbit {
    String color;
    String name;
    Animal animal;
    
    Rabbit(String name, boolean veg, String food, int legs, String color) {
        this.color = color;
        this.name = name;
    }
    
    String getColor() {
        return this.color;
    }
    
    String getName() {
        return this.name;
    }
}

/**
 *
 * @author eLx
 */
public class PBOFS112B_2014436267_Latihan53_Rabbit {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Animal animal1 = new Animal(false, "grass", 4);
        Rabbit rabbit1 = new Rabbit("Peter", animal1.isVegetarian(), animal1.getEats(), animal1.getNoOfLegs(), "grey");
        System.out.println("Hello, His name is " + rabbit1.getName());
        System.out.println(rabbit1.getName() + " is Vegetarian? " + animal1.isVegetarian());
        System.out.println(rabbit1.getName() + " eats " + animal1.getEats());
        System.out.println(rabbit1.getName() + " has " + animal1.getNoOfLegs() + " legs");
        System.out.println(rabbit1.getName() + "'s color is " + rabbit1.getColor());
    }
    
}

