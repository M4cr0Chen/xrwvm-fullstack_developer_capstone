# **README File**

## **Car Dealership Full Stack Web Application**

"Car Dealership" is a full stack web application that utilize
- React.js
- Node.js
- Django
- Python
- HTML / CSS
- Kubernetes
- Docker
- Express
- SQLite
- MongoDB
- Flask
enabling users to view, search and review information about car dealerships in the country.

## **Introduction**

Car Dealership is a capstone project that allow users to view dealerships across the country. Users can register account, login to their account, view the specific information about any car dealership recorded, post reviews to the dealership with the Car Type and Year. The dealerships' review component is AI powered with IBM's Artificial-Intelligence emotion sensor to recognize the review's attitude, providing enriched information to the user.

## **Installation**

To install Project Title, follow these steps:

1. Clone the repository: **`https://github.com/M4cr0Chen/xrwvm-fullstack_developer_capstone.git`**
2. Navigate to the project directory: **`cd xrwvm-fullstack_developer_capstone`**
3. Install dependencies: **`npm install`**
6. Build the project: **`npm run build`**
7. Start the project: **`npm start`**
4. Set up the Django environment:
   ```
   pip install virtualenv
   virtualenv djangoenv
   source djangoenv/bin/activate
   ```
   Install the required packages by running the following command:
   ```
   python3 -m pip install -U -r requirements.txt
   ```
   Run the following command to perform model migration:
   ```
   python3 manage.py makemigrations
   python3 manage.py migrate
   python3 manage.py runserver
   ```
   Perform a docker build with the Dockerfile in the current directory.
   ```
   MY_NAMESPACE=$(ibmcloud cr namespaces | grep sn-labs-)
   docker build -t us.icr.io/$MY_NAMESPACE/dealership .
   ```
   Push the image to the container registry:
   ```
   docker push us.icr.io/$MY_NAMESPACE/dealership
   ```
   Deploy:
   ```
   kubectl apply -f deployment.yaml
   ```
   Port-forward the running application:
   ```
   kubectl port-forward deployment.apps/dealership 8000:8000
   ```

## **Usage**

To use Project Title, follow these steps:

1. Open the project in your favorite code editor.
2. Modify the source code to fit your needs.
3. Build the project: **`npm run build`**
4. Start the project: **`npm start`**
5. Use the project as desired.

## **Contributing**

If you'd like to contribute to Project Title, here are some guidelines:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make your changes.
4. Write tests to cover your changes.
5. Run the tests to ensure they pass.
6. Commit your changes.
7. Push your changes to your forked repository.
8. Submit a pull request.

## **License**

Project Title is released under the Apache License.

## **Authors and Acknowledgment**

Car Dealership was created by **[Zhenghong Chen & IBM](https://github.com/M4cr0Chen)**.



## **Contact**

If you have any questions or comments about the project, please contact (z253chen@uwaterloo.ca).

## **Conclusion**

Have a nice day! :-)
