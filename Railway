package railway;
import java.util.Scanner;
public class Railway {

	public static void main(String[] args) {
		String[] dep_time ={"Mon\t6:04", "Mon\t9:04", "Mon\t12:04", "Mon\t15:04", "Mon\t19:04", "Tue\t6:04", "Tue\t9:04", "Tue\t12:04", "Tue\t15:04", "Tue\t19:04", "Wed\t6:04", "Wed\t9:04", "Wed\t12:04", "Wed\t15:04", "Wed\t19:04"};
        int[] pass_nums = { 22,119,64,177,21,22,111,87,193,22,11,107,93,162,42};
        Scanner rail = new Scanner(System.in);
         while(true)
        {
        	System.out.println("Enter your choice");
            System.out.println("1. Display the information of all trains\n2. Find the most popular train\n3. Find the least popular train\n4. Compare the popularity of 6:04 train and 9:04 train\n5. Compare the popularity of 6:04 train on Monday and Tuesday\n6. Compare the popularity of any two trains of your choice\n7. Display the list of trains with passengers below 50\n8. Calculate the average number of passengers on 12:04 train\n9.Display the number of passengers on any train of your choice\n10. Quit");
            int choice = rail.nextInt();
            switch(choice)
            {
            case 1:
            	{System.out.println("Day\tDeparture Time\tNumber of passengers");
                for (int i=0;i<dep_time.length;i++)
                    System.out.println(dep_time[i]+"\t\t"+pass_nums[i]);
                break;}
                
            case 2:
            	{int mptrain = pass_nums[0];
                String popular = dep_time[0];
                for (int i=0; i<dep_time.length; i++){
                    if (pass_nums[i]>mptrain){
                        mptrain = pass_nums[i];
                        popular = dep_time[i];}}
                 System.out.println("The most popular train is running at "+popular+" with "+mptrain+" number of passengers");
                 break;}   
               
            
            case 3:     
            {
                int lptrain = pass_nums[0];
                String least = dep_time[0];
                for (int i=0; i<dep_time.length; i++){
                    if (pass_nums[i]<lptrain){
                        lptrain = pass_nums[i];
                        least = dep_time[i];
                    }
                }
                System.out.println("The least popular train is running at "+least+" with "+lptrain+" number of passengers");
                break;} 
            
            case 4:
            {
                if(pass_nums[0]>pass_nums[1])
                    System.out.println("Train 6:04 is more popular than Train 9:04 on Monday");
                else
                    System.out.println("Train 6:04 is less popular than Train 9:04 on Monday");
                if(pass_nums[5]>pass_nums[6])
                    System.out.println("Train 6:04 is more popular than Train 9:04 on Tuesday");
                else
                    System.out.println("Train 6:04 is less popular than Train 9:04 on Tuesday");
                if(pass_nums[10]>pass_nums[11])
                    System.out.println("Train 6:04 is more popular than Train 9:04 on Wednesday");
                else
                    System.out.println("Train 6:04 is less popular than Train 9:04 on Wednesday");
                
            break;}
            
            case 5:
            {
                if (pass_nums[0]>pass_nums[5])
                    System.out.println("6:04 Train is more popular on Monday than Tuesday");
                else if (pass_nums[0]<pass_nums[5]) 
                    System.out.println("6:04 Train is more popular on Tuesday than Monday");
                else
                    System.out.println("6:04 Train is equally popular on Monday and Tuesday");
                break;}
            
            case 6:
            {
                System.out.println("Enter the serial numbers of two trains to be compared");
                System.out.println("S.No.\tDay\tDeparture Time");
                for (int i=0;i<dep_time.length;i++)
                    System.out.println(i+"\t"+dep_time[i]);
                int k=rail.nextInt();
                int d=rail.nextInt();
                if (pass_nums[k]>pass_nums[d])
                    System.out.println(dep_time[k]+" is more popular");
                else if (pass_nums[k]<pass_nums[d])
                    System.out.println(dep_time[d]+" is more popular");
                else
                    System.out.println("Both trains are equally popular");
                break;}
            
            case 7:
            {
                System.out.println("The list of trains with below 50 passengers");
                System.out.println("Day\tDeparture Time\tNumber of passengers");
                for (int i=0; i<dep_time.length; i++){
                    if (pass_nums[i]<50){
                        System.out.println(dep_time[i]+"\t\t"+pass_nums[i]);
                    break;}
                   }
               break; }
            
            case 8:
            {
                System.out.println("The average number of passengers on 12:04 trains is "+((pass_nums[2]+pass_nums[7]+pass_nums[12])/3.0));
                break;}
            
            case 9:
            {
                System.out.println("薾ter the serial number of train for which the number of passengers info is needed");
                System.out.println("S. No.\tDay\tDeparture Time");
                for (int i=0;i<dep_time.length;i++)
                    System.out.println(i+"\t"+dep_time[i]);
                int z = rail.nextInt();
                System.out.println("The number of passengers travel on "+dep_time[z]+" is "+pass_nums[z]);
                break;}
            
            case 10:
            	System.exit(0);
            	break;
            }

	}

}}
