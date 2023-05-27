# Yupoo to Shopify - Fully Automated (beta)

## Overview
The **Yupoo to Shopify - Fully Automated (beta)** script is a new and improved method for automatically importing product data from Yupoo to your Shopify store. This is a beta release of the program, and we're excited to introduce a number of new features and improvements that make this script a more efficient and effective solution for product data import.

## New Features
### JSONL Data Storage
The script now stores scraped data in a JSONL (JSON Lines) format. JSONL is a more efficient and scalable storage format for large datasets. Each JSON object is stored on a new line, which allows the script to read or write each line (i.e., each data point) independently. This is a significant upgrade over traditional JSON storage, which requires the entire dataset to be loaded into memory.

### Direct Data Upload to Shopify
The script now uses Shopify's `stagedUploadsCreate` GraphQL mutation to create a URL for the JSONL file and directly uploads the file to Shopify. This eliminates the need for additional data transfer and streamlines the process of getting your product data into your Shopify store.

### Automated Data Import to Shopify
This script runs a `bulkOperationRunMutation` that imports the products data contained in the uploaded JSONL file directly into the Shopify store. This simplifies the process, making it easier to get your product data into your Shopify store, and ensures that the product data import happens automatically after the upload process.

### Webhook Subscription
The script creates a webhook subscription to Shopify's `BULK_OPERATIONS_FINISH` topic. This subscription notifies you when the bulk operation finishes. It's an asynchronous operation that lets your script know when the data import operation is complete, and whether it was successful.

## Benefits of Using the "Yupoo to Shopify - Fully Automated (beta)" Script
1. **Improved Efficiency**: The new script has significant improvements in efficiency, especially for large datasets, thanks to JSONL data storage and direct data upload.
2. **Automation**: With the new script, data import to Shopify is automated, saving you time and effort.
3. **Scalability**: The use of JSONL and Shopify's GraphQL API makes this script more scalable, making it a better fit for stores with large product catalogs or frequent product updates.
4. **Improved Monitoring**: The webhook subscription feature allows you to better monitor the status of your data imports, and ensure they are completing successfully.

We hope you find these new features beneficial for your Shopify store. We welcome any feedback or questions you may have as you use this new script.
