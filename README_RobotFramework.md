# ⚡PIP4004_Internship

## 🚀Robert Framework

Robot Framework is an open source automation framework for test automation and robotic process automation (RPA). It is supported by the Robot Framework Foundation and widely used in the industry.

Its human-friendly and versatile syntax uses keywords and supports extending through libraries in Python, Java, and other languages.

It integrates with other tools for comprehensive automation without licensing fees, bolstered by a rich community with hundreds of 3rd party libraries.

---

## 📚 Robot Framework Style Documentation

### *** Settings ***

```
Documentation     ⚡PIP4004_Internship
...               🚀Robert Framework
...               Robot Framework is an open source automation framework for test automation and robotic process automation (RPA). It is supported by the Robot Framework Foundation and widely used in the industry.
...               Its human-friendly and versatile syntax uses keywords and supports extending through libraries in Python, Java, and other languages.
...               It integrates with other tools for comprehensive automation without licensing fees, bolstered by a rich community with hundreds of 3rd party libraries.
```

### *** Variables ***

```
${API_KEY}                Your_API_key_here
${ANOTHER_API_KEY}       Another_API_key_here
```

### *** Test Cases ***

```
Get All Items
    [Documentation]    Example for getting all items via API
    GET    /api/items    headers=Authorization=${API_KEY}

Get Single Item
    [Documentation]    Example for getting a specific item via ID
    GET    /api/items/${id}    headers=Authorization=${API_KEY}

Add Two Numbers
    [Documentation]    Takes two numbers and returns the sum
    ${result}=    Evaluate    ${num1} + ${num2}
    Log    ${result}

Login With Valid Credentials
    [Documentation]    Validates successful login with correct credentials
    Input Text    username_field    valid_user
    Input Text    password_field    correct_password
    Click Button    login_button
    Page Should Contain    Welcome

Verify Page Title
    [Documentation]    Checks the title of the homepage
    Title Should Be    Dashboard - Robot Test

Check Link Visibility
    [Documentation]    Confirms the presence of a link on the page
    Element Should Be Visible    xpath=//a[text()='Learn More']

Fill Contact Form
    [Documentation]    Fill and submit the contact form
    Input Text    name_field    John Doe
    Input Text    email_field   john@example.com
    Input Text    message_field Hello, this is a test.
    Click Button  send_button
    Page Should Contain    Thank you
```

### *** Keywords ***

```
Import Component Example
    [Documentation]    Usage example of importing a component
    Log    import Component from 'my-project'
    Log    function App() { return <Component /> }
```

### *** Metadata ***

```
Author    ⚡ [@aneeshk888](https://github.com/aneeshk888) 😎
License   MIT, GPLv3, AGPL
Docs      [Documentation](https://linktodocumentation)
Code of Conduct    Please adhere to this project's `code of conduct`
```

---

## API Reference

#### Get all items

```http
  GET /api/items
```

| Parameter | Type     | Description                |
| --------- | -------- | -------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| --------- | -------- | --------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

#### add(num1, num2)

Takes two numbers and returns the sum.

## Authors

⚡[@aneeshk888](https://github.com/aneeshk888)😎

## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)
