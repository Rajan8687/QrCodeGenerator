

├── README.md
├── YoutubeHomepage.png
└── generate_qr.py


/README.md:
--------------------------------------------------------------------------------
1 | # QrCodeGenerator


--------------------------------------------------------------------------------
/YoutubeHomepage.png:
--------------------------------------------------------------------------------
https://raw.githubusercontent.com/Rajan8687/QrCodeGenerator/8b1b308d37cdcdf3538c09b67333e59014878f07/YoutubeHomepage.png


--------------------------------------------------------------------------------
/generate_qr.py:
--------------------------------------------------------------------------------
1 | import qrcode
2 | import qrcode.constants
3 | from PIL import Image
4 | 
5 | qr = qrcode.QRCode(version=1,error_correction=qrcode.constants.ERROR_CORRECT_H,box_size=10,border=4,)
6 | qr.add_data("https://www.youtube.com/")
7 | qr.make(fit=True)
8 | img = qr.make_image(fill_color="black",back_color="white")
9 | img.save("YoutubeHomepage.png")


--------------------------------------------------------------------------------

