# XCTest UI Test Example

## Scenario

User logs in with valid credentials.

## Test Flow

1. Launch the app
2. Tap the email field
3. Enter a valid email address
4. Tap the password field
5. Enter a valid password
6. Tap the login button
7. Verify that the home screen is displayed

## Example XCTest Code

```swift
func testSuccessfulLogin() {
    let app = XCUIApplication()
    app.launch()

    let emailField = app.textFields["emailTextField"]
    emailField.tap()
    emailField.typeText("test@example.com")

    let passwordField = app.secureTextFields["passwordTextField"]
    passwordField.tap()
    passwordField.typeText("Password123")

    app.buttons["loginButton"].tap()

    XCTAssertTrue(app.staticTexts["Home"].exists)
}

