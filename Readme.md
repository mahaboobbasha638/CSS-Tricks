# CSS Tricks
## PopUp Block
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
        