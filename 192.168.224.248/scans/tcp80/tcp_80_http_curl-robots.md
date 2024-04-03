HTTP/1.1 200 OK
Cache-Control: public,max-age=31536000
Content-Type: text/plain
Last-Modified: Wed, 28 Sep 2022 12:36:56 GMT
Accept-Ranges: bytes
ETag: "06490fe36d3d81:0"
Server: Microsoft-IIS/10.0
X-XSS-Protection: 1; mode=block
X-Frame-Options: SAMEORIGIN
Date: Wed, 03 Apr 2024 03:58:05 GMT
Content-Length: 741

# Begin robots.txt file
#/-----------------------------------------------\
#| In single portal/domain situations, uncomment the sitmap line and enter domain name
#\-----------------------------------------------/
#Sitemap: http://www.DomainNamehere.com/sitemap.aspx

User-agent: *
Disallow: /*/ctl/		# Googlebot permits *
Disallow: /admin/
Disallow: /App_Browsers/
Disallow: /App_Code/
Disallow: /App_Data/
Disallow: /App_GlobalResources/
Disallow: /bin/
Disallow: /Components/
Disallow: /Config/
Disallow: /contest/
Disallow: /controls/
Disallow: /Documentation/
Disallow: /HttpModules/
Disallow: /Install/
Disallow: /Providers/
Disallow: /Activity-Feed/userId/	# Do not index user profiles

# End of robots.txt file