## Steps to Host a Static Website on AWS S3

**Step 1:** Create a bucket and name it with a unique bucket name.

**Step 2:** Upload your static files inside that bucket.

**Step 3:** In order to access the website, you must configure the following:

- Enable static website hosting (go to **Properties**).
- Uncheck **"Block all public access"** to make the website publicly accessible (go to **Permissions**).
- Edit the bucket's permissions and update the **Bucket Policy** (also under **Permissions**).

**Step 4:** You can now check the website — it should be successfully accessible!
