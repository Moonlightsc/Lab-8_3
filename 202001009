// Boa class
package mypackage;



public class Boa {

	

	private String name;

	private int length; // the length of the boa, in feet

	private String favoriteFood;

	

	public Boa (String name, int length, String favoriteFood){

		

		this.name = name;

		this.length = length;

		this.favoriteFood = favoriteFood;

		

	}

	

	// returns true if this boa constrictor is healthy

	public boolean isHealthy(){

		

		return this.favoriteFood.equals("granola bars");

		

	}

	

	// returns true if the length of this boa constrictor is

	// less than the given cage length

	public boolean fitsInCage(int cageLength){

		

		return this.length < cageLength;

		

	}

	

	// produces the length of the Boa in inches

	public int lengthInInches(){

		

		int LengthInches=this.length*12;

		

		return LengthInches;

		

	}

}

// Test class 

package mypackage;

import static org.junit.Assert.*;

import org.junit.Before;
import org.junit.Test;

public class BoaTest {
	
	private Boa jen;
	private Boa ken;
	
	@Before
	public void setUp() throws Exception {
		// initialization
		jen = new Boa("Jennifer", 2, "grapes");
		ken = new Boa ("Kenneth", 3, "granola bars");
	}

	@Test
	public void testIsHealthy() {
		
		// testing isHealthy for two objects
		assertEquals(false,jen.isHealthy());
				
		assertEquals(true,ken.isHealthy());
	}
	
	@Test
	public void testFitsInCage()
	{
		
		assertEquals(false,jen.fitsInCage(1)); // less than cage size
		
		assertEquals(false,jen.fitsInCage(2)); // equal to cage size
		
		assertEquals(true,jen.fitsInCage(3));  // greater than cage size
		
	}
	
	@Test
	public void testlengthInInches()
	{
		assertEquals(24,jen.lengthInInches());
		assertEquals(36,ken.lengthInInches());
	}

}
