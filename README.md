# Get-current-time-hour-minute-second-AM-PM-
Get current time (hour :minute :second AM/PM)
*/

import java.util.*;

public class CurrentTime{
  public static void main(String[] args){
    Calendar calendar = new GregorianCalendar();
    String am_pm;
    int hour = calendar.get(Calendar.HOUR);
    int minute = calendar.get(Calendar.MINUTE);
    int second = calendar.get(Calendar.SECOND);
    if(calendar.get(Calendar.AM_PM) == 0)
      am_pm = "AM";
    else
      am_pm = "PM";
    System.out.println("Current Time : " + hour + ":" 
+ minute + ":" + second + " " + am_pm);
  }
}
/*
 * ////////////////////////////////////////////////////////////////////
 */
