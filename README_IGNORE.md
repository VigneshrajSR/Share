## SlideIn Document Issue:  

### JSP added:  
- ALT_emxProgramCentraFolderUtil:  
	```
	var topFrame = findFrame(getTopWindow(), "detailsDisplay");
					if(topFrame == null) {
						topFrame = findFrame(getTopWindow(), "portalDisplay");
	            	            	            
					}
					getTopWindow().closeSlideInDialog();
					topFrame.emxEditableTable.addToSelected('<%=xmlMessage%>');
					topFrame.refreshStructureWithOutSort();
	```
- ALT_emxProgramCentralDocumentCreatePreProcess.jsp:  
```
           		contentURL.append("../components/emxCommonDocumentPreCheckin.jsp?objectAction=create&appDir=programcentral&appProcessPage=ALT_emxProgramCentraFolderUtil.jsp&actionMode=createDocument");
```  
### Spinner added:  
- PMCCreateNewFolderDocument	PMCCreateNewFolderDocument	Create New Document object	emxProgramCentral.Command.CreateDocument	<ins>${SUITE_DIR}/ALT_emxProgramCentralDocumentCreatePreProcess.jsp?documentAction=create&fileRequired=false&mode=workspaceVault</ins>		Access Function | Access Program | CmdName | Image | Licensed Product | Popup Modal | Registered Suite | Submit | Target Location | Slidein Width | Window Height | Window Width	checkFolderAccess | com.dassault_systemes.enovia.lsa.lra.services.ui.Submission | PMCCreateNewFolderDocument | ${COMMON_DIR}/images/I_CreateDocument32.png | ENO_PGE_TP | true | ProgramCentral | true | slidein | 700 | 570 | 1080	Global User | VPLMViewer | 3DSRestrictedReader	FALSE		
