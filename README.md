# Nxt Trendz App with Protected Route

In this project, I have implemented the **Nxt Trendz** app with a Protected Route, applying the concepts learned so far.

### Refer to the image below:

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-protected-route-output.gif" alt="nxt-trendz-protected-route-desktop-output" style="max-width:90%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

### Design Files

<details>
<summary>Click to view</summary>

- [Extra Small (Size < 576px), Small (Size >= 576px), and Medium (Size >= 768px) - Login, Login Error, Home](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-authentication-sm-outputs.png)
- [Extra Small (Size < 576px), Small (Size >= 576px), and Medium (Size >= 768px) - Products, Cart](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-authentication-sm-products-cart-outputs.png)
- [Large (Size >= 992px) and Extra Large (Size >= 1200px) - Login](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-authentication-lg-login-output.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px) - Home](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-authentication-lg-home-output.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px) - Products](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-authorisation-lg-products-output.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px) - Cart](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-authorisation-lg-cart-output.png)

</details>

### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

<details>
<summary>Functionality to be added</summary>
<br/>

The app must have the following functionalities:

- When an unauthenticated user tries to access the Home Route, Products Route, or Cart Route, the page should navigate to the Login Route using the protected route.
- When an authenticated user tries to access the Home Route, Products Route, or Cart Route, the page should navigate to the respective route using the protected route.

</details>

<details>

<summary>API Requests & Responses</summary>
<br/>

**loginApiUrl**

#### API: `https://apis.ccbp.in/login`

#### Method: `POST`

#### Description:

Returns a response based on the credentials provided.

#### Sample Success Response

```json
{
  "jwt_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6InJhaHVsIiwicm9sZSI6IlBSSU1FX1VTRVIiLCJpYXQiOjE2MTk2Mjg2MTN9.nZDlFsnSWArLKKeF0QbmdVfLgzUbx1BGJsqa2kc_21Y"
}
```

#### Sample Failure Response

```json
{
  "status_code": 404,
  "error_msg": "Username is not found"
}
```

</details>

<details>
<summary>Components Structure</summary>

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-authentication-login-home-component-structure-breakdown.png" alt="nxt trendz authentication login and home component structure breakdown" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-authentication-products-cart-component-structure-breakdown.png" alt="nxt trendz authentication products and cart component structure breakdown" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>
</details>

<details>
<summary>Implementation Files</summary>
<br/>

Use these files to complete the implementation:

- `src/App.js`
- `src/components/ProtectedRoute/index.js`
</details>
