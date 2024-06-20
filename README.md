# Netflix Login Feature Test Cases

## Overview

This document contains a set of test cases designed to verify the functionality of the Netflix login feature. The primary focus is on ensuring that users can successfully log in to Netflix using valid credentials and that the login page functions as expected under various conditions.

## Test Case Summary

- **Product Name:** Netflix
- **Module Name:** Login Page
- **Test Case Start Date:** 06/14/2024
- **Test Execution Date:** 06/15/2024
- **Pass:** 16
- **Fail:** 2
- **Total Test Cases:** 18
- **Test Case Developed By:** Rifat Bin Hossain
- **Test Executed By:** Rifat Bin Hossain
- **Developer Name:** Netflix Developer

## Test Cases

### TC001: Verify that the Netflix login page is loaded correctly

- **Test Data:** N/A
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
- **Expected Result:** User is able to access the login page
- **Actual Result:** As expected
- **Status:** Pass

### TC002: Verify user can enter email or phone number in the "Email Address or Phone Number" input field

- **Test Data:**
  - Email: `rifat@gmail.com`
  - Phone: `0088 01556566565`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Click the Email/Phone input field
- **Expected Result:** User can enter email or phone number in the input field
- **Actual Result:** As expected
- **Status:** Pass

### TC003: Verify user can enter password in the "Password" input field

- **Test Data:** Password: `lkjhmnb890`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Click the Password input field
- **Expected Result:** User can enter password in the input field
- **Actual Result:** As expected
- **Status:** Pass

### TC004: Verify user can click on 'sign in' button

- **Test Data:** N/A
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Click the Sign in button
- **Expected Result:** User can click on the 'sign in' button
- **Actual Result:** As expected
- **Status:** Pass

### TC005: Verify user gets country code when trying to log in using Phone

- **Test Data:** Phone: `01756521478`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Enter a valid phone number
- **Expected Result:** User automatically gets the country code when trying to log in using Phone
- **Actual Result:** As expected
- **Status:** Pass

### TC006: Verify that the user is successfully logged in with valid credentials and redirected to the Netflix home page

- **Test Data:**
  - Email: `rifat@gmail.com`
  - Password: `***********`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Enter a valid email in the email field
  3. Enter a valid password in the password field
  4. Click on the "Sign In" button
- **Expected Result:** User is successfully logged in with valid credentials and redirected to the Netflix home page
- **Actual Result:** As expected
- **Status:** Pass

### TC007: Verify if user clicks on login button without entering email/phone and password then system shows a valid error message

- **Test Data:** N/A
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Click Sign in button with empty email and password fields
- **Expected Result:** User gets a valid error message: "Please enter a valid email or phone number."
- **Actual Result:** As expected
- **Status:** Pass

### TC008: Verify if user clicks on login button with an invalid email then system shows a valid error message

- **Test Data:**
  - Email: `qwertyasd@qwe.xyz`
  - Password: `***********`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Enter an invalid email in the email field
  3. Enter a valid password in the password field
  4. Click on the "Sign In" button
- **Expected Result:** User gets a valid error message: "Please enter a valid email."
- **Actual Result:** As expected
- **Status:** Pass

### TC009: Verify if user clicks on login button with an invalid phone then system shows a valid error message

- **Test Data:**
  - Email: `+8800 015346`
  - Password: `***********`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Enter an invalid phone in the phone field
  3. Enter a valid password in the password field
  4. Click on the "Sign In" button
- **Expected Result:** User gets a valid error message: "Please enter a valid phone number."
- **Actual Result:** As expected
- **Status:** Pass

### TC010: Verify if user clicks on login button with an invalid password then system shows a valid error message

- **Test Data:**
  - Email: `rifat@gmail.com`
  - Password: `vsgd23gasf$#`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Enter a valid email/phone in the email field
  3. Enter an invalid password in the password field
  4. Click on the "Sign In" button
- **Expected Result:** User gets a valid error message: "Please enter a valid password."
- **Actual Result:** As expected
- **Status:** Pass

### TC011: Verify Password contains 4 to 60 characters

- **Test Data:** Password: `lkjhmnb890`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Enter a password between 4 to 60 characters
- **Expected Result:** User can input a password of 4 to 60 characters
- **Actual Result:** As expected
- **Status:** Pass

### TC012: Verify that passwords with more than 60 or fewer than 4 characters show a valid error message

- **Test Data:** Password: `2f4`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Enter a password that is not between 4 and 60 characters
- **Expected Result:** Shows a valid error message: "Your password must contain between 4 and 60 characters."
- **Actual Result:** As expected
- **Status:** Pass

### TC013: Verify that the "Use a Sign-in Code" button takes email/phone and verification code from user

- **Test Data:** Email: `rifat@gmail.com`
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Click the "Use a Sign-in Code" button
- **Expected Result:** User can input email/phone and verification code in the input field
- **Actual Result:** Not getting a verification code and gets an error message: "Something went wrong"
- **Status:** Fail

### TC014: Verify the "Forgot password?" link for password reset

- **Test Data:** N/A
- **Steps to Reproduce:**
  1. Go to [Netflix Login Page](https://www.netflix.com/login)
  2. Click on the "Forgot password?" link
- **Expected Result:** User is redirected to the password reset page
- **Actual Result:** As expected
- **Status:** Pass

### TC015: Verify that the "Remember me" checkbox saves the email/phone and on subsequent visits

- **Test Data:**
  - Email: `rifat@gmail.com`
  - Password: `***********`
- **Steps to Reproduce:**
  1. Navigate to [Netflix Login Page](https://www.netflix.com/login)
  2. Enter a valid email/phone and password
  3. Check the "Remember me" checkbox
  4. Click on the "Sign In" button and log out after a successful login
  5. Navigate back to [Netflix Login Page](https://www.netflix.com/login)
- **Expected Result:** The email/phone and password field is pre-filled with the previously entered email
- **Actual Result:** As expected
- **Status:** Pass

