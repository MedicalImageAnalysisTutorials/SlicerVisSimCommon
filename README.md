**SlicerVisSimCommon**

Updtae : 12/6/2019

<img src="https://github.com/MedicalImageAnalysisTutorials/SlicerVisSimCommon/blob/4.10.1/SlicerVisSimCommon.png" width="400" height="400">

This is a [3D Slicer](https://gaithub.com/Slicer/Slicer) Extenion that has different useful functions for other VisSim extensions. 

Tested on: Slicer 4.10.1, Windows 10, Ubuntu 18.04 and Mac 

Available functions (more functions and details will be provided later): 

       setGlobalVariables(self,vsExtension):
          vsExtension = 0: Cochlea, vsExtension = 1: Spine
  
       checkVisSimTools(self,vtVars,vsExtension ):
  
       s2b(self,s):
          string to boolean converter

       t2v(self,txt):
          convert text to vector

       ptIJK2RAS(self,ptIJK,inputImg): # imgPath or imgNode are supported
                This function convert an IJK point to RAS point 
                input:  a point vector and volume node/imagePath
                output: a point vector                     
       
       ptRAS2IJK(self,ptRAS,inputImg,i):      
                This function convert RAS ro an IJK point 
                input:  a point vector/Markup node and volume node/imgpath
                output: a point vector 
                
       image2points(self,inputImgNode):                     
            convert binary image of points to markup node
           
       getFiducilsDistanceself,markupsNode,tblNode):
           compute the distance of all points in a markup node
       
       runCropping(self, inputVolume, pointT,croppingLengthT, samplingLengthT, hrChkT,  vtIDt):           
                   crop a node using a central point and cropping length
                   
       runElastix(self, elastixBinPath, fixed, moving, output, parameters, verbose, line):                   
       
       runTransformix(self,transformixBinPath, img, output, parameters, verbose, line):
       
       chkElxER(self,c, s):
                   
       openResultsFolder(self):                   
       
       getSegmentationEditor
       
       runSmoothing(self,segNode,masterNode,KernelSizeMm):       
         
       runMargining(self,segNode,masterNode,MarginSizeMm):
       
       removeOtputsFolderContents(self):
       
       removeTmpsFiles(self):
       
       setItemChk(self,itemT, itemChk, itemName, nodes,):
       
       locateItem(self, inputVolumeNode, inputPointEdt, reg, vtID):
                  reg =0: no registration, 1: fixed image, 2: moving image
       
       getItemInfo(self, segNode, masterNode, tblNode, vtID):
       
       fitAllSlicesViews(self):
         
       fuseWithOutColor(self, disableColor):
       
       fuseTwoImages(self, firstNode, secondNode, colorful):
    
       dispSeg(self,inputVolumeNode, vtSegNode, view):     
       
Your contribution is welcome! 
