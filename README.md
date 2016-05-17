# zuoye8
package sanjiaoxing;

import static org.junit.Assert.*;

import org.junit.Test;

public class TriangleTest {

	@Test
	
public void testIsTriangle1(){
    Triangle t = new Triangle(3,4,5);
    assertFalse(t.isTriangle(t));
}

@Test
public void testIsTriangle2(){
    // according to the mutant, this test case should fail
    Triangle t = new Triangle(2,3,4);
    assertFalse(t.isTriangle(t));
}

@Test
public void testIsTriangle3(){
    Triangle t = new Triangle(1,2,3);
    assertFalse(t.isTriangle(t));
}
public void testIsTriangle4(){
    Triangle t = new Triangle(8,10,8);
    assertFalse(t.isTriangle(t));
}

@Test
public void testIsTriangle5(){
    // according to the mutant, this test case should fail
    Triangle t = new Triangle(0,0,0);
    assertFalse(t.isTriangle(t));
}

@Test
public void testIsTriangle6(){
    Triangle t = new Triangle(3,3,3);
    assertFalse(t.isTriangle(t));
}
@Test
public void testIsTriangle7(){
    Triangle t = new Triangle(-1,5,4);
    assertFalse(t.isTriangle(t));
}
}
