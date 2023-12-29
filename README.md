
@import '../../assets/scss/variables';
@import '../checkbox/checkbox.component.scss';

//common style for button




.unity-short-button{ 
    min-width: fit-content;
        height: 34px;
    
        padding: 5px 16px 5px 16px !important;
        border-radius: 4px;
        align-self: center;

}
.unity-short-button-with-icon {
    width: 126px;
    height: 34px;
    padding: 5px 16px 5px 16px;
    border-radius: 4px;
    align-self: center;
    gap: 10px;
}

//Default Button
::ng-deep.mat-mdc-button:not(:disabled){
    --mdc-text-button-label-text-color: #0E599E;
}
::ng-deep.mat-mdc-button[disabled] {
    cursor: not-allowed !important;
    pointer-events: none;
    color: #BDBDBD !important;//gray400
    
}
::ng-deep.mat-mdc-button:not(:disabled):hover{
    --mdc-text-button-label-text-color: #60BAD2;
    --mat-text-button-state-layer-color: none;
    --mat-text-button-ripple-color:none
}
::ng-deep.mat-mdc-button:not(:disabled):active{
    --mdc-text-button-label-text-color: #08355F;
    
    --mat-text-button-ripple-color:none
    --mat-text-button-state-layer-color: white;
}

//stroked button
::ng-depp.mat-mdc-outlined-button.mat-accent {
    --mdc-outlined-button-label-text-color: #00FFFFFF ;
    --mdc-outlined-button-outline-color: #00FFFFFF;
    --mat-outlined-button-state-layer-color: #00FFFFFF;
    --mat-outlined-button-ripple-color: #00FFFFFF;
}
.unity-stroked-button {
    color: $primary-default !important; //sec300
    background-color: $white !important;
    transform: none !important;
    &:hover {
        color: $secondary-300 !important; //sec300
        background-color: #F5F5F5 !important; //neutral100
        border: 1px solid #BDBDBD
    }

    &:active {
        color: $primary-pressed !important;
        //sec300
        background-color: #BDBDBD !important; //neutral300
        border: 1px solid #BDBDBD
    }

    &:disabled {
        color: #BDBDBD !important;
        // background: linear-gradient(0deg, #EEEEEE, #EEEEEE),
        // linear-gradient(0deg, #FFFFFF, #FFFFFF);
        border: 1px solid #EEEEEE !important;

    }
}
.icon{
    justify-content: center !important;
    display: flex !important;
    font-size: 22px !important;
    align-items: center !important;
    margin: 0px !important;
}
//flat button

::ng-deep.mat-mdc-unelevated-button.mat-accent {
    --mdc-filled-button-container-color: transparent;
    --mdc-filled-button-label-text-color: white;
    --mat-filled-button-state-layer-color: transparent;
    --mat-filled-button-ripple-color: transparent;
}
.unity-flat-button {
    background-color: $primary-default !important;
    transform: none !important;
    &:hover {
        // color:white;//sec300
        background-color: $primary-hover !important; //sec600 
    }

    &:active {
        // color:white;//sec300
        background: $primary-pressed !important;
        //sec600 
    }

    &:disabled {
        color: white !important;
        background: linear-gradient(0deg, #EEEEEE, #EEEEEE),
            linear-gradient(0deg, #FFFFFF, #FFFFFF) !important;
        border: 1px solid #EEEEEE !important;

    }
}

.mat-mdc-unelevated-button[disabled] {
    color: white;
    cursor: not-allowed;
}
.mat-mdc-unelevated-button .mat-mdc-button-touch-target{
    transform: none !important;
}

.unity-icon-button {
    width: 42px;
    height: 42px;
    border-radius: 4px;
    color: $primary-default;
    background-color: $white;
    border: none;
    cursor: pointer;
    padding: 0px;
    display: flex;
    align-items: center;
    justify-content: center;

    &:hover{
        // background-color: #2E91B8;//sec600 
        color: $primary-hover;
    }
    &:active{
        // background: linear-gradient(0deg, rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)),
        // linear-gradient(0deg, #2E91B8, #2E91B8);
        color:$primary-pressed;
         
    }
    &:disabled{
        color: $primary-disabled;
    // background: linear-gradient(0deg, #EEEEEE, #EEEEEE),
    // linear-gradient(0deg, #FFFFFF, #FFFFFF);
    // border: 1px solid #EEEEEE;
     svg{
        fill:$primary-disabled;
     }
    }
    svg{
        fill:$primary-default;
        &:hover{
            fill: $primary-hover;
        }
        &:active{
            fill:$primary-pressed;
         }
    }
}

.unity-fab-button {
    width: 56px;
    height: 56px;
    background-color: $error-base;
    &:hover{
        background-color:$error-300;
        ;//sec600 
    }
    &:active{
        background:#F15A7D;
         
    }
    &:disabled{
        color: white ;
    background: #E0E0E0;
    }
}








