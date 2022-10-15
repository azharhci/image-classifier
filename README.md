# image-classifier

Download Image folder from Dropbox and copy it to this folder after cloning

To clone this folder run git clone https://github.com/azharhci/image-classifier.git in your terminal



Code Comments

# to Set Path of the Folder
mypath = 'bangladesh_201901_1'
onlyfiles = [f for f in listdir(mypath) if isfile(join(mypath, f))]
images = numpy.empty(len(onlyfiles), dtype=object)
# to Load Images in the Excel Sheet
for n in range(0, len(onlyfiles)):
    images[n] = cv2.imread(join(mypath, onlyfiles[n]))
print(len(onlyfiles))
workbook = xlsxwriter.Workbook(mypath+'.xlsx')

# For Setting the frame 
def highlightFace(net, frame, conf_threshold=0.7):

# writing propeties
for col, data in enumerate(numberOfFaces):
    print(data)
    row = row + 1
    array1.append(data)
    worksheet.write_number(row, 5, data)
print(len(array1))
print(len(genderArray))
print(numberOfFaces)
workbook.close()
