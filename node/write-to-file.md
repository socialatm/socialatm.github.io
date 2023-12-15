write to file 

    const fs = require('node:fs');

   
    const content = 'write something';
    fs.writeFile('./test.txt', content, { flag: 'a+' }, err => {
      if (err) {
        console.error(err);
      }
      // file written successfully
    });