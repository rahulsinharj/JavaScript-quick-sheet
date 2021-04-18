## Local and Session Storage:
  * Web applications can store data locally within the user's browser with web storage. 
  * Before HTML5, application data stored in cookies, included in every server request. 
  * Previously we were having only cookies, which were very restrictive, and the size of the cookies was very small. 
  * But now the web storage is more secure, and large amounts of data can be stored locally, without affecting website performance. 
    <hr/>
  * HTML web storage provides us with two objects for storing data:
      1. `window.localStorage:`
         *  The way to store data on the client's computer is by local storage. 
         *  The local storage allows us to save the key/value pairs in a web browser, and it stores data with no expiration date. 
         *  We can access local storage via JavaScript and HTML5. However, the user can clear the browser data to erase all localStorage data.
      2. `window.sessionStorage:`
         *  The session storage is used to store data only for a session, meaning that it is stored until the browser (or tab) is closed. 
         *  In session storage, the data is never transferred to the server and can only be read on the client-side. 
         *  The storage limit is between 5-10MB. 
         *  By opening multiple windows or tabs with the same URL creates sessionStorage for each tab or window.
    
  * Both storage objects provide the same methods and properties like setItem, getItem, removeItem, and clear. 
  * Some of them are: (The examples are for localStorage, but the same syntax works for sessionStorage.)
      1. Creating Entries:
      ``` 
      let key = 'Entry_1';
      localStorage.setItem(key, 'Value');
      ```
      2. Reading Entries:
      ```
      let myItem = localStorage.getItem(key);
      ```
      3. Updating Entries:
      ```
      localStorage.setItem(key, 'New Value');
      ```
      4. Deleting Entries:
      ```
      localStorage.removeItem(key);
      ```
      5. Clearing Everything:
      ```
      localStorage.clear();
      ```
      6. Storing JSON Objects: 
         * Only strings can be stored with localStorage or sessionStorage, but we can use JSON.stringify to store more complex objects and JSON.parse to read them.
         
         ```
         // Create item:
         let myObj = { name: 'Sanya', language: 'JavaScript' };
         localStorage.setItem(key, JSON.stringify(myObj));
         // Read item:
         let item = JSON.parse(localStorage.getItem(key));
         ```
