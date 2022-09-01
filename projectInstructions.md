## Run the below commands first

npm install react-router-dom@6
npm install firebase
npm install --save react-firebase-hooks
npm install --save react-toastify
npm install react-icons --save
npm install react-hook-form


1. Open index.js and wrap the <App/> with <BrowserRouter>
	<BrowserRouter>
      		<App />
    	</BrowserRouter>

2. Create firebase.init.js file inside src directory and paste the code copied from firebase
2.1 Add below code to firebase.init.js

	import { getAuth } from 'firebase/auth';

	
	const auth = getAuth(app);
	export default auth;

3. import toastify css files and ToastContainer into App.js
	import 'react-toastify/dist/ReactToastify.css';
	import { ToastContainer } from 'react-toastify';
	
3.1 Add this after <Footer/>
	<ToastContainer />

