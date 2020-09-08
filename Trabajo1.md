/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package com.mycompany.com.pascual.trabajo;
import java.util.Scanner;

/**
 *
 * @author alexd
 */
public class Principal {
    
    
    
    public static void main(String[] args){
    
    float [] Altura = new float [5];
    float [] Edad = new float [5];
    float EstaturaPromedio = 0;
    float EdadPromedio = 0;
    int ContadorMayoresAños=0;
    int ContadorMasAltos=0;
    
    Scanner datos = new Scanner(System.in);
    
        System.out.println("Digite la edad de los alumnos: ");
        for (int i = 0; i < 5; i++) {
            
            Edad[i] = datos.nextFloat();
            EdadPromedio = EdadPromedio + Edad[i];
            System.out.println("Guardado");
            
            if (Edad[i] > 18) {
                ContadorMayoresAños++;
            }
            
        }
        
        
        System.out.println("Digite la altura de los alumnos: ");
        for (int i = 0; i < 5; i++) {
            
            Altura[i] = datos.nextFloat();
            EstaturaPromedio = EstaturaPromedio + Altura[i];
            System.out.println("Guardado");
            
            if (Altura[i] > 1.75) {
                ContadorMasAltos++;
            }
        }
        
        EdadPromedio = EdadPromedio/5;
        EstaturaPromedio = EstaturaPromedio/5;
        
        
        System.out.println("La altura promedio es de " + EstaturaPromedio);
        System.out.println("La edad promedio es de " + EdadPromedio);
        System.out.println("La cantidad de alumnos que miden más de 1.75 metros es: " + ContadorMasAltos);
        System.out.println("La cantidad de alumnos mayores de 18 años es: " + ContadorMayoresAños);
        
        
    
}
    
   
    
}
