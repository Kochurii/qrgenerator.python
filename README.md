import qrcode
import image
qr = qrcode.QRCode(
version = 15, #15 means the version of the qr code high the  number bigger the code the code image completed picture
box_size = 10 ,#10 means the size  of the box where qrcode will be displayed
border = 5 #it is the white part of image --border in all 4 sides with white color 
)
data ="https://www.phonepe.com/ "
#as i have given the path of my channel like the same way you can given anything 
#if you don't want to redirect and create for normal text that write text in the quotes
qr.add_data(data) 
qr.make (fit=True )
img=qr.make_image(fill="black",black_color="white" )
img.save("test.png")

