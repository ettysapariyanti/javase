# Catatan Java SE

Di bawah ini source code untuk membuat label, tombol, dan perintah di dalam tombol:

```java

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package com.steven.latihan2;

/**
 *
 * @author owner
 */

import java.awt.*;

import java.awt.event.*;

import java.awt.Font;

import javax.swing.*;



public class file5 {
    
    public static void membuatWindow(){
    
    JFrame bingkai1 = new JFrame("Label dan Tombol");
    
    bingkai1.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    
    JLabel lbKodeEmiten, lbNamaEmiten;
    
    JButton tbUbahNamaEmiten;
    
    lbKodeEmiten = new JLabel("Kode Emiten : ");
    
    lbNamaEmiten = new JLabel("Nama Emiten : ");
    
    tbUbahNamaEmiten = new JButton("Ubah Nama Emiten");
    
    lbKodeEmiten.setFont(new Font("Arial", Font.BOLD, 20));
    
    lbNamaEmiten.setFont(new Font("Arial", Font.BOLD, 20));
    
    tbUbahNamaEmiten.setFont(new Font("Arial", Font.BOLD, 15));
    
    lbKodeEmiten.setBounds(10, 10, 200, 30);
    
    lbNamaEmiten.setBounds(10, 50, 200, 30);
    
    tbUbahNamaEmiten.setBounds(10, 100, 250, 30);
    
    
    // Mengisi tbUbahNamaEmiten  dengan perintah yg bisa dijalankan
    
    tbUbahNamaEmiten.addActionListener(new ActionListener(){
    
        public void actionPerformed(ActionEvent e){
        
            lbNamaEmiten.setText("Harga Saham : ");
        
        }
        
        
    });
    
    
    bingkai1.add(lbKodeEmiten);
    
    bingkai1.add(lbNamaEmiten);
    
    bingkai1.add(tbUbahNamaEmiten);
    
    bingkai1.setSize(500, 500);
    
    bingkai1.setLayout(null);
    
    bingkai1.setVisible(true);
    
    }
    
    
    public static void main(String[]args){
    
    
        membuatWindow();
    
    }
    
    
    
}


```




Source code untuk merubah warna JFrame, membuat JTextField, mengubah font JTextField :

```java

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package com.steven.latihan2;

/**
 *
 * @author owner
 */

import java.awt.*;

import java.awt.event.*;

import java.awt.Font;

import javax.swing.*;



public class file6 {
    
    
    public static void membuatWindow(){
    
        JFrame bingkai1 = new JFrame("Label TextBox Tombol");
        
        bingkai1.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        
        JLabel lbKodeEmiten, lbNamaEmiten;
        
        JTextField txtKodeEmiten, txtNamaEmiten;
        
        JButton tbUbahNamaEmiten;
        
        lbKodeEmiten = new JLabel("Kode Emiten : ");
        
        lbNamaEmiten = new JLabel("Nama Emiten : ");
        
        txtKodeEmiten = new JTextField();
        
        txtNamaEmiten = new JTextField();
        
        lbNamaEmiten = new JLabel("Nama Emiten : ");
        
        tbUbahNamaEmiten = new JButton("Ubah Nama Emiten");
        
        lbKodeEmiten.setFont(new Font("Arial", Font.BOLD, 20));
        
        lbNamaEmiten.setFont(new Font("Arial", Font.BOLD, 20));
        
        tbUbahNamaEmiten.setFont(new Font("Arial", Font.BOLD, 20));
        
        txtKodeEmiten.setFont(new Font("Arial", Font.PLAIN, 20));
        
        txtNamaEmiten.setFont(new Font("Arial", Font.PLAIN, 20));
        
        lbKodeEmiten.setBounds(10, 10, 150, 30);
        
        lbNamaEmiten.setBounds(10, 50, 150, 30);
        
        txtKodeEmiten.setBounds(160, 10, 350, 30);
        
        txtNamaEmiten.setBounds(160,50,350,30);
        
        lbKodeEmiten.setForeground(new java.awt.Color(0,255,0));
        
        lbNamaEmiten.setForeground(new java.awt.Color(0,255,0));
        
        txtKodeEmiten.setEditable(true);
        
        txtNamaEmiten.setEditable(true);
        
        bingkai1.add(lbKodeEmiten);
        
        bingkai1.add(lbNamaEmiten);
        
        bingkai1.add(txtKodeEmiten);
        
        bingkai1.add(txtNamaEmiten);
        
        bingkai1.setSize(550,700);
        
        bingkai1.setLayout(null);
        
        bingkai1.getContentPane().setBackground(new java.awt.Color(0,0,0));
        
        bingkai1.setVisible(true);
        
    
    
    }
    
    
    public static void main(String[]args){
    
        membuatWindow();
    
    }
    
}



```










