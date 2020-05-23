# Firebase

## A. Develop Service

### 1. Authentication
> Complete sign-in system

Đối với những ứng dụng đơn giản thì tính năng mì ăn liền này là giải pháp nhanh chóng để làm Authentication mà không phải đi xây dựng backend service riêng.

**Support**: iOs, Android, Web, C++, Unity, NodeJS, Java

#### Methods:
- Email / Password
- Social: Google, Facebook, Twitter, Github
- Phone / SMS
- Custom (connect with existing signin system)
- Anonymous

#### Implementation Paths:

**Using FirebaseUI Auth**
1. Set up sign-in methods
2. Customize the sign-in UI
3. Use FirebaseUI to perform the sign-in flow

**Using the Firebase Authentication SDK**
1. Set up sign-in methods
2. Implement UI flows for your sign-in methods
3. Pass the user's credentials to the Firebase Authentication SDK

---

### 2. Realtime Database
> Store / Sync NoSQL Database for client - server (JSON)

Lưu trữ dưới dạng JSON (Tree) nên thường được lưu các dạng data đơn giản, không cần phải xử lý các câu query phức tạp.

**Support**: iOs, Android, Web, C++, Unity

#### Implementation Paths:
1. Integrate the Firebase Realtime Database SDKs
2. Create Realtime Database References
3. Set Data and Listen for Changes
4. Enable Offline Persistence
5. Secure your data

---

### 3. Cloud Firestore
> Store / Sync NoSQL Database for client - server (Collection / Document / Data)

Tương tự như realtime-database, cũng sync data theo thời gian thực nhưng lưu trữ dưới dạng collection, document, data (tương tự như MongoDB). Có khả năng xử lý query linh động hơn là dạng JSON.

**Support**: iOs, Android, Web, C++, Unity, NodeJS, Java, Python, GoLang

#### Implementation Paths:
1. Integrate the Cloud Firestore SDKs
2. Secure your data
3. Add Data
4. Get Data

---

### 4. Cloud Storage
> Store and serve user-generated content, such as photos or videos

Lưu trữ các file do người dùng tạo ra, upload như hình ảnh, video, doc ...

**Support**: iOs, Android, Web, C++, Unity

#### Implementation Paths:
1. Integrate the Firebase SDKs for Cloud Storage.
2. Create a Reference
3. Upload or Download
4. Secure your Files

---

### 5. Hosting
> Hosting the web app, static and dynamic content, and microservices: CSS, HTML, JS, Express.js microservices or APIs.

Web Server để chạy Single-page Web App với CSS, JS, cũng có thể chạy được NodeJS - ExpressJS

**Support**: Web

#### Implementation Paths:
1. Install the Firebase CLI
2. Set up a project directory
3. Deploy your site
4. Link to a Firebase Web App (optional)

---

### 6. Cloud Functions
> A serverless framework (JavaScript or TypeScript) run backend code

Tương tự như viết Serverless Backend, thực hiện thông qua event hoặc https request

**Support**: IOS, Android, Web, C++, Unity

#### Implementation Paths:
1. Set up Cloud Functions
2. Write functions (Javascript / TypeScript )
3. Test functions
4. Deploy and monitor

---

### 7. ML Kit
> Machine learning for mobile APP

Dùng Machine Learning (TensorFlow) xử lý các tính năng cần tới ML như nhận diện chữ viết, khuôn mặt, barcode, image label, object tracking...

**Support**: IOS, Android

#### Implementation Paths:
1. Integrate the SDK
2. Prepare input data
3. Apply the ML model to your data

---

### 8. Security Rules
> Secure your data in Cloud Firestore, Firebase Realtime Database, and Cloud Storage.

Dịch vụ hỗ trợ permission cho các dịch vụ firebase khác

**Support**: IOS, Android, Web, NodeJS

#### Implementation Paths:
1. Integrate the product SDKs
2. Write your Firebase Security Rules
3. Test your Firebase Security Rules
4. Deploy your Firebase Security Rules

## B. Quality Service

### 9. Crashlytics
> Crash reporting solution for iOS, Android, and Unity

Report khi mobile app bị crash

**Support**: IOS, Android, Unity

#### Implementation Paths:
1. Connect your app
2. Integrate the SDK
3. Check reports in the Firebase console

---

### 10. Performance Monitoring
> Automatically measure app startup time, HTTP/S network requests, and more

Tương tự như hệ thống log, đo lường thời gian start app, render ...

**Support**: IOS, Android, Web

#### Implementation Paths:
1. Add the Performance Monitoring SDK to your app
2. (Optional) Define custom traces and metrics for your app using the Performance Monitoring SDK
3. Monitor performance data in the Firebase console

---

### 11. Test Lab
> Test your app on devices hosted in a Google data center.

Tương tự như hệ thống log, đo lường thời gian start app, render ...

**Support**: IOS, Android

#### Implementation Paths:
1. Get your app ready for testing
2. Choose a test environment and a test matrix
3. Run your tests, and review test results

---

### 12. App Distribution
> Distributing your apps to trusted testers painless

Phân phối bản pre-release app đến tester dễ dàng hơn.

**Support**: IOS, Android

#### Implementation Paths:
1. Upload your latest pre-release build
2. Invite testers
3. Get feedback
4. Release new beta builds

## C. Grow Service

### 13. Predictions
> Applies machine learning to your analytics data to create dynamic user segments based on your users' predicted behavior

Dùng ML để phân tích, dự đoán hành vi, sở thích của user để từ đó tùy chọn hiển thị, cấu hình phù hợp nâng cao trải nghiệm người dùng

**Support**: IOS, Android, C++, Unity

#### Implementation Paths:
1. Add Analytics to your app
2. Enable Predictions and monitor prediction readiness
3. Access predictions results from your app with Remote Config
4. Reach users in a certain prediction segment using the Notifications composer or Firebase In-App Messaging

---

### 14. A/B Testing
>  Test changes to your app’s UI, features, or engagement campaigns

A/B Testing để thử nghiệm, đánh giá hiệu quả của tính năng mới, thay đổi UI ...

**Support**: IOS, Android

#### Implementation Paths:
1. Add Remote Config or Firebase Cloud Messaging to your app
2. Define the variants that you want to evaluate with an A/B test.
3. Define how you will measure success
4. Monitor your experiment to find the winning variant

---

### 15. Cloud Messaging
>  Cross-platform messaging

Gửi notification message đến người dùng

**Support**: IOS, Android, Web, C++, Unity

#### Implementation Paths:
1. Set up the FCM SDK
2. Develop your client app
3. Develop your app server

---

### 16. In-App Messaging
> Contextual messages

Thu hút người dùng bằng các tin nhắn theo ngữ cảnh, khuyến khích họ sử dụng các tính năng của app: Item đang khuyến mãi, thực hiện nhiệm vụ để tăng level, tips...

**Support**: IOS, Android

#### Implementation Paths:
1. Connect your app
2. Integrate the SDK
3. Create your first message

---

### 17. Remote Config
> Change the behavior and appearance of your app without publishing an app update

Thay đổi, điều khiển cấu hình, hiển thị ứng dụng từ xa.

**Support**: IOS, Android, Web, C++, Unity

#### Implementation Paths:
1. Quickly roll out changes to your app's user base
2. Customize your app for segments of your user base
3. Run A/B tests to improve your app

---

### 18. Dynamic Links
> Google URL Shortener alternative

Tạo ra short url và có thể control link đó trỏ tới đâu mà không thay đổi url đó.

**Support**: IOS, Android, Web, C++, Unity

#### Implementation Paths:
1. Set up Firebase and the Dynamic Links SDK
2. Customize your app for segments of your user base
3. Run A/B tests to improve your app

---

### 18. Dynamic Links
> Google URL Shortener alternative

Tạo ra short url và có thể control link đó trỏ tới đâu mà không thay đổi url đó.

**Support**: IOS, Android, Web, C++, Unity

#### Implementation Paths:
1. Set up Firebase and the Dynamic Links SDK
2. Customize your app for segments of your user base
3. Run A/B tests to improve your app