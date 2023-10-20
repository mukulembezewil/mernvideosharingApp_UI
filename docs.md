- DEPLOYING A REACT APP CREATED WITH create-react-app TO GITHUB PAGES.

    https://github.com/gitname/react-gh-pages

# NB: A react app created with create-react-app has a react-scripts package in the package.json

While deploying this ReactJS app I learnt that If the BrowserRouter is not rendering anything due to a mismatch between the URL and the specified basename, it might be because the basename prop is not being applied correctly or the routing configuration is not matching the URLs as expected.

  Browser was giving the error: 
    router.ts:11 <Router basename="/mernvideosharingApp_UI"> is not able to match the URL "/" because it does not start with the basename, so the <Router> won't render anything.warning @ router.ts:11

To resolve this I needed to set <BrowserRouter basename="/mernvideosharingApp_UI"> in App.jsx
And then "homepage": "https://mukulembezewil.github.io/mernvideosharingApp_UI/", in package.json
The above match the repository name on github and the homepage url on github pages respectively.
     
Then of course re deployed. And homepage displayed the card components on the homepage as expected.