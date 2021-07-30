# WordPress-Backup-RCE

This Metasploit module allows an attacker with a privileged WordPress account to launch a reverse shell due to an arbitrary file upload vulnerability in Wordpress plugin Backup Guard versions prior to 1.6.0. This is due to an incorrect check of the uploaded file extension which should be of SGBP type. Then, the uploaded payload can be triggered by a call to /wp-content/uploads/backup-guard/<random_payload_name>.php.
