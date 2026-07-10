
## Jamf DNS Bypass
> A simple way to bypass JAMF MDM
>
> ### How It Works ?
> When a managed device boots up or connects to the internet, it pings specific Apple/ Jamf servers to pull down MDM. By using a DNS it block those requests and that Block MDM away form your stuff!
 
## How to use 

> ### Method A: NextDNS
> 1. Go to [NextDNS](https://nextdns.io) and create a free account or use without account that also work fine
> 2. In your dashboard, navigate to the **Denylist** tab.
> 3. Copy the domains from the `jamf-domains.txt` file in this repository or blocklist below and paste them in.
> 4. Go to the **Setup** tab on NextDNS, download the configuration profile for your device (iOS, macOS, Android), and install it.
>
> ### Method B: SelfHosted Pi-hole / AdGuard Home etc
> 1. Open your local Pi-hole or AdGuard Home dashboard.
> 2. Go to **Adlists** or **Blocklists**.
> 3. Add the raw URL of the `jamf-domains.txt` file from this GitHub repository or blocklist below.
> 4. Save and update your gravity database.
>
> ### blocklists
> ```text
> * albert.apple.com
> * iprofiles.apple.com
> * mdmenrollment.apple.com
> * deviceenrollment.apple.com
> * mesu.apple.com
> * configuration.apple.com
> * configuration.ls.apple.com
> * ocsp2.apple.com
> * cdn.smoot.apple.com
>
> * jamfschool.com
> * jamfnow.com
> * jamf.com
> * jamfcloud.com
> * mdm-na1.jamfcloud.com
> * 3000619.mdm.jamfschool.com
> * root.edu.3000619.jamfschool.com
> * ap-northeast-1.resources.school.jamf.com
> * leader.edu.3000619.jamfschool.com
> * member.edu.3000619.jamfschool.com
> * apne1-jschool-prod240117.alb.internal.jamfcloud.com
> ```
>
> get an full list form `jamf-domains.txt`
>
> ## ⚖️ Liability Disclaimer
> ### use at your own risk i do not responsible for any outcome 
