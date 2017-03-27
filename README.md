//# GradeActivity
//calculate grade with java
// Hikmet Demir java project 
//calculating grade 
package gradebook;
import java.text.DecimalFormat;
import javax.swing.JOptionPane; 
public class GradeActivity {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		//Using JOptionPane to take input from the user.
		double test1= 0 ;
		double test2 = 0;
		double test3 = 0;
		double test4 = 0;
		double test5= 0;
		
		
				
		String Tname=JOptionPane.showInputDialog( "Hi. Please Enter your name: ");
				JOptionPane.showMessageDialog(null, "Hi, "+Tname.toUpperCase()+".");
				String Sname= JOptionPane.showInputDialog("Please Enter Name of your Student: ");
				String itest1=JOptionPane.showInputDialog("Please Enter The First Test Score: ");
				double Test1=Double.parseDouble(itest1);
				String itest2=JOptionPane.showInputDialog("Please Enter The Second Test Score: ");
				double Test2=Double.parseDouble(itest2);
				String itest3=JOptionPane.showInputDialog("Please Enter The Third Test Score: ");
				double Test3=Double.parseDouble(itest3);
				String itest4=JOptionPane.showInputDialog("Please Enter The Fourth Test Score: ");
				double Test4=Double.parseDouble(itest4);
				String itest5=JOptionPane.showInputDialog("Please Enter The Fifth Test Score: ");
				double Test5=Double.parseDouble(itest5);
		
				double Average=(test1+test2+test3+test4+test5)/5; //Calculating Average
			

	      // Display the formatted variable contents.
	      char grade= 'T' ; //declaring character variable.
			
			
			if (Average>=90 && Average<=100){
				JOptionPane.showInputDialog(Average, "You've got A");
			}
			else if (Average>=80 && Average<90){
				JOptionPane.showInputDialog(Average, "You've got B");
			}
			else if (Average>=70 && Average<80){
				JOptionPane.showInputDialog(Average, "You've got C");
			}
				else if (Average>=60 && Average<70){
					JOptionPane.showInputDialog(Average, "You've got D");
				
				}
				else if (Average>=0 && Average<60){
					JOptionPane.showInputDialog(Average, "You've got F");
				}
				else {
					System.out.println("Sorry, please try again :).");
					System.exit(0); //To exist the code if something goes wrong.
					}
	     
	      
	}

}

