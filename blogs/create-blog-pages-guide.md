# How to Create Individual Blog Post Pages

## 🎯 Overview

I've created `blog-1.html` as a sample for "The Future of Brand Design" article. Here's how to create additional blog post pages for your other articles.

## 📝 Step-by-Step Guide

### **Step 1: Create New Blog Post Page**
1. **Copy** `blog-1.html` and rename it to `blog-2.html`, `blog-3.html`, etc.
2. **Update the file name** to match your blog post number

### **Step 2: Update Page Content**

#### **Update the Title and Meta Tags:**
```html
<title>Your Blog Post Title - Noveyo Technologies</title>
<meta name="description" content="Your blog post description...">
```

#### **Update the Article Header:**
```html
<!-- Article Title -->
<h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6 leading-tight">
    Your Blog Post Title Here
</h1>

<!-- Article Excerpt -->
<p class="text-xl text-gray-600 mb-8 leading-relaxed">
    Your blog post excerpt or summary here...
</p>
```

#### **Update the Article Meta:**
```html
<!-- Article Meta -->
<div class="flex items-center mb-6">
    <span class="bg-COLOR-100 text-COLOR-800 text-sm font-semibold px-3 py-1 rounded-full mr-4">
        Your Category
    </span>
    <div class="flex items-center text-sm text-gray-500">
        <i class="fas fa-calendar-alt mr-2"></i>
        <span>Your Date</span>
        <span class="mx-2">•</span>
        <i class="fas fa-clock mr-1"></i>
        <span>X min read</span>
    </div>
</div>
```

#### **Update the Featured Image:**
```html
<img src="YOUR_IMAGE_URL" 
     alt="Your Blog Post Title" 
     class="w-full h-64 md:h-96 object-cover">
```

#### **Update the Article Content:**
Replace the content inside `<div class="article-content">` with your full blog post content.

### **Step 3: Update the Blogs Page Links**

In `blogs.html`, update the "Read More" links to point to your new blog post pages:

```html
<a href="blog-2.html" class="text-indigo-600 hover:text-indigo-700 font-semibold text-sm transition-colors">
    Read More <i class="fas fa-arrow-right ml-1"></i>
</a>
```

## 🎨 Category Colors

Use these colors for different categories:

- **Design** → `bg-blue-100 text-blue-800`
- **Marketing** → `bg-green-100 text-green-800`
- **Branding** → `bg-purple-100 text-purple-800`
- **Technology** → `bg-indigo-100 text-indigo-800`
- **Business** → `bg-yellow-100 text-yellow-800`

## 📋 Template for New Blog Posts

Here's a quick template for creating new blog post pages:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>YOUR_BLOG_TITLE - Noveyo Technologies</title>
    <meta name="description" content="YOUR_BLOG_DESCRIPTION">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <!-- Custom Styles -->
    <style>
        .gradient-bg {
            background: linear-gradient(135deg, #41c1ba, #060644);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .article-content {
            line-height: 1.8;
        }
        
        .article-content h2 {
            font-size: 1.875rem;
            font-weight: 700;
            color: #1f2937;
            margin: 2rem 0 1rem 0;
        }
        
        .article-content h3 {
            font-size: 1.5rem;
            font-weight: 600;
            color: #374151;
            margin: 1.5rem 0 0.75rem 0;
        }
        
        .article-content p {
            margin-bottom: 1.5rem;
            color: #4b5563;
        }
        
        .article-content ul, .article-content ol {
            margin: 1rem 0;
            padding-left: 2rem;
        }
        
        .article-content li {
            margin-bottom: 0.5rem;
            color: #4b5563;
        }
        
        .article-content blockquote {
            border-left: 4px solid #3b82f6;
            padding-left: 1.5rem;
            margin: 2rem 0;
            font-style: italic;
            color: #6b7280;
        }
        
        .article-content img {
            border-radius: 0.75rem;
            margin: 2rem 0;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Navigation (copy from blog-1.html) -->
    
    <!-- Article Header -->
    <section class="py-16 bg-gradient-to-br from-blue-50 to-indigo-100">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <!-- Breadcrumb -->
            <nav class="mb-8">
                <ol class="flex items-center space-x-2 text-sm text-gray-600">
                    <li><a href="index.html" class="hover:text-indigo-600">Home</a></li>
                    <li><i class="fas fa-chevron-right text-xs"></i></li>
                    <li><a href="blogs.html" class="hover:text-indigo-600">Blogs</a></li>
                    <li><i class="fas fa-chevron-right text-xs"></i></li>
                    <li class="text-gray-900">YOUR_BLOG_TITLE</li>
                </ol>
            </nav>

            <!-- Article Meta -->
            <div class="flex items-center mb-6">
                <span class="bg-COLOR-100 text-COLOR-800 text-sm font-semibold px-3 py-1 rounded-full mr-4">
                    YOUR_CATEGORY
                </span>
                <div class="flex items-center text-sm text-gray-500">
                    <i class="fas fa-calendar-alt mr-2"></i>
                    <span>YOUR_DATE</span>
                    <span class="mx-2">•</span>
                    <i class="fas fa-clock mr-1"></i>
                    <span>X min read</span>
                </div>
            </div>

            <!-- Article Title -->
            <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6 leading-tight">
                YOUR_BLOG_TITLE
            </h1>

            <!-- Article Excerpt -->
            <p class="text-xl text-gray-600 mb-8 leading-relaxed">
                YOUR_BLOG_EXCERPT
            </p>

            <!-- Author Info -->
            <div class="flex items-center">
                <img src="YOUR_AUTHOR_IMAGE" 
                     alt="YOUR_AUTHOR_NAME" 
                     class="w-12 h-12 rounded-full mr-4">
                <div>
                    <p class="font-semibold text-gray-900">YOUR_AUTHOR_NAME</p>
                    <p class="text-sm text-gray-500">YOUR_AUTHOR_TITLE</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Article Content -->
    <article class="py-16">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="bg-white rounded-2xl shadow-lg border border-gray-200 overflow-hidden">
                <!-- Featured Image -->
                <div class="relative">
                    <img src="YOUR_FEATURED_IMAGE" 
                         alt="YOUR_BLOG_TITLE" 
                         class="w-full h-64 md:h-96 object-cover">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent"></div>
                </div>

                <!-- Article Body -->
                <div class="p-8 md:p-12">
                    <div class="article-content">
                        <!-- YOUR FULL BLOG CONTENT GOES HERE -->
                    </div>
                </div>
            </div>
        </div>
    </article>

    <!-- Related Articles (copy from blog-1.html) -->
    
    <!-- Newsletter Section (copy from blog-1.html) -->
    
    <!-- Footer (copy from blog-1.html) -->
    
    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', () => {
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenu.classList.toggle('hidden');
        });

        // Newsletter form
        document.querySelectorAll('.newsletter-form').forEach(form => {
            form.addEventListener('submit', function(e) {
                e.preventDefault();
                const email = e.target.email.value;
                if (email) {
                    alert('Thank you for subscribing to our newsletter!');
                    e.target.reset();
                }
            });
        });
    </script>
</body>
</html>
```

## ✅ Features Included in Each Blog Post Page

- **Professional layout** with header, content, and footer
- **Breadcrumb navigation** for easy navigation
- **Article meta information** (category, date, read time)
- **Author information** with profile image
- **Featured image** with overlay
- **Formatted article content** with proper typography
- **Related articles** section
- **Newsletter subscription** form
- **Mobile responsive** design
- **SEO optimized** with proper meta tags

## 🚀 Quick Steps

1. **Copy** `blog-1.html` to create `blog-2.html`
2. **Update** the title, description, and content
3. **Change** the category color and information
4. **Update** the "Read More" link in `blogs.html`
5. **Test** the page to ensure everything works

## 📱 Testing

After creating a new blog post page:
1. **Open** the page in your browser
2. **Check** that all links work correctly
3. **Test** the mobile responsive design
4. **Verify** the navigation and breadcrumbs
5. **Ensure** the content displays properly

**This system allows you to create professional, individual blog post pages that are easy to maintain and update!** ✨
