Bước 1: Ctrl + Shift + J

Bước 2: Bỏ code vô 

Bước 3: Enter
 
File code:

----------------------------------------------
code"
const button = document.querySelector('#btn-update-groupmeeting');
if (button) {
    button.click();
}

setTimeout(() => {
    for (let i = 1; i <= 10; i++) {
        const selector1 = `.MuiTableRow-root:nth-child(${i}) > .MuiTableCell-root:nth-child(3) .css-ykqdxu:nth-child(9)`;
        const element1 = document.querySelector(selector1);
        if (element1) {
            element1.click();
        }
        
        const selector2 = `.MuiTableRow-root:nth-child(${i}) > .MuiTableCell-root:nth-child(4) .css-ykqdxu:nth-child(9)`;
        const element2 = document.querySelector(selector2);
        if (element2) {
            element2.click();
        }
        
        const selector3 = `.MuiTableRow-root:nth-child(${i}) > .MuiTableCell-root:nth-child(5) .css-ykqdxu:nth-child(9)`;
        const element3 = document.querySelector(selector3);
        if (element3) {
            element3.click();
        }
    }

    const buttons = document.querySelectorAll('button.MuiButtonBase-root');
    let gradeButton;
    for (let i = 0; i < buttons.length; i++) {
        if (buttons[i].textContent === 'Grade') {
            gradeButton = buttons[i];
            break;
        }
    }
    if (gradeButton) {
        gradeButton.click();
    }
}, 500);"
