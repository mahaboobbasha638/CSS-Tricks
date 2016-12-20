# CSS Tricks
## PopUp Block
-
        .popup_container{
            position: absolute;
            top: 0;
            width: 100%;
            height: 100%;
            text-align: center;

            &::before{
                content: "";
                display: inline-block;
                height: 100%;
                vertical-align: middle;
            }

            .pc_main {
                width: 80%;
                height: 300px;
                display: inline-block;
                vertical-align: middle;
            }
        }

        
-
        .container{
            background-color: rgba(0,0,0,0.5);
            width: 100%;
            height: 100%;
            position: fixed;
            top: 0;
            z-index: 10;
        
            .inner{
                max-width: 80%;
                margin: 50px auto;
        
                .head{
                    background-color: white;
                    height: 50px;
                    padding: 15px;
                    border-bottom: 1px solid #e5e5e5;
                }
        
                .conent{
                    max-height: calc(100% - 200px);
                }
        
                .fotter{    
                    background-color: white;
                    height: 50px;
                    padding: 15px;
                    border-top: 1px solid #e5e5e5;
                }
            }
        }