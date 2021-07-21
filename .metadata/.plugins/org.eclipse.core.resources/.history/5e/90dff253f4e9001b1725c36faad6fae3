package org.facebook;



import java.util.Date;

import org.junit.Before;
import org.openqa.selenium.Keys;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.edge.EdgeDriver;
import org.openqa.selenium.support.PageFactory;
import org.testng.annotations.Test;
import org.testng.asserts.SoftAssert;

public class login {

	public static WebDriver browser ;
	public static WebElement email;
	public static WebElement pass;

	@Test(priority = 1,groups = "SmokeTest")
	public static void getfbpage() {		
		System.setProperty("webdriver.edge.driver", 
				"D:\\MyJavaSeleniumProject\\Facebook\\src\\test\\resources\\Driver\\msedgedriver.exe");
		browser =new EdgeDriver();
		browser.get("https://en-gb.facebook.com/");
	}

	@Test(priority = 2,groups = "SmokeTest")
	public static void getfbLogin() {
		PageFactory.initElements(browser, login.class);
		SoftAssert as = new SoftAssert();
		email.sendKeys("Hello");
		boolean userChk = email.getAttribute("value").contains("Hell");
		as.assertTrue(userChk, "UserName validation");
		pass.sendKeys("hello",Keys.ENTER);
		as.assertAll();
	}

	@Test(priority = 3,groups = {"reg"})
	public static void getfbLogin1() {
		PageFactory.initElements(browser, login.class);
		SoftAssert as = new SoftAssert();
		email.sendKeys("Hello");
		boolean userChk = email.getAttribute("value").contains("Hell");
		as.assertTrue(userChk, "UserName validation");
		pass.sendKeys("hello",Keys.ENTER);
		as.assertAll();
	}
	@Test(priority = 4,groups = {"SmokeTest"})
	public static void printstat()
	{	
		Date dt =new Date();
		System.out.println("Test passed at : " +dt.toString());
	}

}
