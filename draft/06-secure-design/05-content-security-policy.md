---

title: Content Security policy
layout: col-document
tags: OWASP Developer Guide
author: Shruti Kulkarni
contributors:
document: OWASP Developer Guide
order: 605

---

{% include breadcrumb.html %}
### 6.5 Content Security policy

The OWASP Development Guide is being rewritten by the OWASP community.
and the content of this section has yet to be filled in.

If you would like to contribute then follow the 
[contributing guidelines](https://github.com/OWASP/www-project-developer-guide/blob/main/CONTRIBUTING.md)
and submit your content for review.


Content Security Policy (CSP) helps in whitelisting the sources that are allowed to be executed by clients.

To this effect CSP helps in addressing vulnerabilities that are the target of scripts getting executed from different domains (namely XSS, ClickJacking)  

1.	The policy elements listed below is restrictive. Third party libraries can be whitelisted as a part of script-src, default-src, frame-src or frame-ancestors.

2.	I assume fonts / images / media / plugins are not loaded from any external sources. 

3.	Do not use \*\ as an attribute for any of the components of the policy.

CSP considers two types of content:

Passive content - resources which cannot directly interact with or modify other resources on a page: images, fonts, audio, and video for example

Active content - content which can in some way directly manipulate the resource with which a user is interacting.

SCOPE

The scope of this policy / procedure / whatever includes (but not limited to):

-	Applications that are displayed in browsers
    - On desktops
    - On laptops
    - On mobile devices
-	Mobile Applications
    - iOS
    - Android


Policy for content security should be set in <<add SSDLC Policy / Secure Coding Policy / any others that is applicable>>. Unless otherwise specified  by the customer, third party sources should not be allowed to connect from the deployed solutions

Web Applications

For web applications, the source of all content is set to self.
-	default-src 'self'
-	script-src 'self';
-	script-src 'unsafe-inline' 'unsafe-eval' https:; (I am fairly sure this is used to block unsafe inline scripts and 'eval' but to be checked) - Have checked now and unsafe-inline should not be used
-	connect-src 'self';
-	img-src 'self';
-	style-src 'self'
-	style-src 'unsafe-inline' https:; (I am fairly sure this is used to block unsafe inline scripts but to be checked) - Have checked now and unsafe-inline should not be used
-	font-src 'self';
-	frame-src https:;
-	frame-ancestors 'none' (This is to prevent ClickJacking equivalent to X-FRAME-OPTIONS = SAME-ORIGIN)
-	frame-ancestors 'self' (This is to prevent ClickJacking equivalent to X-FRAME-OPTIONS = SAME-ORIGIN)
-	frame-ancestors 'example.com' (This component allows content to be loaded only from example.com.)
-	media-src 'self':;
-	object-src 'self:;
-	report-uri <<>> (insert the URL where the report for policy violations should be sent)
-	sandbox (this is something to be tried out specifies an HTML sandbox policy that the user agent applies to the protected resource)
-	plugin-types <<>> (insert the list of plugins that the protected resource can invoke)
-	base-uri (restricts the URLs that can be used to specify the document base URL, but I do not know how this is used)
-	child-src 'self'

An Example:
<add name="Content-Security-Policy" value="script-src *.google-analytics.com maps.googleapis.com apis.google.com 'self';" script-src 'self' font-src 'self' frame-ancestors 'toyota.co.uk' object-src 'self' />

For display on desktops and laptops:
add name="Content-Security-Policy" value

For display on other mobile decvices that use HTML5:
meta http-equiv="Content-Security-Policy"
Mobile Apps	 
iOS

iOS framework has capability to restrict connecting to sites that are not a part of the whitelist on the application, which is the NSExceptionDomains. Use this setting to restrict the content that gets executed by the application

NSAppTransportSecurity : Dictionary {
    NSAllowsArbitraryLoads : Boolean
    NSAllowsArbitraryLoadsForMedia : Boolean
    NSAllowsArbitraryLoadsInWebContent : Boolean
    NSAllowsLocalNetworking : Boolean
    NSExceptionDomains : Dictionary {
        <domain-name-string> : Dictionary {
            NSIncludesSubdomains : Boolean
            NSExceptionAllowsInsecureHTTPLoads : Boolean
            NSExceptionMinimumTLSVersion : String
            NSExceptionRequiresForwardSecrecy : Boolean   
            NSRequiresCertificateTransparency : Boolean
        }
    }
}

4.	Android
Setting rules for Android application:
-	If your application doesn't directly use JavaScript within a WebView, do not call setJavaScriptEnabled()
-	By default, WebView does not execute JavaScript, so cross-site-scripting is not possible
-	Use addJavaScriptInterface() with particular care because it allows JavaScript to invoke operations that are normally reserved for Android applications. If you use it, expose addJavaScriptInterface() only to web pages from which all input is trustworthy
-	Expose addJavaScriptInterface() only to JavaScript that is contained within your application APK
-	When sharing data between two apps that you control or own, use signature-based permissions
<manifest xmlns:android=<link to android schemas ...>
    package="com.example.myapp">
    <permission android:name="my_custom_permission_name"
                android:protectionLevel="signature" />
-	Disallow other apps from accessing ContentProvider objects
<manifest xmlns:android=<link to android schemas ...>
    package="com.example.myapp">
    <application ... >
        <provider
            android:name="android.support.v4.content.FileProvider"
            android:authorities="com.example.myapp.fileprovider"
            ...
            android:exported="false">
            <!-- Place child elements of <provider> here. -->
        </provider>
        ...
    </application>
</manifest>

\newpage
