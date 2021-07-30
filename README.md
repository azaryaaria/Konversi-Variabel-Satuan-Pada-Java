# Casting Data Pada Java 1
Memperbesar dan memperkecil range suatu variabel angka satuan


package com.tutorial;

public class Main {

    public static void main(String[] args){

        long x = 302L;
        int alfath = 120;
        short y = 102;
        byte z = 127;

        int hasil = (int)(x + alfath);
        System.out.println(hasil);

        System.out.println(x + " = ini adalah variabel long");
        System.out.println("Nilai max long : " + Long.MAX_VALUE);
        System.out.println("Nilai min long : " + Long.MIN_VALUE);
        System.out.println("Nilai bit long : " + Long.SIZE);
        System.out.println("Nilai byte long : " + Long.BYTES);

        System.out.println("\n");

        System.out.println(alfath + " = ini adalah variabel int");
        System.out.println("Nilai max integer : " + Integer.MAX_VALUE);
        System.out.println("Nilai min integer : " + Integer.MIN_VALUE);
        System.out.println("Nilai bit integer : " + Integer.SIZE);
        System.out.println("Nilai byte integer : " + Integer.BYTES);

        System.out.println("\n");

        System.out.println(y + " = ini adalah variabel short");
        System.out.println("Nilai max short : " + Short.MAX_VALUE);
        System.out.println("Nilai min short : " + Short.MIN_VALUE);
        System.out.println("Nilai bit short : " + Short.SIZE);
        System.out.println("Nilai byte short : " + Short.BYTES);

        System.out.println("\n");

        System.out.println(z + " = ini adalah variabel byte");
        System.out.println("Nilai max byte : " + Byte.MAX_VALUE);
        System.out.println("Nilai min byte : " + Byte.MIN_VALUE);
        System.out.println("Nilai bit byte : " + Byte.SIZE);
        System.out.println("Nilai byte byte : " + Byte.BYTES);

        System.out.println("==================================Casting Tipe Data====================================");

        //cara mengubah tipe data berjenis satuan
        //bisa memperluas atau memperkecil rentang variabel

        //dari yang kecil mau diperbesar
        int NilaiInt = 260;
        System.out.println("NilaiInt bernilai = " + NilaiInt);
        System.out.println("Nilai max NilaiInt = " + Integer.MAX_VALUE);

        System.out.println("sekarang diperbesar nilai max nya dengan casting ke tipe data long yang nilai max nya lebih besar");

        long NilaiLong = NilaiInt;
        System.out.println("NilaiInt yang sudah diperluas bernilai = " + NilaiLong);
        System.out.println("Nilai max NilaiInt sekarang = " + Long.MAX_VALUE);

        //dari yang besar mau diperkecil
        long NilaiLong2 = 320;
        System.out.println("\nNilaiLong bernilai = " + NilaiLong);
        System.out.println("Nilai max NilaiLong = " + Long.MAX_VALUE);

        System.out.println("sekarang diperkecil nilai max nya dengan casting ke tipe data long yang nilai max nya lebih kecil");

        byte NilaiByte = (byte) NilaiLong;
        System.out.println("NilaiLong yang sudah diperkecil bernilai = " + NilaiByte);
        System.out.println("Nilai max NilaiLong sekarang = " + Byte.MAX_VALUE);
        System.out.println("Sekarang NilaiLong akan mempunyai range nilai yang sama dengan ");


    }

}

