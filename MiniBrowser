// ==UserScript==
// @name         MiniBrowser!
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  MADE SPECIFICALLY FOR EDGENUITY (CODE NOT SPECIFICALLY FITTED FOR IT HOWEVER IT IS MY INTENTION TO MAKE IT SPECIFICALLy FOR EDGENUITY) ONLINE SCHOOL
// @author       H4CKE3R
// @match        https://r17.core.learn.edgenuity.com/player/, www.google.com, ONLINE SCHOOLS!
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    // Create UI elements
    const container = document.createElement('div');
    container.style.position = 'fixed';
    container.style.bottom = '10px';
    container.style.right = '10px';
    container.style.zIndex = '9999';
    container.style.backgroundColor = '#fff';
    container.style.border = '1px solid #ccc';
    container.style.padding = '5px';

    const input = document.createElement('input');
    input.type = 'text';
    input.placeholder = 'Enter URL';
    input.style.width = '200px';

    const button = document.createElement('button');
    button.textContent = 'Go';
    button.style.marginLeft = '5px';

    const iframe = document.createElement('iframe');
    iframe.style.width = '300px';
    iframe.style.height = '200px';
    iframe.style.border = '1px solid #ccc';

    container.appendChild(input);
    container.appendChild(button);
    container.appendChild(document.createElement('br'));
    container.appendChild(iframe);

    document.body.appendChild(container);

    // Navigate function
    const navigate = () => {
        const url = input.value.trim();
        if (url !== '') {
            iframe.src = url;
        }
    };

    // Event listeners
    button.addEventListener('click', navigate);
    input.addEventListener('keydown', (e) => {
        if (e.key === 'Enter') {
            navigate();
        }
    });

})();
