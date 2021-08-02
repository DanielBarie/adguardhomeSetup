# adguardhomeSetup
Some Notes On Setting Up AdguardHome

- Set it up as a snap package: https://snapcraft.io/install/adguard-home/ubuntu
- Having installed it as snap package will lead to adguard not being able to read `/etc/letsencrypt/live/<domain>/privkey.pem`. We need to have a post-renewal hook: https://certbot.eff.org/docs/using.html?highlight=hook#pre-and-post-validation-hooks (and run this at least once so the stuff gets copied)
- Instructions on how to copy: https://github.com/AdguardTeam/AdGuardHome/issues/2601
- 
