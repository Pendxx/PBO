import static org.junit.Assert.*;
import org.junit.After;
import org.junit.Before;
import org.junit.Test;

public class CalcEngineTest
{
    private CalcEngine engine;

    @Before
    public void setUp()
    {
        engine = new CalcEngine();
    }

    @After
    public void tearDown()
    {
    }

    @Test
    public void testPlus()
    {
        engine.numberPressed(3);
        engine.plus();
        engine.numberPressed(4);
        engine.equals();
        assertEquals(7, engine.getDisplayValue());
    }

    @Test
    public void testMinus()
    {
        engine.numberPressed(9);
        engine.minus();
        engine.numberPressed(4);
        engine.equals();
        assertEquals(5, engine.getDisplayValue());
    }

    @Test
    public void testMultiDigit()
    {
        engine.numberPressed(1);
        engine.numberPressed(2);
        assertEquals(12, engine.getDisplayValue());
    }
}
