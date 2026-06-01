# Smart-Pro-Social-Engineering-phishtoolkit-
Phishing is a common form of social engineering in which an attacker creates a convincing imitation of a legitimate website or login page to trick users into revealing credentials. However, more advanced phishing campaigns go beyond simple website cloning and focus heavily on psychological manipulation and trust exploitation.
Modern users are generally aware of basic phishing attempts and are often cautious about clicking suspicious links or messages from unknown sources. To overcome this awareness, attackers may first build a highly credible identity by impersonating a legitimate company, brand, or organization. This can involve professional-looking email addresses, branded profiles, realistic communication styles, and other elements designed to create the appearance of authority and trustworthiness.

Once this trusted image is established, messages or emails are sent to potential targets. Because the communication appears to originate from a recognized organization, victims may be more likely to trust it. A key aspect of these campaigns is the use of realistic user interface (UI) design. By closely replicating the visual appearance of legitimate platforms—including logos, email layouts, usernames, and message formatting—the content can appear authentic at first glance.

Another common technique is the use of hyperlink buttons rather than exposing raw URLs directly. Similar to legitimate emails from major online services, clickable text such as “Reset Your Password” or “Secure Your Account” may conceal the underlying destination link. The visible text appears harmless while the actual URL remains hidden behind the button.

These methods rely heavily on social engineering, where the success of the attack depends on influencing human behavior and decision-making rather than exploiting technical vulnerabilities alone. Because they target trust, perception, and psychology, social engineering techniques have remained one of the most effective components of cyberattacks.

The demonstration described here was built manually using Node.js, JavaScript, and HTML to illustrate how realistic interfaces and communication patterns can influence user trust and awareness in cybersecurity scenarios.


## 𝗥𝗲𝗾𝘂𝗶𝗿𝗲𝗱 𝗜𝗻𝘀𝘁𝗮𝗹𝗹𝗮𝘁𝗶𝗼𝗻 𝗳𝗼𝗿 𝘁𝗵𝗶𝘀 𝗽𝗿𝗼𝗷𝗲𝗰𝘁 : Node.js + Nodemailer + Python 3.12+ <npm init -y npm install nodemailer> #if not installed


### 𝙁𝙤𝙧 Google 𝙢𝙖𝙞𝙡 📧📥 :-
1️⃣ nano[GUI_FILE].js
2️⃣ paste this below 👇🏻 codes and change/replace your Gmail address, User's Gmail address, Your Gmail app passkey & the email part whatever you want to write ✍🏻.

## Paste the script 📃
const nodemailer = require("nodemailer");

// Gmail SMTP setup
const transporter = nodemailer.createTransport({
  service: "gmail",
  auth: {
    user: "YOUR_EMAIL@gmail.com",
    pass: "PASTE_CRRATED_PASSKEY_FROM_GMAILAPP"
  }
});

// 🎨 Clean, minimal email UI (no brand impersonation)
const htmlContent = `
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>

<body style="margin:0; padding:0; background:#f1f3f4; font-family:Arial, sans-serif;">

  <table width="100%" cellpadding="0" cellspacing="0" style="padding:40px 0;">
    <tr>
      <td align="center">

        <table width="100%" cellpadding="0" cellspacing="0"
               style="max-width:520px; background:#ffffff; border-radius:10px; overflow:hidden;">

          <!-- HEADER -->
          <tr>
            <td style="padding:20px 24px; border-bottom:1px solid #e0e0e0;">
              <div style="font-size:16px; font-weight:600; color:#202124;">
                 ⚠️ Suspicious Login Blocked 🚫
              </div>
            </td>
          </tr>

          <!-- LOGO -->
          <tr>
            <td align="center" style="padding-top:30px;">
              <img src="https://images.seeklogo.com/logo-png/27/1/google-logo-png_seeklogo-273192.png"
                   width="60"
                   height="60"
                   alt="Google Logo"
                   style="display:block; border-radius:12px;">
            </td>
          </tr>

          <!-- HEADLINE -->
          <tr>
            <td style="padding:24px 24px 8px 24px;">
              <h2 style="margin:0; font-size:20px; color:#202124;">
                ⚠️ Abnormal Activity Detected
              </h2>
            </td>
          </tr>

          <!-- BODY -->
          <tr>
            <td style="padding:8px 24px 0 24px; font-size:14px; color:#444; line-height:1.6;">
                We have detected Brute Force attack in your account.We think someone is trying to login to your account and we have blocked >
            </td>
          </tr>

          <!-- BUTTON -->
          <tr>
            <td style="padding:24px;">
              <a href="https://exampledomain.com"
                 style="background:#1a73e8;
                        color:#ffffff;
                        padding:12px 24px;
                        text-decoration:none;
                        border-radius:4px;
                        font-weight:600;
                        font-size:14px;
                        display:inline-block;">
                Check account activity
              </a>
            </td>
          </tr>

          <!-- FOOTER -->
          <tr>
            <td style="padding:16px 24px; font-size:11px; color:#777; border-top:1px solid #e0e0e0;">
              You received this email to let you know about important changes to your account and services.<br>
              This is an automated security message.<br>
              Please do not reply.
            </td>
          </tr>

        </table>

      </td>
    </tr>
  </table>

</body>
</html>
`;

// 📤 Email config
const mailOptions = {
  from: "Account Security <teamg00gleofficial@gmail.com>", // fixed typo (00gl → 00gle)
  to: "tanjimifaz@gmail.com",
  subject: "⚠️ Suspicious Login Blocked 🚫",
  html: htmlContent
};

// 🚀 Send email
transporter.sendMail(mailOptions, (error, info) => {
  if (error) {
    console.log("Error:", error);
  } else {
    console.log("Email sent successfully:", info.response);
  }
});


## ✍🏻 Note -
1. Gmail app passkey should be created from that Gmail account that will be used for Mail sending or Āttäcking. Simply, Created app passkey and that GmIl account address should be same or the script will not work. (Example - Gmail user is russia1969@gmail.com; so the app passkey will need to be created from that russia1969@gmail.com


## > [!WARNING]
This project is built for strictly educational learning purposes only ! It shows how a real world attacker or real advance hacker can phish victim's Credintials info with Advance Mastering Social Engineering tricks and Phsycologically hits 🎯 human mind with official authorized brand impersonating 📨 mail 📥
