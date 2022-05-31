# Pipeline process

 1. `environment is set up` this step set up node.js and npm and aws cli 
 2. `backend install` this step install packages for backend `npm run backend:install`
 3. `frontend install` this step install packages for frontend `npm run frontend:install`
 4. `backend build` this step build the backend `npm run backend:build`
 5. `frontend build` this step build the frontend `npm run frontend:build`
 6. `backend test` this step test the backend `npm run backend:test`
 7. `frontend test` this step test the frontend `npm run frontend:test`
 8. `frontend e2e` this step test the frontend `npm run frontend:e2e`
 9. `frontend deploy` this step deploy the frontend `npm run frontend:deploy`