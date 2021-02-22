from PyQt5 import QtCore, QtGui, QtWidgets


class Ui_MainWindow(object):
    def setupUi(self, MainWindow):
        MainWindow.setObjectName("MainWindow")
        MainWindow.resize(703, 607)
        self.centralwidget = QtWidgets.QWidget(MainWindow)
        self.centralwidget.setObjectName("centralwidget")
        self.Photo = QtWidgets.QLabel(self.centralwidget)
        self.Photo.setGeometry(QtCore.QRect(10, 10, 681, 401))
        self.Photo.setText("")
        self.Photo.setPixmap(QtGui.QPixmap("dog.jpg"))
        self.Photo.setScaledContents(True)
        self.Photo.setObjectName("Photo")
        self.DogPB = QtWidgets.QPushButton(self.centralwidget)
        self.DogPB.setGeometry(QtCore.QRect(10, 460, 341, 71))
        self.DogPB.setObjectName("DogPB")
        self.CatPB = QtWidgets.QPushButton(self.centralwidget)
        self.CatPB.setGeometry(QtCore.QRect(360, 460, 331, 71))
        self.CatPB.setObjectName("CatPB")
        MainWindow.setCentralWidget(self.centralwidget)
        self.menubar = QtWidgets.QMenuBar(MainWindow)
        self.menubar.setGeometry(QtCore.QRect(0, 0, 703, 21))
        self.menubar.setObjectName("menubar")
        MainWindow.setMenuBar(self.menubar)
        self.statusbar = QtWidgets.QStatusBar(MainWindow)
        self.statusbar.setObjectName("statusbar")
        MainWindow.setStatusBar(self.statusbar)

        self.retranslateUi(MainWindow)
        QtCore.QMetaObject.connectSlotsByName(MainWindow)

        self.DogPB.clicked.connect(self.show_dog)
        self.CatPB.clicked.connect(self.show_cat)
        

    def retranslateUi(self, MainWindow):
        _translate = QtCore.QCoreApplication.translate
        MainWindow.setWindowTitle(_translate("MainWindow", "MainWindow"))
        self.DogPB.setText(_translate("MainWindow", "Dog"))
        self.CatPB.setText(_translate("MainWindow", "Cat"))

    def show_cat(self):
        self.Photo.setPixmap(QtGui.QPixmap("cat.jpg"))

    def show_dog(self):
        self.Photo.setPixmap(QtGui.QPixmap("dog.jpg"))
        

if __name__ == "__main__":
    import sys
    app = QtWidgets.QApplication(sys.argv)
    MainWindow = QtWidgets.QMainWindow()
    ui = Ui_MainWindow()
    ui.setupUi(MainWindow)
    MainWindow.show()
    sys.exit(app.exec_())
