package com.test;

import java.text.DateFormat;
import java.text.ParseException;
import java.text.SimpleDateFormat;
import java.util.Calendar;
import java.util.Date;

public class DateAndTimeComparision {

	public static void main(String[] args) throws ParseException {

		DateFormat testDateFormat = new SimpleDateFormat("yyyy/MM/dd HH:mm:ss");

		// String testDate = "2014/10/29 23:10:45";
		// String testDate = "2014/10/30 18:10:45";
		String testDate = "2018/08/28 18:10:45";
		Date dateObj = testDateFormat.parse(testDate);

		Calendar calendarObj = Calendar.getInstance();
		calendarObj.setTime(dateObj);
		System.out.println("=================" + testDateFormat.format(calendarObj.getTime()));

		calendarObj.add(Calendar.HOUR, 1);
		calendarObj.add(Calendar.MINUTE, 30);

		System.out.println("=================" + testDateFormat.format(calendarObj.getTime()));

		Long timeInMillisAfterModification = calendarObj.getTimeInMillis();
		System.out.println("======== time in millis after adding 150mins === " + timeInMillisAfterModification);

		// Current Time In Millis
		Long currentTimeInMillis = Calendar.getInstance().getTimeInMillis();

		System.out.println("========= Current Time in Millis ===== " + currentTimeInMillis);
		if (currentTimeInMillis > timeInMillisAfterModification) {

			System.out.println("======== Condition Passed ====");

		} else {

			System.out.println("======== Condition Failed ====");
		}

	}
}
