# ⚙️ Documentation of _Mautic Theme (with tokens)_ by _PIGEONPOSSE™_

The use of this theme is **like any other of Mautic**, the only difference is that as this theme depends on the **custom tokens** of [_Mautic Extra Tools_](https://github.com/PigeonPosse/mautic-plugin-extra-tools#-installation) plugin, these tokens have to be created manually.
We have made a **guide** of recommendations of how those **tokens** should be.


List of **custom tokens** used by the theme:

+ [```{pigeontoken="header"}```](#-pigeontokenheader)
+ [```{pigeontoken="social-links"}```](#-pigeontokensocial-links)
+ [```{pigeontoken="web-links"}```](#-pigeontokenweb-links)
+ [```{pigeontoken="copyright"}```](#-pigeontokencopyright)

## PigeonTokens

### 📌 {pigeontoken="header"}

This token is intended to be the header of the **mails** and the **_Mautic_ pages**. 
The example would show an image as a link, usually the image will be the logo and the url of the link will be the address of your website.

<details open>
	<summary>HTML structure recommendation:</summary>

```html

<table border="0" cellpadding="0" cellspacing="0" role="presentation" style="border-collapse:collapse;border-spacing:0px;margin: auto;">
	<tbody>
		<tr>
			<td style="width:320px;">
				<a href="{url}" target="_blank">
					<img height="auto" src="{img-url}" style="border: 0px; display: block; outline: none; text-decoration: none; height: auto; width: 100%; font-size: 13px; float: left;" width="320" alt="Logo" title="Logo"/> 
				</a>
			</td>
		</tr>
	</tbody>
</table>

```

Variables to change:

- **``{url}``**: Change for a url, _example: your website url_.
- **``{img-url}``**: Change for an image url, _example: your website logo_.

</details>

<details>
	<summary>Change the position of the image table</summary>

If you want to change the position of the image you have to change image table margin style.
Examples:

- Center _(default)_:

	```html 
	<table border="0" cellpadding="0" cellspacing="0" role="presentation" style="border-collapse:collapse;border-spacing:0px;margin: auto;">
	```

- Left:

	```html 
	<table border="0" cellpadding="0" cellspacing="0" role="presentation" style="border-collapse:collapse;border-spacing:0px;margin: auto auto auto 0;">
	```

- Right:

	```html 
	<table border="0" cellpadding="0" cellspacing="0" role="presentation" style="border-collapse:collapse;border-spacing:0px;margin: auto 0 auto auto;">
	```

</details>

### 📌 {pigeontoken="social-links"}

This token is designed to display social media links.

<details open>
	<summary>HTML structure recommendation:</summary>

```html

<table border="0" cellpadding="0" cellspacing="0" width="100%">
	<tbody>
		<tr>
			<!-- First cell -->
			<td style="align-content: center; width:10%;"></td>
			<!-- Social icon cell example -->
			<td style="align-content: center;">
				<a href="{social-url}" target="_blank">
					<img height="auto" src="{social-image-url}" style="border:0;display:block;outline:none;text-decoration:none;height:auto;width: 20px;font-size:13px;margin: auto;" width="20px" alt="Social Network" title="Social Network" /> 
				</a>
			</td>
			<!-- Last cell -->
			<td style="align-content: center; width:10%;"></td>
		</tr>
	</tbody>
</table>

```

Variables to change:

+ **``{social-url}``**: Change for social url.
+ **``{social-image-url}``**: Change for a social image url.

</details>

<details>
	<summary>Social Theme Icons:</summary>

In this same theme, there are already social icons for _Facebook_, _Github_, _Instagram_, _Pinterest_ and _Twitter_, you can use them, if you think necessary.

</details>

### 📌 {pigeontoken="web-links"}

This token is designed to display links of the most prominent sections of your website.

<details open>
	<summary>HTML structure recommendation:</summary>

```html

<p>
	<!-- link example-->
	<a href="{link-url}" style="color: #351f53; font-style: italic; text-decoration: none; margin: 0 10px; font-size:14px;" target="_blank">
		{link-name}
	</a>
</p>

```

Variables to change:

+ **``{link-url}``**: Change for your link url.
+ **``{link-name}``**: Change for link name.

</details>

<details>
	<summary>Change link color:</summary>

If you want the link text color to be changed in the email, you must specify it in each link style attribute.

</details>


### 📌 {pigeontoken="copyright"}

This token is designed to display copyright text.

<details open>
	<summary>HTML structure recommendation:</summary>

```html

<p style="font-size:13px">copyright © {year}</p>

```

Change variables: 

+ **``{year}``**: Change to the year it is.

</details>


