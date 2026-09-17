# Razorpay Payment Plugin for nopCommerce

A secure and easy-to-integrate Razorpay payment gateway plugin for nopCommerce. This plugin allows your customers to pay using a variety of methods including Credit/Debit Cards, NetBanking, UPI, and Wallets.

## Features

- **Wide Range of Payment Options**: Supports all payment methods offered by Razorpay (Cards, NetBanking, UPI, Wallets).
- **Refund Support**: Supports both full and partial refunds directly from the nopCommerce administration area.
- **Customizable Fees**: Ability to add an additional handling fee to orders, configurable as either a fixed amount or a percentage of the total.
- **Seamless Integration**: Uses a redirection-based payment flow for a secure checkout experience.
- **Modern Tech Stack**: Built for nopCommerce 5.00 and .NET 10.

## Prerequisites

Before installing the plugin, ensure you have:
- A valid [Razorpay](https://razorpay.com/) account.
- Your Razorpay **Key ID** and **Key Secret** from the Razorpay Dashboard.
- A nopCommerce 5.00 installation.

## Installation

1. **Download/Build the Plugin**: Obtain the compiled DLLs and resources of the plugin.
2. **Deploy to nopCommerce**:
   - Copy the `Nop.Plugin.Payments.RazorpayPayment` folder to the `plugins` directory of your nopCommerce installation.
3. **Restart Application**: Restart your web server or application pool to ensure the plugin is detected.
4. **Install from Admin**:
   - Log in to the nopCommerce administration area.
   - Navigate to **Configuration** $\rightarrow$ **Local Plugins**.
   - Find **Razorpay** in the list and click the **Install** button.

## Configuration

Once installed, you can configure the plugin by navigating to **Configuration** $\rightarrow$ **Payment Methods** $\rightarrow$ **Razorpay**.

| Setting | Description |
| :--- | :--- |
| **Key ID** | Your Razorpay API Key ID. |
| **Key Secret** | Your Razorpay API Key Secret. |
| **Additional Fee** | An optional fee to charge customers on top of the order total. |
| **Additional Fee Percentage** | Enable this to treat the additional fee as a percentage; otherwise, it is treated as a fixed value. |

## Managing Refunds

This plugin supports the native nopCommerce refund workflow:
- Navigate to the **Order Details** page in the admin area.
- Use the **Refund** option to initiate a full or partial refund.
- The plugin communicates with the Razorpay API to process the refund and returns the result to nopCommerce.

## Technical Details

- **Supported Versions**: nopCommerce 5.00
- **Framework**: .NET 10
- **Payment Method Type**: Redirection

---
*Developed by [Pankaj Dobariya]*
