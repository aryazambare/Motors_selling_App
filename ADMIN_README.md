# PRAGATI MOTORS - Admin Panel

A comprehensive admin panel for managing tractor products, including photo uploads, pricing, and inventory management.

## 🚜 Features

### **Product Management**
- ✅ **Add New Products** with detailed information
- ✅ **Edit Existing Products** with all fields
- ✅ **Delete Products** with confirmation
- ✅ **Search Products** by name or description
- ✅ **Filter by Category** (Compact, Utility, Heavy-Duty)
- ✅ **Price Management** with currency formatting

### **Photo Management**
- ✅ **Multiple Photo Upload** (drag & drop or click to upload)
- ✅ **Photo Preview** with click-to-enlarge
- ✅ **Cover Photo Selection** from uploaded photos
- ✅ **Photo Removal** with individual delete buttons
- ✅ **File Size Validation** (5MB limit per image)
- ✅ **Image Format Support** (JPG, PNG, GIF)

### **Data Management**
- ✅ **Local Storage** for data persistence
- ✅ **Export Products** to JSON file
- ✅ **Import Products** from JSON file
- ✅ **Real-time Statistics** dashboard
- ✅ **Form Validation** with error messages

### **User Experience**
- ✅ **Responsive Design** for all devices
- ✅ **Modern UI** with smooth animations
- ✅ **Keyboard Shortcuts** (Ctrl+N, Escape)
- ✅ **Notification System** for user feedback
- ✅ **Modal Dialogs** for better UX

## 📁 File Structure

```
pragati-motors-admin/
├── admin.html          # Admin panel HTML
├── admin-styles.css    # Admin panel styles
├── admin-script.js     # Admin functionality
├── index.html          # Main website
├── styles.css          # Website styles
├── script.js           # Website functionality
└── ADMIN_README.md     # This documentation
```

## 🚀 Getting Started

1. **Open** `admin.html` in your web browser
2. **Start Adding Products** using the "Add Product" button
3. **Upload Photos** by clicking the upload area or dragging files
4. **Select Cover Photo** from uploaded images
5. **Save Products** and manage your inventory

## 📋 Product Fields

### **Required Fields**
- **Product Name** - The name of the tractor
- **Price** - Cost in dollars (supports decimals)
- **Category** - Compact, Utility, or Heavy-Duty
- **Description** - Detailed product description
- **Photos** - At least one image required
- **Cover Photo** - Main display image

### **Optional Fields**
- **Horsepower** - Engine power specification
- **Key Features** - Bullet points of features (one per line)

## 🖼️ Photo Management

### **Uploading Photos**
1. Click the upload area or drag files onto it
2. Select multiple images at once
3. Files are validated for size (5MB max) and format
4. Photos appear as thumbnails with action buttons

### **Setting Cover Photo**
1. Upload multiple photos
2. Click the star icon on any photo to set as cover
3. Or click on photos in the cover selection area
4. Cover photo is used as the main product image

### **Managing Photos**
- **Preview**: Click any photo to view full size
- **Remove**: Click trash icon to delete individual photos
- **Cover**: Click star icon to set as cover photo

## 📊 Dashboard Statistics

The admin panel displays real-time statistics:
- **Total Products** - Number of products in inventory
- **Average Price** - Mean price of all products
- **Total Images** - Total number of uploaded photos

## 🔍 Search & Filter

### **Search Products**
- Type in the search box to find products by name or description
- Search is case-insensitive and real-time

### **Filter by Category**
- Use the dropdown to filter by tractor category
- Options: All Categories, Compact, Utility, Heavy-Duty

## 💾 Data Management

### **Local Storage**
- All data is automatically saved to browser's local storage
- Data persists between browser sessions
- No server required for basic functionality

### **Export Products**
- Click "Export" button to download all products as JSON
- Useful for backup and data migration
- File name: `pragati-motors-products.json`

### **Import Products**
- Click "Import" button to upload a JSON file
- Replaces all existing products with imported data
- Useful for restoring from backup

## ⌨️ Keyboard Shortcuts

- **Ctrl + N** - Add new product
- **Escape** - Close any open modal

## 📱 Responsive Design

The admin panel is fully responsive and works on:
- **Desktop** - Full feature set with grid layout
- **Tablet** - Adapted layout with touch-friendly controls
- **Mobile** - Single-column layout with optimized forms

## 🎨 Customization

### **Colors**
The admin panel uses the same color scheme as the main website:
- Primary Green: `#2c5530`
- Secondary Green: `#4a7c59`
- Accent Gold: `#ffd700`

### **Adding New Categories**
To add new tractor categories:
1. Update the select options in `admin.html`
2. Add category labels in `admin-script.js` `getCategoryLabel()` function
3. Update the main website to display new categories

## 🔧 Technical Details

### **Browser Support**
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### **File Size Limits**
- Individual photos: 5MB maximum
- Total storage: Limited by browser's local storage (typically 5-10MB)

### **Data Format**
Products are stored as JSON objects with the following structure:
```json
{
  "id": "unique_id",
  "name": "Product Name",
  "price": 25000.00,
  "category": "compact",
  "horsepower": "25-35 HP",
  "description": "Product description",
  "features": ["Feature 1", "Feature 2"],
  "photos": [
    {
      "id": "photo_id",
      "data": "base64_image_data",
      "name": "filename.jpg"
    }
  ],
  "coverPhoto": "photo_id",
  "createdAt": "2024-01-01T00:00:00.000Z",
  "updatedAt": "2024-01-01T00:00:00.000Z"
}
```

## 🚨 Troubleshooting

### **Common Issues**

**Photos not uploading:**
- Check file size (must be under 5MB)
- Ensure file is an image (JPG, PNG, GIF)
- Try refreshing the page

**Data not saving:**
- Check if local storage is enabled in browser
- Clear browser cache and try again
- Export data as backup before troubleshooting

**Form validation errors:**
- Ensure all required fields are filled
- Check that at least one photo is uploaded
- Verify a cover photo is selected

### **Browser Compatibility**
If features don't work:
- Update to the latest browser version
- Enable JavaScript
- Allow local storage
- Try a different browser

## 🔮 Future Enhancements

- **Bulk Operations** - Select multiple products for batch actions
- **Product Categories** - Custom category management
- **Image Optimization** - Automatic image compression
- **Advanced Search** - Filter by price range, date, etc.
- **Product Templates** - Save common product configurations
- **Analytics** - Track product views and performance
- **User Management** - Multiple admin accounts
- **API Integration** - Connect to external inventory systems

## 📞 Support

For technical support or feature requests:
- Check the browser console for error messages
- Export your data before making changes
- Test in different browsers if issues persist

---

**PRAGATI MOTORS Admin Panel** - Manage your tractor inventory with ease! 🚜
