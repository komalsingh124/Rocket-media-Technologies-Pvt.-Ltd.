import java.util.HashMap;
import java.util.Iterator;
import java.util.Set;

public class DemoDummy 
{
	public static void main(String[] args) 
	{
		int a[]={10,10,10,10,20,30,30,30,30,30,30,30,40,40,40,40,40};
		HashMap hm=new HashMap();
		for(int i=0;ia.length;i++)
		{
			int count=0;
			for(int j=0;ja.length;j++)
			{
				if(a[i]==a[j])
				{
					count++;
				}
			}
			hm.put(a[i], (count2));
		}
		System.out.println(hm);
		Set set=hm.keySet();
		System.out.println(set);
		Integer sum=0;
		Iterator itr=set.iterator();
		while(itr.hasNext())
		{
			sum=sum+(Integer)hm.get(itr.next());
		}
		System.out.println(sum);

	}

}
