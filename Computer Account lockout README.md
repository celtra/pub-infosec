# Account lockout

By limiting the number of failed login attempts, the risk of unauthorized system access via user password guessing, otherwise known as brute forcing, is reduced. Limits are imposed by locking the account. 

Setting a lockout expiration of 15 minutes is an effective deterrent against brute forcing that also makes allowances for legitimate mistakes by users.

Computer accounts must be configured to automatically lock themselves for at least 15 minutes after 5 consecutive failed login attempts.

## MacOS X Account Lockout settings

To set up a suitable Password Policy and Account Lockout we have provided a user-installable configuration profile which will automatically set the constraints described above. This profile will affect all user accounts on your macOS.

### To obtain the configuration profile please follow the instructions below:

1. Download our [macOS-Login-Password-Policy.mobileconfig](https://github.com/celtra/pub-infosec/raw/master/macOS-Login-Password-Policy.mobileconfig) file from GitHub.
(You may be asked by your browser to confirm that you wish to download this type of file, if so click Allow/Permit.)
2. Open *Profiles* under *Apple menu > System Settings > Privacy & Security > Others*.
  * A quick alternative is to open [Spotlight](https://support.apple.com/en-gb/guide/mac-help/mchlp1008/mac) with *Command+Space* and search for *profiles*.
3. Click *+*, navigate to your Downloads folder and locate the downloaded mobileconfig file, *Open* it.
4. A pop-up dialog will allow you to review the contents of the device profile, select *Continue* and then *Install*.
5. You may be prompted to provide your password to install the profile, please do so if requested.

ℹ️  Note: This will also set password complexity settings for MacOS accounts according to the Celtra password policy minimum standards.

## Windows 10 Account Lockout settings

To set up the Account Lockout threshold and duration, open the Local Security Policy application. 

1. Start → type in “Local Security Policy” to search bar and press enter.
2. Navigate to: Security Settings → Account Policies → Account Lockout Policy → Account lockout threshold.
3. Set the value to 5 and click Apply. 
4. In pop-up windows, click OK to confirm two related settings (Duration & Counter) to be applied as well.

## Need help?

If you have any questions about policy content, please contact infosec@celtra.com. If you need help enabling this on your computer please contact your local IT for assistance.

