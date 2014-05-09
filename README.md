ArtPricingSystem
================
package artpricingsystem;

import java.io.File;
import java.io.RandomAccessFile;

public class ArtPricingSystem {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
       BoughtPainting p1=new BoughtPainting();
       p1.print();
       p1.readInRecord();
       p1.performDeletion();
       
       
       
      /* 
       ----------------------------save testing------------------------------
       File paintingsFile = new File ("GalleryPaintings.dat");     
       try {
       RandomAccessFile oldFile = new RandomAccessFile (paintingsFile, "r");  
       p1.read(oldFile);
       p1.print();
       System.out.println(p1.find("Marget", "Universal Judge"));
       p1.save();
       }
       
       catch (Exception e)
      {
          System.out.println ("***** Error: BoughtPainting.putRecord () *****");
          System.out.println ("\t" + e);
      }/*

        
       
       ---------------------testing artist crap--------------------------------
        /*Artist art=new Artist("Claude", "Monet", 500); //if artist already exists, this won't replace the old one in the save yet
        Artist art2=new Artist("Tiger", "Woods", 770);
        art.updateArtistLastName();
        art.print();
        art2.print();
        art2.save();
        art.save(); */
    }
    
}
