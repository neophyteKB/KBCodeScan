# KBCodeScan
Drop a view in xib, name it <KBCodeScanner> 
To get output of QRScanner, use call back like :

scanView.callBackQRData = { (_ strScannerString: String?) in
            if let strOutput = strScannerString{
                print("output : \(strOutput)")
                self.messageLabel.text = strOutput
            }
        }
