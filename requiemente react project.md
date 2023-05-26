<!-- // npm check updates // --> => "مكتبه مسؤله عن عمل تحديثات للمكاتب"
-> npm i npm-check-updates
    \-> enter file package.json search on  script and add "update":"ncu -u" and run npm update

<!-- // FontAwesome // --> =>"مكتبه الايقونات"
-> npm i --save @fortawesome/fontawesome-svg-core
-> npm i --save @fortawesome/free-solid-svg-icons
-> npm i --save @fortawesome/free-regular-svg-icons
-> npm i --save @fortawesome/react-fontawesome@latest
    \-> use :
        \-> import {FontAwesomeIcon} from '@fontawesome/react-fontawesome'
            \-> import {nameIcon} from '@fontawesome/free-solid-svg-icons'


<!-- // emotion style // --> =>"مكتبه لعمل تنسيقات css"
-> npm i @emotion/styled
    \-> import styled from '@emotion/styled';
        \-> export const Navbar =styled('div')`code css`
            \-> import {Navbar} from './path.css'

<!-- // link module alias // --> => "اختصار رابط الملفات"
-> npm i link-module-alias
    \-> enter file package.json search on  script and add "postinstall": "link-module-alias" and add // Aliases
"_moduleAliases": {
  "shared" : "./src/shared",
  "images":"./src/assets/imatges"
} and run npm postinstall after add any link 

<!-- // upload file on github // -->
git add . && git commit -m "setup Project React" && git push -u origin main

<!-- // add Ruls Hook Error // -->
 -> npm install eslint-plugin-react-hooks --save-dev
    \-> // Your ESLint configuration
        {
          "plugins": [
            "react-hooks"
          ],
          "rules": {
            "react-hooks/rules-of-hooks": "error", // Checks rules of Hooks
            "react-hooks/exhaustive-deps": "warn" // Checks effect dependencies
          }
        }

