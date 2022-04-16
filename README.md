# Javascript popup show with c#

#Code
modal popup show on click button using c#  
(1) -  string clientScript = @"
                $(function(){
                          $('#RechargeConfirmPopup').modal('show');
                    });";
                Page.ClientScript.RegisterStartupScript(this.GetType(), this.ClientID, clientScript, true);
                
                
         (2)-       // ScriptManager.RegisterStartupScript(Page, Page.GetType(), "myModal", "$('#RechargeConfirmPopup').modal('show');", true);
                
         (3)     // ClientScript.RegisterStartupScript(this.GetType(), "Popup", "PopupConfirmRecharge();", true);
