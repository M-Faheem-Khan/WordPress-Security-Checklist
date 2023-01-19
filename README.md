# WordPress-Security-Checklist

The following are some of the many 

- [ ] Download the latest WordPress release
- [ ] Download the latest MySql release
- [ ] Download the latest MyPhpAdmin release
- [ ] Change default MySQL `root` and `user` password
- [ ] Set a strong password for WordPress admin (prevents default/weak password guessing)
- [ ] Enable Multi-Factor Authentication(MFA)  
- [ ] Block or add rate limit on login and form pages (prevents bruteforcing)
    - Block the login routes via WAF
    - Add Captcha or WAF rate limit
- [ ] Block the following routes to prevent user enumeration:
    - /?author=1
    - /wp-json/wp/v2/users
    - /?rest_route=/wp/v2/users
    - /wp-json/wp/v2/users?search
- [ ] Prevent external connection to sensitive ports (MySQL:3306, CPanel:2082/2083, FTP:21, SSH:22)
- [ ] Update Themes and Plugins to the latest version
- [ ] Disable directory indexing
- [ ] Setup SSL Certificate
- [ ] Redirect HTTP connect to HTTPS
- [ ] Remove unused themes and plugins
- [ ] Regularly update all plugins, themese and software

### Additional Reading
- https://www.gosecure.net/blog/2021/03/16/6-ways-to-enumerate-wordpress-users/
- https://hackertarget.com/wordpress-user-enumeration/
- https://www.wpbeginner.com/wp-tutorials/disable-directory-browsing-wordpress/
- https://www.wpbeginner.com/wp-tutorials/how-to-add-ssl-and-https-in-wordpress/
- https://www.wpbeginner.com/wp-tutorials/how-to-add-free-ssl-in-wordpress-with-lets-encrypt/
- https://blog.wpsec.com/enumerating-wordpress-plugins-at-scale/

#### Vulnerability Databases
- https://patchstack.com/database/
- https://wpscan.com/plugins

<!-- EOF -->
