## 🧩 Troubleshooting Notes

> 🔗 Reference implementation: (https://github.com/ByteBug64/static-web.git)

During this lab, the following issues were encountered and resolved:

- CloudFront returned AccessDenied due to missing default root object
- Cached content caused outdated files to load
- Incorrect deployment of source files instead of build output
- MIME type errors due to missing assets

These issues were resolved by:
- Setting `index.html` as the default root object
- Invalidating CloudFront cache (`/*`)
- Deploying correct build artifacts (`dist/` when using Vite)
