# **Triple-Decky**

## New triple deck filament block for ERCF V1, Sturdy Bunny and ERCF V2.

## I add the Rev C for 3 positions servo STLs. Make sure to read the note below first if you want to use it !!!

Triple Decky is a replacement for the filament block on ERCF V1 and Sturdy Bunny. Its goal is to avoid the filament to move in or out the filament block while loading or unloading another gate.

To do that, the filament block consist in 2 hinged parts (decks), that are kept apart by magnets. The filament is lifted by 1 mm from the bottom BMG gear.

The tophat comes on top of the 2nd deck and has the top BMG gear as before. 

Although the current Rev B version still has the possibility to install the magnetic gate, it is normally not needed anymore.

**I have re-structure this GitHub to show only the latest versions of each type. All previous STLs are available in the Archives folder.**

## **In Beta testing :**
* **Version C.** 
  *  It will have a kind of brake to press against the filament when the gate is not selected. The exit side of the filament path can lift up about 0.5 mm, enough to make the filament touching the brake part (trap). To release the brake it will use either :
     *  with a magnet that will be pushed back by the encoder magnet.
     *  by using a special tophat that will need a 3rd position of the servo to be able to move the selector. (not available yet : software in development)<p>
  * The brake part will be easily replaceable in case it breaks.
  *  The multicolor tag plates will be the same for input and output side. (Same as in version B4 Base)<p>
  *  The use of the old magnetic gates will be impossible on that version.
  *  If you are using Happy Hare software, you should decrease the "parking_distance" in the ercf_parameters to about 15 so the filament parks inside the trap.<p>
## **Yet in development :**
* **ERCF V2 :** at this moment, ERCF V2 is in development by a team of designers. Lots of things have been developed and are tested, but regarding the filament blocks, no decision have been taken on which version of Triple Decky or another type will be used.
  * Mods in progress :
    * Sturdy Bunny: https://github.com/sneakytreesnake/SturdyBunnyProject
    * Springy: https://github.com/moggieuk/ERCF-Springy/tree/main
    * Ejection Assisted Purge: https://github.com/bombela/EjectionAssistedPurge
    * Binky: https://github.com/mneuhaus/EnragedRabbitProject/tree/main/usermods/Binky
    * and much more...
   

## **Actual versions**

### At this moment, there are 4 versions of Triple-Decky.

*  ## For Sturdy Bunny build on a 2020 extrusion. 
    * ### **Triple Decky for Sturdy Bunny Rev C6 magnet brake release or 3 positions servo.**
  
      * **This is an update from Rev C5 that fixes the following issues: (use it with caution)**
        * wall around the bearing cracks
        * filament path output side rubbing on the encoder and get pushed down. 
      * **It has the following new feature :**
        * thicker wall around the bearing
        * output face of the filament path is tilted 4° to avoid rubbing on the encoder cart
        * new tophat to match the brake release magnet new position
        <center><img src="Images/C6-bearing.JPG" width="250" alt="C6 bearing"> <img src="Images/C6-backside.JPG" width="250" alt="C6 output face"></center>

        * **Warning:**
          * C6_x base need to have C6_x filament path
          * C6_x filament path need to have C6_x tophat
          * C5_x base is compatible with C6_x filament path
          * C5_x filament path is compatible with C6_x tophat
          * For all Rev C, only the integrated tophat are available, and needs the Springy servo holder to work. (see above in mods in progress) <p>
      <p>
           
      
      
    * ### **Triple Decky for Sturdy Bunny Rev C6 for 3 positions servo brake release. "3PS"**
      * #### **<u>IMPORTANT NOTE ABOUT THE 3PS VERSION.</u>**
          * **If you want to test the C6 with 3 positions servo YOU HAVE TO install the latest Happy-Hare software (HHv2) that support the servo 3rd position. Otherwise IT WILL NOT WORK. It is in beta for a few people at this moment. If you are one of those beta tester, you can try this Triple Decky C6 3PS. If not, wait until it is fully released. The actual KlipperScreen for Happy Hare needs also a special updated version.**
          * The base is the same for both Rev C versions (Triple_Decky_Base_C6_0.stl).
          * The taps are the same for both Rev C versions (Traps folder).
          * If you are already using the magnet version, you can still use it if you print the universal tophat ([a]Triple_Decky_Tophat-integerated_Universal_Mag&3PS_C6_0.stl). **DO NOT USE THIS STL IF YOU DO NOT HAVE ENABLED THE 3rd POSITIONS FOR SERVO IN YOUR SOFTWARE!!!**
          * If this is your first use of Rev C 3PS, then it is better to use the dedicated tophat for 3PS ([a]Triple_Decky_Tophat-integerated_3PS_C6_2.stl).
          * Optionaly you may want to use the special servo arm with rounded edges (Servo Arm MG90S_for_3PS.stl) (currently only available for MG90S).
          * **Software parameters** 
            * Add "servo_move_angle: (move position angle)" in mmu_parameters.cfg
              * In my case I have :
                * servo_move_angle: 45
                * servo_up_angle: 24
                * servo_down_angle: 115
            * Change the "encoder_parking_distance:" in mmu_parameters.cfg so the filament parks in the trap. (for me I change it to 15, it was 23) 
            <p>
      
      

       <center><img src="Images/C6-3PS-in.JPG" width="250" alt="C5 in"> <img src="Images/C6-3PS-out.JPG" width="250" alt="C5 out"></center><p>
       <center><img src="Images/C6-3PS-cut.JPG" height="200" alt="C5 cutout"> <img src="Images/C6-3PS-trap.JPG" height="200" alt="C5 trap"><center>


    * ### **Triple Decky for Sturdy Bunny Rev C6 magnet brake release** 
      * In beta testing.
      

       <center><img src="Images/C5-in.JPG" width="250" alt="C5 in"> <img src="Images/C5-out.JPG" width="250" alt="C5 out"></center><p>
       <center><img src="Images/C5-cut.JPG" height="200" alt="C5 cutout"> <img src="Images/C5-trap.JPG" height="200" alt="C5 trap"><center>


    * ### **Triple Decky for Sturdy Bunny Rev. B (previously B4)**
      * The output side of the filament path has been tilted by 4° to avoid rubbing on the encoder when the selector is moving.
      * The input side tag plate is rotated 90° for better printing without support.
      * New multicolor tag plates for 12 carts on the input side.
      * New multicolor gate plates for 12 carts on the output side to replace the magnetic gate. 
      * New integrated tophat based on number 1 tophat locker to be used with Springy [from Moggieuk](https://github.com/moggieuk/ERCF-Springy/tree/main)  
      * optional base to use the old magnetic gates. In that case, the small part of the hinge of the filament path must be cut at the mark.
      * The latch has an optional set screw to apply a little bit of friction on the filament. This help the filament to stay still in case of vibrations.<p>
  
    <center><img src="Images/B4-in.JPG" width="250" alt="Triple Decky for Sturdy Bunny"> <img src="Images/B4-out.JPG" width="250" alt="Triple Decky for Sturdy Bunny"> <img src="Images/B4-side.JPG" width="250" alt="Triple Decky for Sturdy Bunny"></center>
           
    * ### Triple Decky for Sturdy Bunny Rev. B2 / B3 (Can be found in the Archives folder)
      This is the fisrt release 
    <center><img src="Images/TD%20for%20Sturdy-Bunny.JPG" width="250" alt="Triple Decky for Sturdy Bunny"></center>




 *  ## For ERCF V1 / V1.1
   This is for the original design that is build with M5 all threaded rod. This version will not be developed further because almost all users / builders are moving to Sturdy Bunny, or the coming (soon) ERCF V2. 
   <p>
        <center><img src="Images/TD%20for%20ERCF-V1.JPG" width="250" alt="Triple Decky for ERCF V1"></center>


   
