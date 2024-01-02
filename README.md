# DomainCleaner
A script repository for removing specific domains from text files using `sed`. 

```
sed -i -E '/(azure.net|botframework.com|ckeditor.com|atlassian.com|yimg.com|githubusercontent.com|github.io|hcg.one|azure-mobile.net|cloudflaressl.com|selforder.live|minhtamgroup.org|titano.jp|click.fan|choiceagedcare.com.au|instagram.com|vereinerhaltungundbauungvonstaumauern.ch|azurewebsites.net|tcraft.ch|karma.life|wgarvey.info|zudios.com|document360.io|quantummetric.com|xking.id|ynothave.fun|juntao.life|dyang.com.mx|33tab.jp|slapdefi.io|ch.se|stevehaar.com|mccartney.ie|cloudflaressl.com|mosa-architect.com|rudydogum.com|quickdsn.com|adorie.com.br|safarixperts.com|form.io|pbbl.co|seanfinegan.dev|justiceapp.com|windowsazure.us|azure-ppe.net|microsoftazuread-sso.com|azure-int.net|onmicrosoft.com|microsoft.com|microsoftonline.com|msidentity.com|windows.net|windows-ppe.net|microsoftonline-p-int.com|b2clogin.com|live.com|office.com|live-int.com|windowsazure.us|ccsctp.com|localhost.localdomain|game.co.za|dasherapp.net|member-ally.com|cloudflare-dns.com|bootstrapcdn.com|equifax.com|akamaized.net|akamai.net|akamaihd-staging.net|microsoftonline.com|akamaihd.net|akamaized-staging.net|google.com|cloudflare.com|cloudfront.net|cloudfront.com|fastly.com|incapsula.com|oracle.com|akamai.com|sucuri.com|leaseweb.com|awmdm.com|lync.com|msecnd.net|exacttarget.com|nextdoor.com|onmicrosoft.com|one.one.one.one|awmdm.com|windows.net|aspnetcdn.com|ccsctp.com|outbrain.com|mopinion.com)/d domainlist.txt'
```

### Remove Specific Domains Using sed

- **Command**: `sed -i -E '/(domain1|domain2|...|domainN)/d'`
- **Purpose**: This update includes a `sed` command used to modify files in-place. The `-i` flag ensures the changes are written directly to the file.
- **Regex Explanation**: The regular expression `/(domain1|domain2|...|domainN)/d` is used for pattern matching. It targets a list of specific domains, such as `azure.net`, `botframework.com`, `ckeditor.com`, etc.
- **Action**: For every line in the file that matches any of the listed domains, this command will delete that line. The `-E` flag enables extended regular expressions, which allow for the use of the `|` operator for 'or' functionality within the parentheses.
- **Use Case**: Useful for cleaning configuration files or logs where specific domain references need to be removed for privacy, compliance, or security reasons.
- **Caution**: Be careful with this command as it directly alters the file. Ensure you have backups or version control in place.
